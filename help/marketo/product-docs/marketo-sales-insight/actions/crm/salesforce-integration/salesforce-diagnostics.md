---
description: Salesforce Diagnostics - Marketo Docs - Produktdokumentation
title: Salesforce-Diagnose
exl-id: c449f938-9615-47cb-b232-613ec29068a3
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '1445'
ht-degree: 1%

---

# Salesforce-Diagnose {#salesforce-diagnostics}

Teil unserer Salesforce-Integration ist eine Salesforce-Diagnoseseite innerhalb der Webanwendung. Auf dieser Seite werden Fehler aus der fehlgeschlagenen Datenprotokollierung in Salesforce erfasst. Die Fehler können hilfreich sein, sind aber nicht immer lesbar. Daher erstellen wir ein Datenblatt, das die Fehlermeldungen erklärt.

## Access Diagnostics {#access-diagnostics}

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **Einstellungen**.

   ![](assets/salesforce-diagnostics-1.png)

1. Klicken Sie unter Integrationen auf **Diagnose**.

   ![](assets/salesforce-diagnostics-2.png)

## Fehlermeldungsblatt {#error-cheat-sheet}

**Fehler:** API_CURRENTLY_DISABLED\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** Die API ist für diesen Benutzer deaktiviert\
**Was geschieht:** Benutzer hat keinen API-Zugriff\
**Schritte zur Fehlerbehebung:** Salesforce Admin muss dem Benutzer-API-Zugriff gewähren.

**Fehler:** AUTHENTICATION_FAILURE\
**Kategorie:** Authentifizierung\
**Nachricht:** invalid_grant: Authentifizierungsfehler\
**Was geschieht:** Authentifizierung fehlgeschlagen\
**Schritte zur Fehlerbehebung:** Trennen Sie Salesforce und verbinden Sie sich dann erneut.

**Fehler:** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;Sitzung abgelaufen oder ungültig&quot;}\
**Was geschieht:**

1 - Trigger-Code führt dazu, dass die Aktualisierung fehlschlägt.\
2 - Benutzer verfügt nicht über Schreibberechtigungen auf Objektebene für das angegebene Objekt.

**Schritte zur Fehlerbehebung:**

1 - Trigger überprüfen, der fehlschlägt.\
2 - Erteilen Sie dem Benutzer entweder Schreibzugriff für das Objekt ODER deaktivieren Sie die Funktion, die versucht, in das Objekt zu schreiben.

