---
description: Dynamic Chat - Versionshinweise - Marketo-Dokumente - Produktdokumentation
title: Dynamic Chat-Versionshinweise
hide: true
hidefromtoc: true
feature: Release Information, Dynamic Chat
source-git-commit: c2c95f36c710ba7a9ac75c2160c72e44b5f81a99
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 1%

---

# April 2024 - Versionshinweise {#release-notes-apr-24}

Adobe Dynamic Chat-Releases basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen skalierbareren Ansatz für die Implementierung von Funktionen ermöglicht. Manchmal gibt es mehrere Versionen in einem Monat. Schauen Sie daher regelmäßig nach, um aktuelle Informationen zu erhalten.

Die standardmäßige Seite mit Versionshinweisen für Marketo Engage [finden Sie hier .](/help/marketo/release-notes/current.md){target="_blank"}.

## April-Version {#april-release}

**Veröffentlichungsdatum: 16. April 2024**

### Konversationsflüsse jetzt für Kunden im Paket auswählen verfügbar {#conversational-flows-select-package}

Als wir im letzten Jahr die Conversational Flows veröffentlicht haben, konnten Kunden, die das Dynamic Chat Select-Paket nutzen, die Funktion nur als Testversion von 100 Lebensdauerinteraktionen nutzen. Konversationsflüsse stehen nun allen Kunden im Select-Paket zur Verfügung.

Konversationsflussinteraktionen zählen auf die monatliche Begrenzung von 250 engagierten Konversationen für Kunden im Select-Paket.

### Callback-Funktionen {#callback-functions}

Callback-Funktionen ermöglichen es Ihnen, Dynamic Chat-Analyseereignisse in externen Systemen wie Adobe Analytics oder Google Analytics zu erfassen, wenn Besucher mit Dynamic Chat-Konversationen interagieren. Sie aktivieren Dynamic Chat-Analytics-Ereignisse, indem Sie einen Callback mit der API registrieren, um die Ereignisse zu überwachen. Auf diese Weise können Sie eine ganzheitlichere Sicht auf Ihre Dynamic Chat-Interaktion im Zusammenhang mit anderen wichtigen Daten wie dem Web-Traffic haben.

### Verfügbarkeitsbedingungen für Live-Agenten zu bedingter Verzweigung hinzugefügt {#live-agent-availability-conditional-branching}

Zusätzlich zu nativen und benutzerdefinierten Marketo-Feldern können Sie jetzt bedingte Verzweigungen verwenden, um Verzweigungen basierend auf der Verfügbarkeit von Agenten zu erstellen. Dies ist nützlich, wenn Sie Besuchern nur die Möglichkeit bieten möchten, mit einem Live-Agenten zu sprechen, wenn Live-Agenten verfügbar sind.

SCREENSHOT

### Bedingung für intelligente Liste zu bedingter Verzweigung hinzugefügt {#smart-list-condition}

Durch das Hinzufügen der neuen Marketo Engage-Smart-List-Bedingung zur bedingten Verzweigung können Sie Verzweigungen erstellen, die auf bereits in Marketo erstellten bereits bestehenden Zielgruppen basieren, anstatt die Verzweigungsbedingungen für Zielgruppen im Dynamic Chat zu definieren.

SCREENSHOT

### Bedingte Verzweigung für konversale Flüsse {#conditional-branching-for-conversational-flows}

Wir haben Anfang des Jahres bedingte Verzweigungen für Dialoge veröffentlicht und jetzt können Sie auch die bedingte Verzweigung in Konversationsflüssen nutzen! Bedingte Verzweigungen ermöglichen Ihnen, Verzweigungen in Ihrem Fluss basierend auf unterschiedlichen Bedingungen zu erstellen.

### Live-Chat für Konversationsflüsse {#live-chat-for-conversational-flows}

Wir haben im letzten Jahr Live-Chatfunktionen für Dialoge veröffentlicht, und jetzt können Sie auch Live-Chatinteraktionen in Ihren Konversationsflüssen hinzufügen. Wenn Sie Konversionsflüsse mit Ihren Marketo-Formularen verwenden, können Sie jetzt qualifizierten Besuchern gestatten, unmittelbar nach der Formularübermittlung mit einem Live-Agenten zu chatten!

