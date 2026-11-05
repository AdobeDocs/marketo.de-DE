---
description: Verwenden Sie CX Enterprise Coworker für Marketo Engage, um eine Kampagnenübersicht in einen strukturierten Programmplan umzuwandeln, der Zielgruppenlogik, E-Mails, Token und QA-Prüfungen abdeckt.
title: Kampagnen planen
source-git-commit: e72db83a5f1f3c58a29da7c4b4b1bbb79a61b596
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 1%
---
# Kampagnen planen {#plan-campaigns}

Umwandeln einer Kampagnenbeschreibung in einen strukturierten Implementierungsplan für Marketo Engage. Die Fähigkeit Kampagnen planen skizziert die Programmstruktur, Zielgruppenlogik, E-Mails, intelligente Kampagnen, Token, Reporting und Prüfungen vor der Aktivierung. Die Ausgabe ist ein herunterladbarer Bericht, der im Arbeitsbereich-Bedienfeld angezeigt wird.

>[!NOTE]
>
>- Diese Fähigkeit generiert Implementierungspläne für Marketo Engage-Programme (strukturierte Dokumente, die einem menschlichen oder Automatisierungssystem genau sagen, wie eine Kampagne zu erstellen ist). In Marketo Engage werden keine Elemente erstellt. Es gibt eine separate Fähigkeit für [Erstellen von Programmen](/help/marketo/product-docs/coworker-for-marketo/skills/build-programs.md){target="_blank"}.
>- Diese Fähigkeit basiert auf [Organisationsregeln](/help/marketo/product-docs/coworker-for-marketo/organizational-rules.md){target="_blank"}.

## Voraussetzungen {#prerequisites}

- Geben Sie für einen Programmplan einen Überblick über die Kampagne mit den verfügbaren Informationen wie Kampagnenziele, Zielgruppe, Messaging, Timeline und Erfolgsmetriken.
- Um eine bestehende Zusammenfassung oder einen Plan zu verbessern, geben Sie das Dokument an und beschreiben Sie die gewünschten Änderungen.
- Um ohne eine Zusammenfassung zu beginnen, fordern Sie eine Beispielbeschreibung an oder fragen Sie nach einem Plan, der auf einem allgemeinen Kampagnenszenario basiert.

## Informationen zur Verwendung {#how-to-use}

1. Klicken Sie in „Mein Marketo&quot; auf die Kachel **[!UICONTROL CX Enterprise Coworker für Marketo Engage]** .

1. Wählen Sie die **[!UICONTROL Kampagnen planen]** und klicken Sie auf **[!UICONTROL Diese Qualifikation verwenden]**.

1. Wählen Sie aus, was Sie tun möchten:
   - Planen eines Programms aus einer Kampagnenbeschreibung.
   - Generieren einer Beispiel-Kampagnenbeschreibung.
   - Polnisch einen bestehenden Brief.
   - Überarbeiten eines vorhandenen Einrichtungsplans.

1. Stellen Sie die Zusammenfassung oder das Dokument bereit. Schließen Sie alle spezifischen Änderungen, Kampagnenanforderungen oder organisatorischen Konventionen ein.

1. Überprüfen Sie den generierten Bericht im Arbeitsbereich-Bedienfeld. Öffnen Sie sie, um die Details zu überprüfen oder den Bericht herunterzuladen.

1. Überprüfen und genehmigen Sie den Einrichtungsplan, bevor Sie das Programm in Marketo Engage erstellen.

## SKILL options {#skill-options}

### Planen eines Programms {#plan-a-program}

Ein Programmplan setzt Kampagnenanforderungen in Anweisungen zum Erstellen des Programms um. Abhängig von der Zusammenfassung kann sie Folgendes umfassen:

- **Programmübersicht:** Kampagnenname, Ziele, Zielgruppe und Zeitleiste.
- **Ordnerstruktur:** empfohlene lokale Ordner für E-Mails, intelligente Kampagnen und Berichte.
- **Smart Lists:** Segmentierungslogik, Filterdefinitionen und erforderliche Ausschlüsse.
- **E-Mail-Konfiguration** Betreffzeilen, Preheader-Text, Inhaltsstruktur, Absenderdetails und Compliance-Elemente.
- **Intelligente Kampagnen:** Kampagnennamen, Trigger- oder Batch-Bestimmung, Flussschritte und Zeitplanempfehlungen.
- **Token und Felder:** Meine Token, erforderliche und benutzerdefinierte Token und alle erforderlichen benutzerdefinierten Felder mit ihren Typen und Werten.
- **Journey-Fluss:** Kampagnensequenz, Warteschritte und Entscheidungslogik.
- **Reporting und QA:** Erfolgsmetriken, empfohlene Berichte und Validierungsprüfungen vor der Aktivierung.