**Fehler:** CANNOT_UPDATE_CONVERTED_LEAD\
**Kategorie:** Sonstiges\
**Nachricht:** kann nicht auf konvertierten Lead verweisen\
**Was geschieht:** Wir versuchen, uns während der Protokollierung der letzten Aktivitäten für Kontakte und Leads bei einem konvertierten Lead zu anmelden. Auch ein paar von diesen für Felsen gesehen.\
**Schritte zur Fehlerbehebung:** Bitte melden Sie alle Fälle von diesem an unsere [Supportteam](https://nation.marketo.com/t5/Support/ct-p/Support).

**Fehler:** ENTITY_IS_LOCKED\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** die Entität für die Bearbeitung gesperrt ist\
**Was geschieht:** Der Datensatz befindet sich in einem Genehmigungsprozess, bei dem er vor weiteren Bearbeitungen gesperrt wird, bis er von einer Person genehmigt oder abgelehnt wird, die Eigentümer der Genehmigung ist.\
**Schritte zur Fehlerbehebung:** Siehe oben.

**Fehler:** EXPIRED_ACCESS
**Kategorie:** Authentifizierung
**Nachricht:** invalid_grant: abgelaufenes Zugriffs-/Aktualisierungstoken
**Was geschieht:** Das Zugriffs- oder Aktualisierungstoken ist abgelaufen. Token laufen basierend auf ab [Sitzungseinstellungen in Salesforce](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Schritte zur Fehlerbehebung:** Sie müssen sich erneut authentifizieren. Trennen Sie die Salesforce-Verbindung und stellen Sie eine erneute Verbindung her.

**Fehler:** FAILED_WRITE\
**Kategorie:** Gelegentlich\
**Nachricht:** Dateiende erreicht\
**Was geschieht:** Leistungsproblem mit Salesforce, wahrscheinlich aufgrund suboptimaler Trigger auf Kundenseite.\
**Schritte zur Fehlerbehebung:** Wiederholungslogik sollte dies handhaben. Wenn es immer noch nicht funktioniert, wenden Sie sich an Ihren Salesforce-Administrator, um einen problematischen Trigger zu beheben.

**Fehler:** FIELD_CUSTOM_VALIDATION_EXCEPTION
**Kategorie:** Zugriff/Validierung
**Nachricht:** Je nach Kunde variiert.
**Was geschieht:** Fehlschlagen einer benutzerdefinierten Validierungsregel für das Objekt.
**Schritte zur Fehlerbehebung:** Überprüfen Sie die benutzerdefinierte Validierungsregel, die diesen Fehler verursacht. Da es sich hierbei um eine benutzerspezifische Regel handelt, muss der Fehler nur einmal behandelt werden.

**Fehler:** FIELD_FILTER_VALIDATION_EXCEPTION\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** Wert ist nicht vorhanden oder entspricht nicht den Filterkriterien\
**Was geschieht:** Vorhandene fehlerhafte Daten in Salesforce werden bei der Aktualisierung erzwungen.\
**Schritte zur Fehlerbehebung:** Siehe oben.

**Fehler:** FIELD_INTEGRITY_EXCEPTION\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** Das bestehende Land/Gebiet erkennt den Landeswert für das Feld nicht an: Code für Bundesland/Provinz\
**Was geschieht:** Vorhandene fehlerhafte Daten in Salesforce werden bei der Aktualisierung erzwungen.\
**Schritte zur Fehlerbehebung:** Siehe oben.

**Fehler:** INACTIVE_ORGANIZATION\
**Kategorie:** Authentifizierung\
**Nachricht:** invalid_grant: inaktive Organisation\
**Was geschieht:** Ihre Salesforce-Organisation ist nicht mehr aktiv.
**Schritte zur Fehlerbehebung:** Trennen Sie dann die Verbindung von Salesforce.

**Fehler:** INACTIVE_USER
**Kategorie:** Authentifizierung
**Nachricht:** invalid_grant: inaktiver Benutzer
**Was geschieht:** Der Salesforce-Benutzer ist nicht mehr aktiv
**Schritte zur Fehlerbehebung:** Trennen Sie dann die Verbindung von Salesforce.

**Fehler:** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**Kategorie:** Gelegentlich\
**Nachricht:** (keine zusätzliche Nachricht)\
**Was geschieht:** Die Salesforce-Instanz befindet sich im Wartungsmodus.\
**Schritte zur Fehlerbehebung:** Warten Sie, bis die Systemwartung abgeschlossen ist, und versuchen Sie dann erneut die Protokollierung.

**Fehler:** INSUFFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY
**Kategorie:** Zugriff/Validierung
**Nachricht:** unzureichende Zugriffsrechte auf Objekt-ID
**Was geschieht:** Kein Zugriff auf den übergeordneten Datensatz für eine Aufgabe.
**Schritte zur Fehlerbehebung:** Siehe oben.

**Fehler:** INSUFFICIENT_ACCESS_OR_READONLY\
**Kategorie:** Zugriff/Validierung
**Nachricht:** unzureichende Zugriffsrechte auf Objekt-ID
**Was geschieht:** Die Protokollierung der letzten Aktivität kann den spezifischen Datensatz nicht bearbeiten, da der Benutzer keinen Schreibzugriff hat.\
**Schritte zur Fehlerbehebung:** Gewähren Sie dem Benutzer Zugriff in Salesforce ODER deaktivieren Sie die Protokollierung der letzten Aktivität für dieses Objekt für diesen Benutzer.

**Fehler:** INVALID_FIELD\
**Kategorie:** Gelegentlich\
**Nachricht:** Net::ReadTimeout\
**Was geschieht:** Die Anfrage hat eine Zeitüberschreitung. Dies ist wahrscheinlich auf zu viele langsame Transaktionen zurückzuführen.\
**Schritte zur Fehlerbehebung:** Überprüfen Sie vorhandene Anpassungen auf potenzielle Ursachen für Latenzprobleme und/oder deaktivieren Sie die Protokollierung der letzten Aktivität für ein oder alle Objekte, um die Last zu reduzieren.

**Fehler:** INVALID_FIELD_FOR_INSERT_UPDATE\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** Felder können nicht erstellt/aktualisiert werden: MSE_Replied__c. Überprüfen Sie die Sicherheitseinstellungen dieses Felds.
**Was geschieht:** Benutzer haben keinen Schreibzugriff auf die benutzerdefinierten Felder für Sales Insight-Aktionen, die zur Durchführung der Protokollierung der letzten Aktivität erforderlich sind. Team hat möglicherweise das Paket installiert, aber die korrekten Felder für die Benutzer wurden nicht aktiviert.\
**Schritte zur Fehlerbehebung:** Salesforce Admin muss Zugriff auf die benutzerdefinierten Felder gewähren ODER die Protokollierung der letzten Aktivität deaktivieren.

**Fehler:** INVALID_GRANT\
**Kategorie:** Authentifizierung\
**Nachricht:** invalid_grant: ip restricted\
**Was geschieht:** Wir versuchen, auf Ihre Salesforce zuzugreifen, aber Sie haben IP-Einschränkungen, die uns daran hindern, dies zu tun.\
**Schritte zur Fehlerbehebung:** Ihr Salesforce-Administrator muss unsere IPs in Zulassungsliste stellen. Benutzer sollten sich an den Support wenden, um die IP-Adressen zu erhalten.

**Fehler:** INVALID_TYPE\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** CreatedDate, (SELECT ID FROM Tasks) FROM Lead WHERE Email=&#39;emailid&#39;^ERROR at Row:1:Column:53sObject type &#39;Lead&#39; wird nicht unterstützt. Wenn Sie versuchen, ein benutzerdefiniertes Objekt zu verwenden, stellen Sie sicher, dass hinter dem Namen der Entität das Zeichen &#39;__c&#39; angehängt wird. Bitte verweisen Sie auf Ihre WSDL oder auf den Aufruf zur Beschreibung der entsprechenden Namen
**Was geschieht:** Wir versuchen, einen Objekttyp aus Salesforce abzufragen, auf den der Benutzer keinen Zugriff hat. Dies hängt höchstwahrscheinlich damit zusammen, dass der Benutzer keinen Zugriff auf das Lead-Objekt hat.\
**Schritte zur Fehlerbehebung:** Gewähren Sie entweder Lese- und Aktualisierungszugriff auf das Lead-Objekt in Salesforce oder deaktivieren Sie die E-Mail-Protokollierung und die Protokollierung der letzten Aktivität, um Lead-Datensätze zu speichern.

**Fehler:** QUERY_TIMEOUT\
**Kategorie:** Gelegentlich\
**Nachricht:** Ihre Abfrageanforderung wurde zu lange ausgeführt.\
**Was geschieht:** Siehe oben.\
**Schritte zur Fehlerbehebung:** Wiederholungslogik sollte dies handhaben. Wenn es immer noch nicht funktioniert, wenden Sie sich an Ihren Salesforce-Administrator, um einen problematischen Trigger zu beheben.

**Fehler:** ANFRAGE_LIMIT_EXCEEDED\
**Kategorie:** Gelegentlich\
**Nachricht:**
1 - ConcurrentPerOrgLongTxn Limit überschritten\
2 - Maximale Anzahl an Anfragen überschritten\
3 - ConcurrentRequest\
**Was geschieht:**
1 - Grenzwert für gleichzeitige Anforderungen überschritten, was wahrscheinlich auf ineffizienten Trigger-Code zurückzuführen ist.\
2 - Zu viele Integrationen haben die Organisation über das 24-Stunden-rollierende Fenster hinaus geführt.\
**Schritte zur Fehlerbehebung:**
1 - Überprüfen vorhandener Trigger auf die betroffenen Objekte. Die Rollup-Protokollierung für ein oder mehrere Objekte kann potenziell deaktiviert werden.\
2 - Kaufen Sie weitere API-Aufrufe von Salesforce. Die Rollup-Protokollierung für ein oder mehrere Objekte kann potenziell deaktiviert werden.

**Fehler:** REQUIRED_FIELD_MISSING\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** Erforderliche Felder fehlen: `[Amount_Committed_Private_Capital__c]`
**Was geschieht:** Dies geschieht normalerweise bei der Protokollierung der letzten Aktivität. Benutzerdefinierte Felder wurden so eingerichtet, dass sie erforderlich sind, jedoch leere Werte enthalten. Dies kann vorkommen, wenn der Datensatz mit einem leeren Wert des benutzerdefinierten Felds erstellt und dann als erforderlich festgelegt wurde. Die Anforderung wird erzwungen, wenn wir versuchen, den Datensatz zu aktualisieren, auch wenn wir das benutzerdefinierte Feld nicht berühren.\
**Schritte zur Fehlerbehebung:** Aktualisieren Sie die Werte der fehlenden Felder manuell. Sie können die Nachricht dann über &quot;Sales Insight-Aktionen&quot;erneut ausprobieren.

**Fehler:** SERVER_UNAVAILABLE\
**Kategorie:** Gelegentlich\
**Nachricht:** Server zu stark ausgelastet\
**Was geschieht:** Leistungsproblem mit Salesforce, wahrscheinlich aufgrund suboptimaler Trigger durch den Kunden\
**Schritte zur Fehlerbehebung:** Wiederholungslogik sollte dies handhaben. Wenn es immer noch nicht funktioniert, wenden Sie sich an Ihren Salesforce-Administrator, um Probleme beim Erstellen eines problematischen Triggers zu vermeiden.

**Fehler:** TXN_SECURITY_NO_ACCESS\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** Der von Ihnen angeforderte Vorgang ist aufgrund einer Sicherheitsrichtlinie in Ihrem Unternehmen nicht zulässig. Kontaktieren Sie diesbezüglich Ihre oder Ihren Admin.
**Was geschieht:** Es wurde eine Art Sicherheitsbeschränkung eingerichtet - siehe https://developer.salesforce.com/forums/?id=&quot;Datensatz-ID&quot;\
**Schritte zur Fehlerbehebung:** Sprechen Sie mit Ihrem Salesforce-Administrator und sehen Sie, welche spezifische Einschränkung auftreten kann.

**Fehler:** UNABLE_TO_LOCK_ROW\
**Kategorie:** Gelegentlich\
**Nachricht:** kann keinen ausschließlichen Zugriff auf diesen Datensatz oder 1 Datensätze erhalten: &quot;Datensatz-ID&quot;\
**Was geschieht:** Wahrscheinlich gibt es einen Trigger, der mehrere Versuche zum Zugriff auf denselben Datensatz verursacht, möglicherweise im Fall einer Gruppen-E-Mail.\
**Schritte zur Fehlerbehebung:** Wiederholungslogik sollte dies handhaben. Wenn es immer noch nicht funktioniert, wenden Sie sich an Ihren Salesforce-Administrator, um einen problematischen Trigger zu beheben.

**Fehler:** UNKNOWN_EXCEPTION
**Kategorie:** Sonstiges\
**Nachricht:** Unbekannte Ausnahme aufgetreten\
**Was geschieht:** Unbehandelte Ausnahme in Salesforce.\
**Schritte zur Fehlerbehebung:** Geben Sie Salesforce eine Groß-/Kleinschreibung an und kopieren Sie die numerischen Werte in die Fehlermeldung. Dies ist Salesforce-Code, der einen Fehler nicht ordnungsgemäß verarbeitet.