### Letzte Marketo Engage-Aktivitäten im Agent-Posteingang {#recent-marketo-engage-activities-in-agent-inbox}

Wir haben die letzten Marketo Engage-Aktivitäten zum Abschnitt &quot;Letzte Aktivitäten&quot;des Agenten-Posteingangs hinzugefügt, sodass der Agent leicht erkennen kann, ob der Besucher, der vor Kurzem eine der folgenden Marketo-Aktivitäten ausgeführt hat (letzte 25 Aktivitäten), wenn ein Site-Besucher einen Chat mit einem Agenten anfordert:

* Hat E-Mail geöffnet
* Besuchte Webseite
* Ausgefülltes Formular
* Hatte interessanten Moment

SCREENSHOT

### Verbindungsstatus des Kalenders in der Agentenverwaltung {#calendar-connection-status-in-agent-management}

Administratoren können nun leicht erkennen, welche Agenten mit Buchungsberechtigungen für Meetings ihre Kalender in Dynamic Chat verbunden haben. Dadurch können Sie sicherstellen, dass Ihr gesamtes Vertriebsteam verbunden ist und bereit ist, Meetinganfragen von Dynamic Chat zu akzeptieren.

SCREENSHOT

### Mindestmeldeeinstellung in der Konfiguration des Agentkalenkalenders {#minimum-notice-setting-in-agent-calendar-configuration}

Kunden berichteten, dass Webbesucher mit nur 10 Minuten erweiterter Benachrichtigung Sitzungen in ihrem Kalender buchten. Daher haben wir in der Agentenkalenderkonfiguration eine Mindestwarnungseinstellung eingeführt und die standardmäßige Vorlaufzeit auf 24 Stunden festgelegt.

SCREENSHOT

### Neue In-App-Benachrichtigungen {#new-in-app-notifications}

Wir haben drei neue In-App-Benachrichtigungen eingeführt, die Sie über den Status Ihrer Dynamic Chat-Instanz in Echtzeit informieren.

* Text
* Text
* Text

### Benutzerverhalten aktualisiert hinzufügen/entfernen {#add-remove-user-behavior-updated}

Einige Kunden informieren uns über Probleme beim Hinzufügen und Entfernen von Agenten im dynamischen Chat. Daher haben wir einige Änderungen vorgenommen, um diese Probleme zu beheben.

Wenn ein Benutzer zur Admin Console mit der Berechtigung zum Live-Chat oder zur Buchung von Meetings hinzugefügt wird, wird er sofort in der Liste der Agentenverwaltung angezeigt und kann zu Dialogen, Konversationsflüssen, Routing-Regeln und Teams hinzugefügt werden.

Wenn ein Benutzer mit einer Sitzungsbuchung oder Live-Chat-Berechtigung aus der Admin Console entfernt wird, wird er sofort aus dem Dynamic Chat entfernt, ist nicht mehr für Live-Chat oder Meeting-Routing verfügbar und wird nicht mehr mit Lizenzbeschränkungen gezählt.

### Verbesserte Berichtleistung auf Konversationsebene {#improved-conversation-level-report-performance}

Berichte auf Ebene einzelner Dialogfelder und Konversationsflüsse sind jetzt leistungsfähiger und genauer. Bisher konnte das Laden von Dialogfeldberichten mehrere Sekunden dauern und die Daten waren manchmal nicht mit den globalen Leistungsberichten konsistent. Jetzt werden Ihre einzelnen Dialogfeldberichte sofort geladen und die Daten werden immer mit den globalen Berichtsdaten abgestimmt.

SCREENSHOT

### Berechtigungsaktualisierungen {#permission-updates}

Wir haben die Berechtigungsstruktur und -benennung in Adobe Admin Console bereinigt, um die Berechtigungsverwaltung intuitiver zu gestalten.

* Die Kategorie &quot;Unterhaltungsverwaltung&quot;heißt jetzt &quot;Konversationen&quot;
* Die Kategorie &quot;Sitzungen&quot;heißt jetzt &quot;Aktivitäten&quot;
* Die Kategorie &quot;Agenteneinstellungen&quot;heißt jetzt &quot;Agenten&quot;
* Die Kategorie &quot;Admin-Einstellungen&quot;heißt jetzt &quot;Konfiguration&quot;
* Die Kategorie &quot;Live-Chat&quot;wurde entfernt und alle Live-Chat-Berechtigungen wurden in die Kategorie &quot;Agenten&quot;verschoben

