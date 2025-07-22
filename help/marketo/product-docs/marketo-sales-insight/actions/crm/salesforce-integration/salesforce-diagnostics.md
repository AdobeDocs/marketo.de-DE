---
description: Salesforce-Diagnose - Marketo-Dokumente - Produktdokumentation
title: Salesforce-Diagnose
exl-id: c449f938-9615-47cb-b232-613ec29068a3
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '1344'
ht-degree: 1%

---

# [!DNL Salesforce] {#salesforce-diagnostics}

Ein Teil unserer [!DNL Salesforce]-Integration umfasst eine [!DNL Salesforce] Diagnoseseite innerhalb der Web-Anwendung. Auf dieser Seite werden Fehler aus der fehlgeschlagenen Datenprotokollierung in [!DNL Salesforce] erfasst. Die Fehler können hilfreich sein, sind aber nicht immer lesbar. Daher haben wir eine Kurzdarstellung zusammengestellt, die die Fehlermeldungen erklärt.

## Zugriff auf die Diagnose {#access-diagnostics}

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **[!UICONTROL Einstellungen]** aus.

   ![](assets/salesforce-diagnostics-1.png)

1. Klicken [!UICONTROL  unter „Integrationen] auf **[!UICONTROL Diagnose]**.

   ![](assets/salesforce-diagnostics-2.png)

## Fehlerkorrektur - Schnellübersicht {#error-cheat-sheet}

**error:** API_CURRENTLY_DISABLED\
**category:** access/validation\
**Nachricht:** API ist für diesen Benutzer deaktiviert\
**Was passiert:** Benutzer hat keinen API-Zugriff\
**Schritte zur Fehlerbehebung:** muss [!DNL Salesforce] Administrator der Benutzer-API Zugriff gewähren.

**ERROR:** AUTHENTICATION_FAILURE\
**Kategorie:** Authentifizierung\
**Nachricht:** invalid_grant: Authentifizierungsfehler\
**Was passiert:** Authentifizierung fehlgeschlagen\
**Schritte zur Fehlerbehebung:** Trennen Sie die Verbindung zu [!DNL Salesforce] und stellen Sie dann die Verbindung wieder her.

**ERROR:** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**category:** access/validation\
**Message:** {„errorCode“:„INVALID_SESSION_ID“,„message“:„Sitzung abgelaufen oder ungültig“}\
**Was passiert:**

&#x200B;1. Trigger-Code verursacht, dass die Aktualisierung fehlschlägt.\
2 - Der Benutzer hat keine Schreibberechtigungen auf Objektebene für das angegebene Objekt.

**Schritte zur Fehlerbehebung:**

&#x200B;1. Überprüfen Sie den fehlgeschlagenen Trigger.\
2 - Gewähren Sie dem Benutzer Schreibzugriff für das Objekt ODER deaktivieren Sie die Funktion, die versucht, in das Objekt zu schreiben.