### Erstellen einer Beispielbeschreibung {#create-a-sample-brief}

Fordern Sie eine kurze Beispielbeschreibung an, wenn Sie möchten, dass ein Beispiel angepasst wird. Sie können ein Thema oder einen Kampagnentyp angeben, z. B. einen Produktstart oder ein Webinar. Wenn Sie um einen Plan bitten, ohne einen kurzen Überblick zu geben, kann die Kenntnisse ein Beispielszenario wie ein Webinar zur Produkteinführung als Grundlage für den Plan verwenden.

### Einen kurzen Plan aufpolieren oder überarbeiten {#polish-a-brief-or-revise-a-plan}

Die Qualifikation identifiziert den Dokumenttyp anhand seines Inhalts, anstatt sich nur auf den Wortlaut Ihrer Anfrage zu verlassen.

Eine **Kampagnenübersicht** beschreibt normalerweise Ziele, Zielgruppe, Messaging-Strategie, Timeline und Erfolgsmetriken. Ein **Einrichtungsplan** enthält normalerweise Implementierungsdetails wie Smart-Listen-Konfigurationen, Smart-Kampagnen-Flussschritte, Token-Definitionen, E-Mail-Spezifikationen und technische Anforderungen.

Geben Sie das Dokument und die von Ihnen angeforderten Änderungen an. Wenn Sie beispielsweise darum bitten, einen Plan zu polieren, aber eine Kampagnenbeschreibung angeben, behandelt die Kenntnis das Dokument als Zusammenfassung. Wenn Sie einen Einrichtungsplan bereitstellen und eine Zusammenfassung überarbeiten möchten, wird das Dokument als Plan behandelt.

## Integration von Organisationsregeln {#organizational-rules-integration}

Einrichtungsdokumente sollten die Regeln Ihres Unternehmens aus dem Systemkontext einbeziehen.

### Namenskonventionen {#naming-conventions}

- Programme: `{{REGION}}_FY{{YEAR}}_{{QUARTER}}_{{TYPE}}_{{DATE}}_{{NAME}}`
- E-Mails: `{{PROGRAM_NAME}}_{{SEQUENCE}}_{{PURPOSE}}`
- Intelligente Kampagnen: `{{NUMBER}}_{{TRIGGER_OR_BATCH}}_{{ACTION}}`

### Erforderliche Elemente {#required-elements}

- Drei lokale Ordner (01 E-Mails, 02 intelligente Kampagnen, 03 Berichte)
- Vier erforderliche Token (eventDate, eventTime, replyToEmail, senderName)
- Ausschlussfilter (abgemeldet, E-Mail ungültig, Marketing ausgesetzt,)
- E-Mail-Konformität (Abmelde-Link, physische Adresse)

### Prä-Aktivierungs-QA {#pre-activation-qa}

- Validierung des Namensmusters
- Bestätigung der Ordnerstruktur
- Ausschlussfilter-Überprüfung
- Prüfung der Kompatibilitätselemente

## Anwendungsfälle {#use-cases}

**Planen eines Webinar-Programms:** Geben Sie die Ziele des Webinars, die Zielgruppe, den Zeitplan für das Ereignis und die Messaging-Anforderungen an. Im Setup-Plan können die Programmstruktur, E-Mail-Spezifikationen, die Kampagnensequenz, Token und QA-Prüfungen umrissen werden.

**Beispielübersicht erstellen:** Fordern Sie eine Beispielübersicht für einen Kampagnentyp an und passen Sie sie dann mit Ihren Kampagnendetails an, bevor Sie einen Programmplan anfordern.

**Vorhandenen Einrichtungsplan aktualisieren:** Geben Sie den Plan an und geben Sie die Änderungen an, z. B. die Aktualisierung der Zeitleiste, das Hinzufügen eines Kampagnenschritts oder die Überarbeitung der Zielgruppenlogik.

## Nächste Schritte {#next-steps}

Nach Abschluss eines Planungsvorgangs können geeignete Folgeaufforderungen Folgendes umfassen:

- „Diesen Einrichtungsplan überarbeiten“
- „Abruf einer Beispiel-Kampagnenbeschreibung“
- „Erstellen Sie dieses Programm in Marketo&quot; (zum Erstellen eines Programms müssen Sie die Qualifikation [Erstellen von Programmen](/help/marketo/product-docs/coworker-for-marketo/skills/build-programs.md) verwenden).