SCREENSHOT

### Unterstützung für Hyperlinks im Agent-Posteingang {#support-for-hyperlinks-in-agent-inbox}

Wenn jetzt Live-Chat-Agenten URLs mit Besuchern im Chat teilen, werden diese URLs per Hyperlink verknüpft, sodass Besucher einfach auf sie klicken können, um zur Seite zu navigieren, anstatt die URL kopieren und in ihren Browser einfügen zu müssen.

### Eingabe des Schlüsselverhaltens, das im Agent-Posteingang aktualisiert wurde {#enter-key-behavior-updated-in-agent-inbox}

Wir haben das Verhalten der Eingabetaste im Agent Inbox so geändert, dass durch Drücken der Eingabe- oder Eingabetaste Ihre Nachricht gesendet wird und durch Drücken von Umschalt+Eingabetaste eine Zeilenumbruch entsteht.

SCREENSHOT

### Round Robin-Seite entfernt {#round-robin-page-removed}

Mach dir keine Sorgen! Das Round Robin Routing ist weiterhin voll funktionsfähig und funktioniert genauso wie immer. Wir haben gerade die Seite entfernt, die eine häufig ungenaue Liste von Agenten und deren Reihenfolge in der Round Robin Routing-Warteschlange anzeigte.

Als wir 2022 Dynamic Chat veröffentlichte, gab es keine Unterstützung für Live-Chat, sondern nur für die Buchung von Meetings und die Round Robin Routing-Seite wurde nur unter Berücksichtigung von Meetingbuchungen entwickelt. Mit der Einführung des Live-Chat im letzten Jahr wurde die Round Robin-Seite überholt, da sie nicht genau die komplexere Art des Round Robin Routing zwischen Agenten mit sowohl Sitzungsbuchung als auch Live-Chat-Berechtigungen widerspiegelt. Wir haben verschiedene Möglichkeiten untersucht, um dieses Problem zu lösen, aber letztlich beschlossen wir, dass die vollständige Abschaffung die beste Option ist, um Verwirrung zu minimieren.

## Version – Februar {#february-release}

**Veröffentlichungsdatum: 22. Februar 2024**

### Seite &quot;Konversationen&quot; {#conversations-page}

Auf der neuen Seite &quot;Konversationen&quot;finden Sie eine zentrale Anlaufstelle, um Transkripte für alle Konversationen (automatisiert und live) anzuzeigen, die für Ihre Instanz stattgefunden haben, sowohl für bekannte als auch für anonyme Leads. So erhalten Sie eine bessere Übersicht darüber, wie Ihre Kunden mit Ihren Dialogfeldern, Konversationsflüssen und Live-Agenten interagieren.

SCREENSHOT

Der Datumsbereich im globalen Dashboard wurde von 90 Tagen auf 24 Monate erhöht

Du hast gefragt, und wir haben geliefert. Sie können jetzt Dynamic Chat-Interaktionsdaten für bis zu zwei Jahre in allen Analyse-Dashboards sehen.

### Bedingte Verzweigung in Dialogfeldern {#conditional-branching-in-dialogues}

Die bedingte Verzweigung ermöglicht es Ihnen, Verzweigungen in Ihren Dialogfeldern basierend auf unterschiedlichen Bedingungen zu erstellen. Jetzt können Sie verschiedenen Personen unterschiedliche Inhalte im selben Dialogfeld basierend auf Lead- und Firmenattributen in Marketo präsentieren.

## Januar-Release {#january-release}

**Veröffentlichungsdatum: 24. Januar 2024**

### Begrenzung für gleichzeitige Live-Chat-Vorgänge in der Agentenverwaltung {#Concurrent-live-chat-limit-setting}

Standardmäßig kann jeder Live-Chat-Agent in Ihrer Instanz maximal fünf Live-Chat-Sitzungen gleichzeitig abhalten. Wir haben eine neue Einstellung für die Agentenverwaltung eingeführt, mit der Sie diese Grenze von 1 bis 10 anpassen können.

SCREENSHOT