**ERROR:** CANNOT_UPDATE_CONVERTED_LEAD\
**Kategorie:** andere\
**Nachricht:** kann nicht auf konvertierten Lead verweisen\
**Was passiert:** Wir versuchen, uns während der Protokollierung der letzten Aktivität für Kontakte und Leads bei einem konvertierten Lead anzumelden. Ich sah auch einige von diesen für Stellplätze.\
**Schritte zur Fehlerbehebung:** Bitte melden Sie etwaige Vorfälle hiervon unserem [Supportteam](https://nation.marketo.com/t5/Support/ct-p/Support).

**error:** ENTITY_IS_LOCKED\
**category:** access/validation\
**Nachricht:** Die Entität ist für die Bearbeitung gesperrt.\
**Was passiert:** Der Datensatz befindet sich in einem Genehmigungsprozess, bei dem er für alle weiteren Bearbeitungen gesperrt wird, bis er von einer Person, die Inhaber der Genehmigung ist, genehmigt oder abgelehnt wird.\
**Schritte zur Fehlerbehebung:** Siehe oben.

**ERROR:** EXPIRED_ACCESS
**Kategorie:** Authentifizierung
**Nachricht:** invalid_grant: abgelaufenes Zugriffs-/Aktualisierungstoken
**Was passiert:** Das Zugriffs- oder Aktualisierungstoken ist abgelaufen. Token laufen basierend auf [Sitzungseinstellungen in [!DNL Salesforce]](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via) ab.
**Schritte zur Fehlerbehebung:** Sie müssen sich erneut authentifizieren. Trennen Sie die [!DNL Salesforce] und stellen Sie die Verbindung wieder her.

**ERROR:** FAILED_WRITE\
**Kategorie:** intermittierend\
**Nachricht:** Ende der Datei erreicht\
**Was passiert:** Leistungsproblem mit [!DNL Salesforce], wahrscheinlich aufgrund suboptimaler Trigger auf Kundenseite.\
**Schritte zur Fehlerbehebung:** Die Logik „Erneut versuchen“ sollte dies beheben. Wenn es immer noch nicht funktioniert, wenden Sie sich an Ihren [!DNL Salesforce], um einen problematischen Trigger zu beheben.

**ERROR:** FIELD_CUSTOM_VALIDATION_EXCEPTION
**category:** access/validation
**Nachricht:** variiert von Kunde zu Kunde.
**Was passiert:** einer benutzerdefinierten Validierungsregel für das Objekt.
**Schritte zur Fehlerbehebung:** Überprüfen Sie die benutzerdefinierte Validierungsregel, die diesen Fehler verursacht. Da es sich um eine benutzerdefinierte Regel handelt, muss der Fehler nur einmal behandelt werden.

**ERROR:** FIELD_FILTER_VALIDATION_EXCEPTION\
**category:** access/validation\
**Nachricht:** Wert ist nicht vorhanden oder entspricht nicht den Filterkriterien\
**Was passiert:** vorhandenen fehlerhaften Daten in [!DNL Salesforce] werden bei der Aktualisierung erzwungen.\
**Schritte zur Fehlerbehebung:** Siehe oben.

**ERROR:** FIELD_INTEGRITY_EXCEPTION\
**category:** access/validation\
**Nachricht:** Das vorhandene Land/Gebiet erkennt den Wert des Bundeslandes für das Feld: Bundesland/Provinz-Code nicht.\
**Was passiert:** vorhandenen fehlerhaften Daten in [!DNL Salesforce] werden bei der Aktualisierung erzwungen.\
**Schritte zur Fehlerbehebung:** Siehe oben.

**ERROR:** INACTIVE_ORGANIZATION\
**Kategorie:** Authentifizierung\
**Nachricht:** invalid_grant: inaktive Organisation\
**Was passiert:** Ihre [!DNL Salesforce] Organisation ist nicht mehr aktiv.
**Schritte zur Fehlerbehebung:** Trennen Sie die Verbindung und stellen Sie sie erneut [!DNL Salesforce].

**ERROR:** INACTIVE_USER
**Kategorie:** Authentifizierung
**Nachricht:** invalid_grant: inaktiver Benutzer
**Was passiert:** Der [!DNL Salesforce] ist nicht mehr aktiv.
**Schritte zur Fehlerbehebung:** Trennen Sie die Verbindung und stellen Sie sie erneut [!DNL Salesforce].

**ERROR:** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**Kategorie:** intermittierend\
**Nachricht:** (keine zusätzliche Nachricht)\
**Was passiert:** [!DNL Salesforce] Instanz befindet sich im Wartungsmodus.\
**Schritte zur Fehlerbehebung:** Warten Sie, bis die Systemwartung abgeschlossen ist, und wiederholen Sie dann die Protokollierung.

**ERROR:** INSUFFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY
**category:** access/validation
**Nachricht:** Zugriffsrechte für Objekt-ID nicht ausreichend
**Was passiert:** Zugriff auf den übergeordneten Datensatz für eine Aufgabe.
**Schritte zur Fehlerbehebung:** Siehe oben.

**ERROR:** INSUFFICIENT_ACCESS_OR_READONLY\
**category:** access/validation
**Nachricht:** Zugriffsrechte für Objekt-ID nicht ausreichend
**Was passiert:** Die letzte Aktivitätsprotokollierung kann den spezifischen Datensatz nicht bearbeiten, da der Benutzer keinen Schreibzugriff hat.\
**Schritte zur Fehlerbehebung:** Gewähren Sie dem Benutzer Zugriff in [!DNL Salesforce] ODER deaktivieren Sie die Protokollierung der letzten Aktivität für dieses Objekt für diesen Benutzer.

**ERROR:** INVALID_FIELD\
**Kategorie:** intermittierend\
**message:** net::ReadTimeout\
**Was passiert:** Anfrage überschreitet die Zeit. Dies ist wahrscheinlich das Ergebnis zu vieler langsamer Transaktionen.\
**Schritte zur Fehlerbehebung:** Überprüfen Sie die vorhandenen Anpassungen auf mögliche Ursachen für die Latenzprobleme und/oder deaktivieren Sie die Protokollierung der letzten Aktivität für ein oder alle Objekte, um die Last zu reduzieren.

**ERROR:** INVALID_FIELD_FOR_INSERT_UPDATE\
**category:** access/validation\
**Nachricht:** Felder können nicht erstellt/aktualisiert werden: MSE_Replied__c. Überprüfen Sie die Sicherheitseinstellungen dieses Feldes.
**Was passiert:** Benutzer haben keinen Schreibzugriff auf die benutzerdefinierten Felder für die Insight-Verkaufsaktionen, die zum Ausführen der letzten Aktivitätsprotokollierungstransaktion erforderlich sind. Team hat möglicherweise das Paket installiert, aber nicht die richtigen Felder für die Benutzer aktiviert.\
**Schritte zur Fehlerbehebung:** muss [!DNL Salesforce] Admin Zugriff auf die benutzerdefinierten Felder gewähren ODER die Protokollierung der letzten Aktivität deaktivieren.

**ERROR:** INVALID_GRANT\
**Kategorie:** Authentifizierung\
**Nachricht:** invalid_grant: IP eingeschränkt\
**Was passiert:** Wir versuchen auf Ihre [!DNL Salesforce] zuzugreifen, aber Sie haben IP-Einschränkungen, die uns davon abhalten.\
auf die Zulassungsliste setzen **Schritte zur Fehlerbehebung:** Ihr [!DNL Salesforce]-Administrator muss unsere IPs ändern. Benutzer sollten sich an den Support wenden, um die IP-Adressen zu erhalten.

**ERROR:** INVALID_TYPE\
**category:** access/validation\
**Nachricht:** Erstellungsdatum, (SELECT ID FROM Tasks) VOM Lead WO E-Mail=&#39;emailid&#39;^FEHLER beim `Row:1:Column:53sObject` &#39;Lead&#39; nicht unterstützt wird. Wenn Sie versuchen, ein benutzerdefiniertes Objekt zu verwenden, stellen Sie sicher, dass hinter dem Namen der Entität das Zeichen &#39;__c&#39; angehängt wird. Bitte die WSDL referenzieren oder den Aufruf für die entsprechenden Namen beschreiben
**Was passiert:** Wir versuchen, einen Objekttyp aus Salesforce abzufragen, auf den der Benutzer keinen Zugriff hat. Dies hängt höchstwahrscheinlich damit zusammen, dass der Benutzer nicht den richtigen Zugriff auf das Lead-Objekt hat.\
**Schritte zur Fehlerbehebung:** Gewähren Sie Lese- und Aktualisierungszugriff auf das Lead-Objekt in Salesforce oder deaktivieren Sie die E-Mail-Protokollierung und die Protokollierung der letzten Aktivitäten, um Lead-Datensätze zu ermitteln.

**ERROR:** QUERY_TIMEOUT\
**Kategorie:** intermittierend\
**Nachricht:** Ihre Abfrageanfrage wurde zu lange ausgeführt\
**Was geschieht:** Siehe oben.\
**Schritte zur Fehlerbehebung:** Die Logik „Erneut versuchen“ sollte dies beheben. Wenn es immer noch nicht funktioniert, wenden Sie sich an Ihren [!DNL Salesforce], um einen problematischen Trigger zu beheben.

**ERROR:** REQUEST_LIMIT_EXCEEDED\
**Kategorie:** intermittierend\
**message:**
1 - ConcurrentPerOrgLongTxn-Limit überschritten\
&#x200B;2. Gesamtzahl der Anfragen überschritten\
&#x200B;3. ConcurrentRequest\
**Was passiert:**
1 - Das Limit für gleichzeitige Anfragen wurde überschritten, wahrscheinlich aufgrund eines ineffizienten Trigger-Codes.\
2 - Zu viele Integrationen führen dazu, dass die Organisation das 24-Stunden-Rollierfenster hinter sich lässt.\
**Schritte zur Fehlerbehebung:**
1. Überprüfen Sie die vorhandenen Trigger der betroffenen Objekte. Deaktivieren Sie möglicherweise die Rollup-Protokollierung für ein oder mehrere Objekte.\
&#x200B;2. Kaufen Sie weitere API-Aufrufe von [!DNL Salesforce]. Deaktivieren Sie möglicherweise die Rollup-Protokollierung für ein oder mehrere Objekte.

**ERROR:** REQUIRED_FIELD_MISSING\
**category:** access/validation\
**Nachricht:** Erforderliche Felder fehlen: `[Amount_Committed_Private_Capital__c]`
**Was passiert:** Dies geschieht im Allgemeinen für die Protokollierung der letzten Aktivitäten. Benutzerdefinierte Felder wurden so eingerichtet, dass sie erforderlich sind, aber leere Werte enthalten. Dies kann vorkommen, wenn der Datensatz mit einem leeren Wert des benutzerdefinierten Felds erstellt und dann zu einem Pflichtfeld gemacht wurde. Erforderlichkeit wird erzwungen, wenn wir versuchen, den Datensatz zu aktualisieren, obwohl wir das benutzerdefinierte Feld nicht berühren.\
**Schritte zur Fehlerbehebung:** Aktualisieren Sie die Werte der fehlenden Felder manuell. Sie können die Nachricht dann über die Insight-Aktionen für den Vertrieb erneut senden.

**ERROR:** SERVER_UNAVAILABLE\
**Kategorie:** intermittierend\
**Nachricht:** Server ist ausgelastet\
**Was passiert:** Leistungsproblem mit [!DNL Salesforce], wahrscheinlich aufgrund suboptimaler Trigger durch den Kunden\
**Schritte zur Fehlerbehebung:** Die Logik „Erneut versuchen“ sollte dies beheben. Wenn es immer noch nicht funktioniert, wenden Sie sich an Ihren [!DNL Salesforce], um einen problematischen Trigger zu beheben.

**ERROR:** TXN_SECURITY_NO_ACCESS\
**category:** access/validation\
**Nachricht:** Der angeforderte Vorgang ist aufgrund einer Sicherheitsrichtlinie in Ihrer Organisation nicht zulässig. Wenden Sie sich an Ihren Administrator.
**Was passiert:** Eine Art von Sicherheitsbeschränkung wurde eingerichtet - siehe https://developer.salesforce.com/forums/?id=„record ID“\
**Schritte zur Fehlerbehebung:** Sprechen Sie mit Ihrem [!DNL Salesforce] Admin und sehen Sie sich an, was die spezifische Einschränkung sein könnte.

**ERROR:** UNABLE_TO_LOCK_ROW\
**Kategorie:** intermittierend\
**Nachricht:** kann keinen exklusiven Zugriff auf diesen Datensatz oder 1 Datensatz erhalten: „Datensatz-ID“\
**Was passiert:** Wahrscheinlich gibt es einen Trigger, der mehrere Versuche verursacht, auf denselben Datensatz zuzugreifen, möglicherweise im Fall einer Gruppen-E-Mail.\
**Schritte zur Fehlerbehebung:** Die Logik „Erneut versuchen“ sollte dies beheben. Wenn es immer noch nicht funktioniert, wenden Sie sich an Ihren [!DNL Salesforce], um einen problematischen Trigger zu beheben.

**ERROR:** UNKNOWN_EXCEPTION
**Kategorie:** andere\
**Nachricht:** unbekannte Ausnahme aufgetreten\
**Was passiert:** Ausnahmefehler in [!DNL Salesforce].\
**Schritte zur Fehlerbehebung:** Sie einen Fall bei [!DNL Salesforce] ein und kopieren Sie die numerischen Werte in der Fehlermeldung. Dies ist [!DNL Salesforce] Code, der einen Fehler nicht ordnungsgemäß behandelt.
