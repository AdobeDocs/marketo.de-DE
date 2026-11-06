---
description: Verwenden Sie aufrufbare Agenten in CX Enterprise Coworker für Marketo Engage, um KI-Schritte in Smart Campaign auszuführen, die Daten bereinigen, klassifizieren, anreichern oder auf dem Bildschirm anzeigen.
title: Aufrufbare Agenten
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
source-git-commit: 16b8e470bd4a4460c0179ccdd406ef89af7e9e17
workflow-type: tm+mt
source-wordcount: '2002'
ht-degree: 1%
---
# Aufrufbare Agenten {#callable-agents}

Mit aufrufbaren Agenten können Sie einen KI-Agenten als Schritt in einer Marketo Engage Smart Campaign verwenden. Erstellen Sie einen Agenten in CX Enterprise Coworker für Marketo Engage, wählen Sie die Lead-Felder aus, die er liest und aktualisiert, und veröffentlichen Sie ihn zur Verwendung in Kampagnen. Agenten können dabei helfen, Daten zu bereinigen, Leads zu klassifizieren, fehlende Informationen anzureichern oder Formularübermittlungen auf dem Bildschirm anzuzeigen.

>[!PREREQUISITES]
>
>Sie müssen über die Berechtigung **Zugriffsadministrator** in Marketo Engage verfügen.

## Voraussetzungen {#before-you-begin}

- Entscheiden Sie, welche Lead-Felder der Agent lesen muss und welche Felder er aktualisieren soll. Jede Eingabe und Ausgabe muss einem Marketo Engage-Lead-Feld zugeordnet sein.
- Überprüfen, ob Ausgabefelder aktualisierbar sind. Schreibgeschützte Felder und Felder für Programmmitglieder werden nicht unterstützt.

## Informationen zur Verwendung {#how-to-use}

1. Klicken Sie in „Mein Marketo&quot; auf die Kachel **[!UICONTROL CX Enterprise Coworker für Marketo Engage]** .

1. Wählen Sie **[!UICONTROL aufrufbare Agenten]** im linken Navigationsbereich aus. Die Liste enthält den Namen, das Erstellungsdatum, den Ersteller und den Status jedes Agenten. Nach Name suchen oder nach Name oder Erstellungsdatum sortieren.

1. Wählen Sie **[!UICONTROL Aufrufbaren Agenten erstellen]** aus. Wählen Sie eine Vorlage aus oder lassen Sie die Vorlagenauswahl leer, um von Grund auf neu zu beginnen.

1. Geben Sie einen **[!UICONTROL Agentennamen]** ein und schreiben Sie **[!UICONTROL Agentenanweisungen]** in denen beschrieben wird, wie die einzelnen Leads verarbeitet werden.

1. Fügen **[!UICONTROL unter „Zu sendende Lead]** die Lead-Felder hinzu, die der Agent als Eingabe benötigt. Fügen Sie unter **[!UICONTROL Zu aktualisierende Lead]** jeden Wert hinzu, den der Agent zurückgeben soll, und ordnen Sie ihn einem aktualisierbaren Lead-Feld zu.

1. Wählen Sie **[!UICONTROL Speichern]**, um einen Entwurf zu speichern, oder **[!UICONTROL Speichern und Veröffentlichen]**, um den Agenten in Marketo Engage verfügbar zu machen.

1. Öffnen Sie eine Smart-Kampagne und wählen Sie die Registerkarte **[!UICONTROL Fluss]** aus. Suchen Sie im Abschnitt Marketing der Flussschritt-Liste nach **Aufrufagent: _[Agentenname]_**und ziehen Sie ihn in den Fluss.

1. Testen Sie die Kampagne mit einer kleinen Gruppe von Leads. Überprüfen Sie das Aktivitätsprotokoll und bestätigen Sie, dass die Ausgabefelder wie erwartet aktualisiert werden, bevor Sie die Kampagne für alle Leads aktivieren.

## Zu beachtende Punkte {#things-to-note}

- Ein aufrufbarer Agent verarbeitet jeden Lead unabhängig voneinander. Marketo Engage sendet die zugeordneten Lead-Werte an den Agenten, schreibt die zurückgegebenen Werte in die zugeordneten Lead-Felder und fährt mit dem nächsten Kampagnenschritt fort.
- Sie können aufrufbare Agenten in CX Enterprise Coworker für Marketo Engage erstellen und verwalten. Es ist keine externe Verbindung erforderlich.
- Veröffentlichte Agenten können nicht bearbeitet werden. Um einen bereits veröffentlichten Agenten zu ändern, müssen Sie einen neuen Agenten erstellen und die entsprechenden Smart-Kampagnen aktualisieren.

