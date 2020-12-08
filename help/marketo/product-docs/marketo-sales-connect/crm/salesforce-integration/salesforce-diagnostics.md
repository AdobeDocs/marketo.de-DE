---
unique-page-id: 14745730
description: Salesforce-Diagnose - Marketing Docs - Produktdokumentation
title: Salesforce-Diagnose
translation-type: tm+mt
source-git-commit: 44ed91b485b52173922c709de63a4353e16c5072
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---


# Salesforce-Diagnose {#salesforce-diagnostics}

Teil unserer Salesforce-Integration ist eine Salesforce-Diagnoseseite innerhalb der Webanwendung. Diese Seite erfasst Fehler bei der fehlgeschlagenen Datenprotokollierung in Salesforce. Die Fehler können hilfreich sein, sind aber nicht immer lesbar. Als solche haben wir eine Betrügerei zusammengestellt, die hilft, die Fehlermeldungen zu erklären.

**Fehler:** API_CURRENTLY_DEABLED\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** API für diesen Benutzer deaktiviert\
**Was geschieht:** Benutzer hat keinen API-Zugriff\
**Schritte zur Fehlerbehebung:** Salesforce Admin muss dem Benutzer-API-Zugriff gewähren.

<br> 

**Fehler:** AUTHENTICATION_FAILURE\
**Kategorie:** Authentifizierung\
**Nachricht:** Invalid_grant: Authentifizierungsfehler\
**Was geschieht:** Authentifizierung fehlgeschlagen\
**Schritte zur Fehlerbehebung:** Trennen Sie die Verbindung zu Salesforce und stellen Sie dann die Verbindung wieder her.

<br> 

**Fehler:** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;Sitzung abgelaufen oder ungültig&quot;}\
**Was geschieht:**

1 - Der Auslösercode verursacht einen Fehler bei der Aktualisierung.\
2 - Der Benutzer verfügt über keine Schreibberechtigung auf Objektebene für das angegebene Objekt.

**Schritte zur Fehlerbehebung:**

1 - Überprüfungsauslöser, der fehlschlägt.\
2 - Gewähren Sie dem Benutzer Schreibzugriff für das Objekt ODER deaktivieren Sie die Funktion, die versucht, in das Objekt zu schreiben.

<br> 