## Erstellen eines Agenten {#create-an-agent}

### Neuerstellen eines Agenten {#create-an-agent-from-scratch}

Lassen Sie die Vorlagenauswahl leer. Das Formular beginnt mit einem leeren Eingabefeld und einem leeren Ausgabefeld. Geben Sie den Namen und die Anweisungen ein und konfigurieren Sie dann die Eingabe- und Ausgabefelder so, dass sie Ihrer Geschäftsregel entsprechen.

### Von einer Vorlage starten {#start-from-a-template}

Wählen Sie eine Vorlage aus, um die Anweisungen, Eingabefelder und Ausgabefelder vorauszufüllen. Der Agent wird als eigene Kopie gespeichert, die Sie bearbeiten oder löschen können. Wenn Sie einen aus einer Vorlage erstellten Agenten löschen, wird die Vorlage wieder in der Auswahl verfügbar.

| Vorlage | Zweck | Eingaben | Ausgaben |
| --- | --- | --- | --- |
| Normalisierer für Firmennamen | Bereinigt Firmennamen durch Entfernen rechtlicher Suffixe, Korrigieren gängiger Tippfehler und Anwenden der standardmäßigen Markengroßschreibung. | Unternehmen | Normalisierte Firma (Text); Konfidenz (Zahl) |
| Formatierer E.164 Telefon | Formatiert Telefonnummern nach dem internationalen E.164-Standard. | Telefon | Normalisierte Telefonnummer (Text); Konfidenz (Zahl) |
| Job Title Standardizer | Standardisiert Stellenbezeichnungen und leitet Dienstalter ab. | Titel | Normalisierter Titel (Text); Dienstalter (C-Level, VP, Director, Manager, Person oder Unbekannt); Konfidenz |
| Bot- und Spam-Erkennung | Kennzeichnet Bot- oder Spam-Formularübermittlungen. | E-Mail, Vorname, Nachname, Firma, Telefon | Ist nicht (true/false); Konfidenz; Grund; Flags (kommagetrennt) |
| Einweg-E-Mail-Detektor | Identifiziert temporäre oder Wegwerf-E-Mail-Adressen. | E-Mail | Ist nicht (true/false); Konfidenz; Grund; E-Mail-Typ (Einweg, privat oder geschäftlich) |
| Lead-Klassifikator | Segmente Leads nach Unternehmensgröße, Branche, Rolle und Absicht. | Firma, Titel, E-Mail, Mitarbeiter, Umsatz | Segment (Enterprise, Mid-Market, SMB, Startup oder Unknown); Branche; Persona; Absichtsebene (Hoch, Medium oder Niedrig); Konfidenz |
| Lead-Anreicherung | leitet fehlende Lead-Details aus den verfügbaren Informationen ab. | E-Mail, Titel, Firma | Abgeleitetes Unternehmen, Abteilung, Dienstalter, ist Entscheidungsträger (true/false), ist B2B (true/false), Vertrauen |
| Unternehmensforschung | Generiert Vertriebsdaten aus Unternehmensinformationen. | Unternehmen, Website, Beschreibung | Die vollständige Liste finden Sie in der Vorlage . |

### Effektive Anweisungen schreiben {#write-effective-instructions}

- Fügen Sie allgemeine Regeln und Beispiele in die Agentenanweisungen ein. Verwenden Sie Feldanweisungen, um die Erwartungen für eine einzelne Ausgabe anzugeben.
- Seien Sie spezifisch. Beispielsweise ist „Entfernen rechtlicher Suffixe wie Inc, LLC und Corp“ klarer als „Bereinigen von Firmennamen“.
- Beispiele für Inputs und erwartete Outputs, insbesondere für Randfälle, einschließen.
- Geben Sie an, was der Agent zurückgeben soll, wenn er keine Entscheidung treffen kann, z. B. „Wenn Sie sich nicht sicher sind, geben Sie den ursprünglichen Wert zurück.“
- Fügen Sie eine Konfidenzausgabe hinzu, damit Kampagnenlogik Ergebnisse mit geringer Konfidenz zur Überprüfung weiterleiten kann.
- Eingabeaufforderungen kurz halten. Kürzere Eingabeaufforderungen werden schneller ausgeführt und kosten weniger.

## Speichern, Veröffentlichen und Verwalten von Agenten {#save-publish-and-manage-agents}

### Als Entwurf oder Veröffentlichung speichern {#save-as-a-draft-or-publish}

Wählen Sie **[!UICONTROL Speichern]**, um den Agenten als Entwurf zu speichern. Entwürfe können bearbeitet werden, sind jedoch nicht als Workflow-Schritte in Smart Campaign verfügbar. Wählen Sie **[!UICONTROL Speichern und veröffentlichen]** wenn der Agent bereit ist. Marketo Engage stellt den Agenten als Flussschritt zur Verfügung und kehrt mit einer Veröffentlichungsbestätigung zur Agentenliste zurück. Wählen Sie **[!UICONTROL Abbrechen]** aus, um den Vorgang ohne Speichern zu beenden.

| Status | Bedeutung | Verfügbare Aktion |
| --- | --- | --- |
| Entwurf | Der Agent wird gespeichert, ist aber in Marketo Engage nicht verfügbar. | Bearbeiten Sie es und wählen Sie dann **[!UICONTROL Speichern und veröffentlichen]** aus, wenn es fertig ist. |
| Veröffentlicht | Der Agent ist in Smart-Kampagnen verfügbar. Veröffentlichte Agenten werden eingefroren. | Verwenden Sie den veröffentlichten Agenten oder erstellen Sie einen neuen Agenten, um Änderungen vorzunehmen. |
| Veröffentlichung fehlgeschlagen | Marketo Engage hat den Agenten beispielsweise abgelehnt, weil ein Ausgabefeldname reserviert ist. Der Agent wird jedoch weiterhin als Entwurf gespeichert. | Bearbeiten Sie den Agenten, korrigieren Sie das in der Nachricht benannte Feld und veröffentlichen Sie erneut. |

### Bearbeiten, Überprüfen der Nutzung oder Löschen {#edit-check-usage-or-delete}

- Wählen Sie **[!UICONTROL Bearbeiten]** für einen Entwurf aus, um ihn zu ändern. **[!UICONTROL Speichern]** behält Sie auf der Seite und zeigt eine Bestätigung „Agent gespeichert“ an. Sie können auch **[!UICONTROL Speichern und Veröffentlichen]**, **[!UICONTROL Abbrechen]** oder **[!UICONTROL Löschen]** auswählen.
- Veröffentlichte Agenten werden eingefroren, da intelligente Kampagnen von ihnen abhängen können. Erstellen Sie einen neuen Agenten, um Änderungen vorzunehmen.
- Überprüfen Sie **[!UICONTROL Verwendet von]** um zu sehen, welche Smart-Kampagnen auf einen Agenten verweisen, bevor Sie einen Agenten löschen oder seine Kampagneneinrichtung ändern.
- Sie können einen Agenten nicht löschen, während eine Smart Campaign ihn noch verwendet. Entfernen Sie den Flussschritt des Agenten aus jeder aufgelisteten Kampagne und löschen Sie dann den Agenten.

## Integration von Organisationsregeln {#organizational-rules-integration}

### Benennungskonventionen {#naming-conventions}

- **Agentenname:** 1-100 Zeichen und eindeutig im Abonnement. Der Name wird auch im Schritt Smart-Campaign-Fluss verwendet. Wählen Sie einen erkennbaren Namen aus, z. B. `Company Name Normalizer`.
- **Name des Ausgabefelds:** Verwenden Sie Buchstaben, Ziffern und Unterstriche. Der Name muss mit einem Buchstaben oder einem Unterstrich beginnen, eindeutig sein und nicht mehr als 64 Zeichen lang sein.
- **Reservierte Namen:** Einige Ausgabenamen sind für die Verwendung durch das System reserviert. Wenn ein Name abgelehnt wird, wählen Sie einen anderen Namen, z. B. `qualificationReason` anstelle von `reason`.

### Erforderliche Elemente und unterstützte Felder {#required-elements-and-supported-fields}

- Ordnen Sie vor dem Speichern jedes Eingabefeld einem Marketo Engage-Lead-Feld zu.
- Konfigurieren Sie mindestens ein Ausgabefeld. Ordnen Sie jede Ausgabe einem aktualisierbaren Lead-Feld zu. Schreibgeschützte Felder sind in der Feldauswahl nicht verfügbar.
- Die Felder für Programmteilnehmer werden nicht unterstützt. Die Feldauswahl zeigt nur Lead-Felder an.
- Unterstützte Ausgabetypen sind **Text**, **Number** und **True/False**.
- Um eine Liste zurückzugeben, verwenden Sie einen kommagetrennten Textwert und beschreiben Sie das erwartete Format in den Feldanweisungen.
- Bei jeder erfolgreichen Ausführung werden genau die konfigurierten Ausgabefelder zurückgegeben.