**Fehler:** CANNOT_UPDATE_CONVERTED_LEAD\
**Kategorie:** Sonstiges\
**Nachricht:** kann nicht auf konvertierten Interessenten verweisen\
**Was geschieht:** Wir versuchen, uns während der Protokollierung der neuesten Aktivitäten für Kontakte und Interessenten bei einem umgerechneten Interessenten anzumelden. Auch ein paar davon für Pitches gesehen.\
**Schritte zur Fehlerbehebung:** Bitte melden Sie diese Fälle unserem [Supportteam](http://nation.marketo.com/community/support_solutions).

<br> 

**Fehler:** ENTITY_IS_LOCKED\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** die Entität zur Bearbeitung gesperrt ist\
**Was geschieht:** Der Datensatz befindet sich in einem Genehmigungsprozess, bei dem er vor weiteren Änderungen gesperrt wird, bis er entweder von einer Person genehmigt oder verweigert wird, die Eigentümer der Genehmigung ist.\
**Schritte zur Fehlerbehebung:** Siehe oben.

<br> 

**Fehler:** EXPIRED_ACCESS **-Kategorie:** Authentifizierungsmeldung **:** Invalid_grant: Token **für abgelaufenen Zugriff/AktualisierungWas geschieht:** Das Zugriffs- oder Aktualisierungstoken ist abgelaufen. Tokens laufen je nach [Sitzungseinstellungen in Salesforce](http://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via)ab.
**Schritte zur Fehlerbehebung:** Sie müssen sich erneut authentifizieren. Trennen Sie die Salesforce-Verbindung und stellen Sie eine erneute Verbindung her.

<br> 

**Fehler:** FAILED_WRITE\
**Kategorie:** intermittierend\
**Nachricht:** Dateiende erreicht\
**Was geschieht:** Leistungsproblem bei Salesforce, wahrscheinlich aufgrund der suboptimalen Auslöser auf Kundenseite.\
**Schritte zur Fehlerbehebung:** Die Logik des Wiederholens sollte damit umgehen. Falls dies weiterhin nicht funktioniert, sollten Sie mit Ihrem Salesforce-Administrator zusammenarbeiten, um einen problematischen Auslöser zu beheben.

<br> 

**Fehler:** FIELD_CUSTOM_VALIDATION_EXCEPTION **-Kategorie:** Zugriffs-/Überprüfungsmeldung **:** Je nach Kunde unterschiedlich.
**Was geschieht:** Fehlschlagen einer benutzerdefinierten Validierungsregel für das Objekt.
**Schritte zur Fehlerbehebung:** Überprüfen Sie die benutzerspezifische Validierungsregel, die diesen Fehler verursacht. Da es sich um eine benutzerspezifische Regel handelt, muss der Fehler einmalig behandelt werden.

<br> 

**Fehler:** FIELD_FILTER_VALIDATION_EXCEPTION\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** Wert ist nicht vorhanden oder entspricht nicht den Filterkriterien\
**Was geschieht:** Bestehende fehlerhafte Daten in Salesforce werden bei der Aktualisierung erzwungen.\
**Schritte zur Fehlerbehebung:** Siehe oben.

<br> 

**Fehler:** FIELD_INTEGRITY_EXCEPTION\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** Das bestehende Land/Gebiet erkennt den Landeswert für Feld nicht an: Bundesland-/Kantonscode\
**Was geschieht:** Bestehende fehlerhafte Daten in Salesforce werden bei der Aktualisierung erzwungen.\
**Schritte zur Fehlerbehebung:** Siehe oben.

<br> 

**Fehler:** INACTIVE_ORGANISATION\
**Kategorie:** Authentifizierung\
**Nachricht:** Invalid_grant: inaktive Organisation\
**Was geschieht:** Ihre Salesforce-Organisation ist nicht mehr aktiv.\
**Schritte zur Fehlerbehebung:** Trennen Sie dann die Verbindung wieder von Salesforce.

**Fehler:** INACTIVE_USER **-Kategorie:** Authentifizierungsmeldung **:** Invalid_grant: Inaktiver Benutzer **Was passiert:** Der Salesforce-Benutzer ist nicht mehr aktiv **:** Trennen Sie dann die Verbindung wieder von Salesforce.

**Fehler:** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**Kategorie:** intermittierend\
**Nachricht:** (keine zusätzliche Meldung)\
**Was geschieht:** Die Salesforce-Instanz befindet sich im Wartungsmodus.\
**Schritte zur Fehlerbehebung:** Warten Sie, bis die Systemwartung abgeschlossen ist, und versuchen Sie es erneut.

**Fehler:** INSUFFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY **-Kategorie:** Zugriffs-/Überprüfungsmeldung **:** Unzureichende Zugriffsrechte für die Objekt-ID **Was geschieht?** Kein Zugriff auf den übergeordneten Datensatz für eine Aufgabe.
**Schritte zur Fehlerbehebung:** Siehe oben.

<br> 

**Fehler:** INSUFFICIENT_ACCESS_OR_READONLY\
**Kategorie:** Zugriff/Validierung** ****Meldung:** Unzureichende Zugriffsrechte auf Objekt-ID******Was geschieht?** Die Protokollierung der letzten Aktivität kann den spezifischen Datensatz nicht bearbeiten, da der Benutzer keinen Schreibzugriff hat.\
**Schritte zur Fehlerbehebung:** Gewähren Sie dem Benutzer Zugriff in Salesforce ODER deaktivieren Sie die Protokollierung der letzten Aktivität für dieses Objekt.

**Fehler:** INVALID_FIELD\
**Kategorie:** intermittierend\
**Nachricht:** Net::ReadTimeout\
**Was geschieht:** Bei der Anforderung wird der Zeitrahmen überschritten. Dies ist wahrscheinlich auf zu viele langsame Transaktionen zurückzuführen.\
**Schritte zur Fehlerbehebung:** Prüfen Sie vorhandene Anpassungen auf mögliche Ursachen für Latenzprobleme und/oder deaktivieren Sie die Protokollierung der neuesten Aktivität für eines oder alle Objekte, um die Belastung zu reduzieren.

**Fehler:** INVALID_FIELD_FOR_INSERT_UPDATE\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** Felder können nicht erstellt/aktualisiert werden: ToutApp__Tout_Last_Replied__c. Bitte überprüfen Sie die Sicherheitseinstellungen dieses Feldes.\
**Was geschieht:** Benutzer haben keinen Schreibzugriff auf die benutzerdefinierten Tout-Felder, die zur Durchführung der Protokollierungsaktion &quot;Zuletzt verwendete Aktivität&quot;erforderlich sind. Team hat möglicherweise das Paket installiert, hat aber nicht die korrekten Felder für die Benutzer aktiviert.\
**Schritte zur Fehlerbehebung:** Salesforce-Administrator muss Zugriff auf die benutzerdefinierten Felder gewähren ODER die Protokollierung der letzten Aktivität deaktivieren.

**Fehler:** INVALID_GRANT\
**Kategorie:** Authentifizierung\
**Nachricht:** Invalid_grant: IP eingeschränkt\
**Was geschieht:** Wir versuchen, auf Ihre Salesforce zuzugreifen, aber Sie haben IP-Beschränkungen, die uns daran hindern, dies zu tun.\
**Schritte zur Fehlerbehebung:** Ihr Salesforce-Administrator muss unsere IPs in Zulassungsliste setzen. Die Benutzer sollten sich an den Support wenden, um die IP-Adressen zu erhalten.

**Fehler:** INVALID_TYPE\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** CreatedDate, (SELECT Id From Aufgaben) from Lead WO Email=&#39;emailid&#39;^ERROR at Row:1:Column:53sObjekttyp &#39;Lead&#39; wird nicht unterstützt. Wenn Sie versuchen, ein benutzerdefiniertes Objekt zu verwenden, hängen Sie &quot;__c&quot;nach dem Entitätsnamen an. Bitte verweisen Sie auf Ihre WSDL oder auf die Beschreibung des Aufrufs für die entsprechenden Namen\
**Was geschieht:** Wir versuchen, einen Objekttyp von Salesforce Abfrage, auf den der Benutzer keinen Zugriff hat. Dies ist höchstwahrscheinlich darauf zurückzuführen, dass der Benutzer keinen Zugriff auf das Interessentenobjekt hat.\
**Schritte zur Fehlerbehebung:** Erteilen Sie entweder Lese- und Aktualisierungszugriff auf das Lead-Objekt in Salesforce oder deaktivieren Sie die E-Mail-Protokollierung und die Protokollierung der neuesten Aktivität für Interessentendatensätze.

**Fehler:** ABFRAGE_TIMEOUT\
**Kategorie:** intermittierend\
**Nachricht:** Ihre Abfrage-Anforderung wurde zu lange ausgeführt\
**Was geschieht:** Siehe oben.\
**Schritte zur Fehlerbehebung:** Die Logik des Wiederholens sollte damit umgehen. Falls dies weiterhin nicht funktioniert, sollten Sie mit Ihrem Salesforce-Administrator zusammenarbeiten, um einen problematischen Auslöser zu beheben.

**Fehler:** REQUEST_LIMIT_EXCEEDED\
**Kategorie:** intermittierend\
**Nachricht:**
1 - ConcurrentPerOrgLongTxn-Grenzwert überschritten\
2 - Maximale Anzahl der Anfragen überschritten\
3 - ConcurrentRequest\
**Was geschieht:**
1 - Limit für gleichzeitige Anfragen wurde überschritten, was wahrscheinlich auf ineffizienten Auslösercode zurückzuführen ist.\
2 - Zu viele Integrationen haben die Organisation über das 24-Stunden-Rollierungsfenster hinaus gebracht.\
**Schritte zur Fehlerbehebung:**
1 - Prüfen Sie vorhandene Auslöser für die betroffenen Objekte. Die Rollup-Protokollierung für ein oder mehrere Objekte kann deaktiviert werden.\
2 - Kaufen Sie weitere API-Aufrufe von Salesforce. Die Rollup-Protokollierung für ein oder mehrere Objekte kann deaktiviert werden.

**Fehler:** REQUIRED_FIELD_MISSING\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** Die erforderlichen Felder fehlen: [Amount_Committed_Private_Capital_c]\
**Was geschieht:** Dies geschieht im Allgemeinen bei der Protokollierung der neuesten Aktivität. Benutzerdefinierte Felder wurden so eingerichtet, dass sie erforderlich sind, jedoch leere Werte enthalten. Dies kann vorkommen, wenn der Datensatz mit einem leeren Wert des benutzerdefinierten Felds erstellt und dann als erforderlich festgelegt wurde. Die Anforderung wird erzwungen, wenn wir versuchen, den Datensatz zu aktualisieren, auch wenn wir das benutzerdefinierte Feld nicht berühren.\
**Schritte zur Fehlerbehebung:** Aktualisieren Sie manuell die Werte der fehlenden Felder. Sie können die Nachricht dann von ToutApp erneut ausprobieren.

**Fehler:** SERVER_UNAVAILABLE\
**Kategorie:** intermittierend\
**Nachricht:** Server zu stark\
**Was geschieht:** Leistungsproblem mit Salesforce, wahrscheinlich aufgrund der suboptimalen Auslöser durch den Kunden\
**Schritte zur Fehlerbehebung:** Die Logik des Wiederholens sollte damit umgehen. Wenn es immer noch nicht funktioniert, sollten Sie mit Ihrem Salesforce-Administrator zusammenarbeiten, um Probleme beim Erstellen eines problematischen Auslösers zu vermeiden.

**Fehler:** TXN_SECURITY_NO_ACCESS\
**Kategorie:** Zugriff/Validierung\
**Nachricht:** Der angeforderte Vorgang ist aufgrund einer Sicherheitsrichtlinie in Ihrem Unternehmen nicht zulässig. Wenden Sie sich an Ihren Administrator.\
**Was geschieht:** Es wurde eine Art Sicherheitsbeschränkung eingerichtet - siehe `https://developer.salesforce.com/forums/?id="record` ID&quot;\
**Schritte zur Fehlerbehebung:** Sprechen Sie mit Ihrem Salesforce-Administrator und sehen Sie, welche spezifischen Einschränkungen möglicherweise bestehen.

**Fehler:** UNABLE_TO_LOCK_ROW\
**Kategorie:** intermittierend\
**Nachricht:** keinen ausschließlichen Zugriff auf diesen Datensatz oder 1 Datensatz erhalten: &quot;record ID&quot;\
**Was geschieht:** Wahrscheinlich gibt es einen Auslöser, der mehrere Versuche auslöst, auf denselben Datensatz zuzugreifen, möglicherweise im Falle einer Gruppen-E-Mail.\
**Schritte zur Fehlerbehebung:** Die Logik des Wiederholens sollte damit umgehen. Falls dies weiterhin nicht funktioniert, sollten Sie mit Ihrem Salesforce-Administrator zusammenarbeiten, um einen problematischen Auslöser zu beheben.

**Fehler:** UNKNOWN_EXCEPTION\
**Kategorie:** Sonstiges\
**Nachricht:** Unbekannte Ausnahme aufgetreten\
**Was geschieht:** Unbehandelte Ausnahme in Salesforce.\
**Schritte zur Fehlerbehebung:** Geben Sie eine Groß-/Kleinschreibung mit Salesforce ein und kopieren Sie die numerischen Werte in der Fehlermeldung. Dies ist Salesforce-Code, der einen Fehler nicht ordnungsgemäß behandelt.