### Beschränkungen {#limits}

| Einstellung | Beschränkungen |
| --- | --- |
| Agentenname | 1-100 Zeichen; eindeutig innerhalb des Abonnements |
| Agent-Anweisungen | 1-4.000 Zeichen |
| Eingabefelder | Bis zu 20; jede muss einem Lead-Feld zugeordnet sein |
| Output fields | 1-20; jede muss einem aktualisierbaren Lead-Feld zugeordnet werden |
| Name des Ausgabefelds | Bis zu 64 Zeichen; Buchstaben, Ziffern und Unterstriche; beginnt mit einem Buchstaben oder einem Unterstrich; eindeutig |
| Anweisungen für Ausgabefelder | Bis zu 512 Zeichen |
| Leads pro Anfrage | Bis zu 1.000 Leads aus Marketo Engage, parallel verarbeitet |

## Inhalts-Screening und Datenverarbeitung {#content-screening-and-data-handling}

Wenn Sie einen Agenten erstellen oder seine Anweisungen bearbeiten, überprüft Marketo Engage die Anweisungen für Agenten und die Ausgabefelder auf Richtlinienverletzungen, sofortige Injektion und Versuche zur Datenextraktion. Beispiele sind Anfragen zum Anzeigen von Anmeldeinformationen oder zum Überschreiben des Agentenverhaltens. Wenn Inhalte gekennzeichnet sind, wird das Speichern blockiert und es kann eine Meldung angezeigt werden, z. B. „Eingabeaufforderung enthält eingeschränkten Inhalt“ oder „Eingabeaufforderung für fehlgeschlagene Inhaltsmoderation“. Den Text überarbeiten und erneut speichern.

- **Zugriff:** Die Verwaltung von Agenten erfordert die Berechtigung **Zugriff auf Admin**. Agenten und Anrufverlauf werden durch Abonnements isoliert.
- **Lead-Datenschutz:** Lead-Daten werden getrennt von Agentenanweisungen weitergeleitet, wobei die Lead-Werte als Daten und nicht als Befehle behandelt werden.
- **Inhaltsrichtlinie:** Wenn die Daten eines Leads gegen die Inhaltsrichtlinie des KI-Anbieters verstoßen, erhält dieser Lead eine Fehleraktivität anstelle eines Ergebnisses.
- **Bindung** Anfrage- und Antwort-Payloads, einschließlich der an den Agenten gesendeten Lead-Feldwerte, werden 30 Tage lang im Anrufverlauf aufbewahrt, um die Fehlerbehebung zu unterstützen, und dann automatisch gelöscht.

## Ausführen von aufrufbaren Agenten in einer Kampagne {#how-callable-agents-run-in-a-campaign}

1. Wenn die Kampagne ausgeführt wird, sendet Marketo Engage die zugeordneten Lead-Feldwerte für jeden qualifizierten Lead an den Agenten.
1. Der Agent verarbeitet jeden Lead unabhängig voneinander und gibt die konfigurierten Ausgabefelder zurück.
1. Marketo Engage schreibt die Ergebnisse in die zugeordneten Lead-Felder. Geänderte Felder werden auch als standardmäßige Datenwertänderungsaktivitäten angezeigt.
1. Die Kampagne geht zum nächsten Schritt über.

Die Verarbeitung erfolgt asynchron. Der Flussschritt wartet bis zum Fenster mit dem Flussschritt-Warten in Marketo Engage auf ein Ergebnis. Wenn ein Lead fehlschlägt (z. B. aufgrund einer Zeitüberschreitung), erhält dieser Lead eine Fehleraktivität und andere Leads bleiben erhalten. Jedes Ergebnis wird im Aktivitätsprotokoll des Leads für den aufrufbaren Agenten angezeigt.

Verwenden Sie Ausgabefelder in der Kampagnenlogik. Verzweigung auf **Ist nicht**, um Spam-Übermittlungen anders zu leiten, oder Verzweigung auf **Konfidenz**, um Ergebnisse mit geringer Konfidenz an einen Überprüfungsschritt zu senden.

## Prä-Aktivierungs-QA {#pre-activation-qa}

Vor der Aktivierung einer Kampagne für alle Leads:

- Führen Sie die Kampagne mit einem kleinen Testsatz von Leads aus.
- Überprüfen Sie das Aktivitätsprotokoll jedes Leads und bestätigen Sie, dass die Ausgabefelder korrekt aktualisiert wurden.
- Testen Sie Edge-Fälle, einschließlich fehlender Werte und ungewöhnlicher Eingaben.
- Vergewissern Sie sich, dass Kampagnenzweige Werte wie geringe Konfidenz oder eine Bot-/Spam-Klassifizierung wie beabsichtigt verarbeiten.

## Anwendungsfälle {#use-cases}

- **Datenbereinigung:** Standardisieren Sie Firmennamen, formatieren Sie Telefonnummern auf E.164 und normalisieren Sie Auftragstitel, wenn Leads erstellt oder importiert werden.
- **Bot- und Spam-Screening:** Überprüfen Sie die Einreichungen auf spitzfindige Namen, verdächtige E-Mails und wiederholte Ziffern der Telefonnummern. Verzweigen Sie die Kampagne basierend auf dem Ergebnis.
- **Einweg-E-Mail-Erkennung:** Identifizieren Sie temporäre E-Mail-Adressen und leiten Sie sie anders als Geschäftsadressen weiter.
- **Lead-Klassifizierung:** Segment-Leads nach Unternehmensgröße, Branche, Rolle und Absicht, um Routing oder Bewertung zu unterstützen.
- **Lead-Anreicherung:** Ziehen Sie fehlende Details wie Abteilung, Dienstalter oder die Frage, ob ein Lead ein Entscheidungsträger ist.
- **Benutzerdefinierte Regeln:** Erstellen Sie eine Ja/Nein-Prüfung oder Kategorisierung, die als Lead-Verarbeitungsregel beschrieben werden kann, z. B. das Kennzeichnen von Leads aus einer Region oder Branche.

## Fehlerbehebung {#troubleshooting}

| Problem | Auflösung |
| --- | --- |
| **Agenten** wird in der Navigation nicht angezeigt. | Bitten Sie Ihren Marketo Engage-Administrator, die Berechtigung **Zugriffsadministrator** zu erteilen. |
| Das Speichern ist mit einer Inhaltsmeldung blockiert. | Ändern Sie die Agentenanweisungen oder Feldanweisungen, um den gekennzeichneten Inhalt zu entfernen, und speichern Sie dann erneut. |
| Der Agentstatus lautet **Veröffentlichung fehlgeschlagen**. | Bearbeiten Sie den Agenten, korrigieren Sie das in der Nachricht benannte Feld und wählen Sie **Speichern und veröffentlichen** aus. |
| Veröffentlichte Agenten können nicht bearbeitet werden. | Veröffentlichte Agenten werden eingefroren. Erstellen Sie einen neuen Agenten, um Änderungen vorzunehmen. |
| Ein Agent kann nicht gelöscht werden. | Entfernen Sie den entsprechenden Flussschritt aus jeder Smart-Kampagne, die unter Verwendung des Agenten aufgeführt wird, und löschen Sie ihn dann. |
| Ein Feldname wird als reserviert gemeldet. | Wählen Sie einen anderen Ausgabefeldnamen aus, z. B. `qualificationReason`, und speichern Sie erneut. |
| Einige Leads erhalten eine Fehleraktivität. | Überprüfen Sie das Aktivitätsprotokoll des Leads. Einzelne Fehler, einschließlich Zeitüberschreitungen oder Inhaltsrichtlinienverletzungen, wirken sich nicht auf andere Leads aus. |
| Die Ergebnisse sind unerwartet. | Machen Sie die Anweisungen spezifischer, fügen Sie Beispiele hinzu, verfeinern Sie die Feldanweisungen und testen Sie sie erneut mit einem kleinen Satz Leads. |

## Nächste Schritte {#next-steps}

- Überprüfen Sie die Liste **Verwendet von** des Agenten und bestätigen Sie, welche Smart-Kampagnen ihn verwenden werden.
- Testen Sie den Flussschritt mit einer kleinen Gruppe von Leads und validieren Sie die Aktivitätsprotokolle und Ausgabefelder.
- Verwenden Sie die Ausgabefelder, um Kampagnenverzweigungen für Klassifizierungen oder Ergebnisse mit geringer Konfidenz hinzuzufügen.
- Entfernen Sie den Schritt Agentenfluss aus allen Kampagnen, bevor Sie den Agenten löschen.
