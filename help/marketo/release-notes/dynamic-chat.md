---
description: Dynamic Chat-Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Versionshinweise zu Dynamic Chat
feature: Release Information, Dynamic Chat
exl-id: 0447dc47-b9c5-42e1-8f66-73bf67c7871d
source-git-commit: d88406c1f9d72c57a6d4f09934cbf685499ed198
workflow-type: tm+mt
source-wordcount: '1869'
ht-degree: 3%

---

# Versionshinweise zu Dynamic Chat {#dynamic-chat-release}

Adobe Dynamic Chat-Releases basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen skalierbareren Ansatz für die Implementierung von Funktionen ermöglicht. Manchmal gibt es mehrere Versionen in einem Monat. Schauen Sie daher regelmäßig nach, um aktuelle Informationen zu erhalten.

Die standardmäßige Seite mit Versionshinweisen für Marketo Engage [finden Sie hier ](/help/marketo/release-notes/current.md){target="_blank"}.

## Version August 2024 {#august-release}

**Veröffentlichungsdatum: Samstag, 23. August 2024**

### Benutzerdefiniertes Format für Konversationsnachrichten {#custom-format-conversation-messages}

Stream-Designer unterstützen jetzt das Einfügen von [HTML](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#create-a-stream){target="_blank"}, um das Erscheinungsbild Ihrer Konversationen anzupassen.

![](assets/dynamic-chat-aug-2024-release-1.png)

### ChatBot scrollen zum unteren Rand {#chatbot-scroll-to-bottom}

Im Chat-Bot wurde ein Symbol hinzugefügt, über das Webbesucher direkt zur letzten Nachricht springen können. So können Besucher durch den Text scrollen, um schnell zur Konversation zurückzukehren.

![](assets/dynamic-chat-aug-2024-release-2.png)

### Core-Pulsbenachrichtigungen {#core-pulse-notifications}

Benutzer erhalten jetzt eine [E-Mail-Benachrichtigung](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#failed-action-notifications){target="_blank"}, wenn die Buchung eines Meetings oder ein Live-Chat fehlschlägt.

![](assets/dynamic-chat-aug-2024-release-3.png)

### Unterstützung mehrerer Konversationen {#support-for-multiple-conversations}

Der Chatbot unterstützt jetzt mehrere Konversationen. Website-Besucher können auf verschiedenen Seiten gleichzeitig verschiedene Gespräche führen, mit der Möglichkeit, zwischen ihnen zu wechseln.

![](assets/dynamic-chat-aug-2024-release-4.png)

### Standardmäßige Sortierung für Inhalte {#default-sorting-for-content}

Standardmäßig werden Ihre Konversationslogs, unbeantwortete Fragen und Tabellen zur Fragengenerierung nach dem Erstellungsdatum (vom letzten zum ältesten) sortiert.

### Echtzeit-Lead-Auflösung {#real-time-lead-resolution}

Bei einer Konversation mit einem anonymen Lead und einer E-Mail-ID lösen wir auf, ob ein bekannter Lead-Datensatz mit dieser E-Mail-ID vorhanden ist, und verwenden diesen Datensatz zur Personalisierung in Echtzeit. Wenn wir mehrere Datensätze finden, führen wir sie in Echtzeit zusammen. Dieses Verhalten ist sowohl für Dialogfelder als auch für Konversationsflüsse implementiert.

### Synchronisieren von Leads ohne Cookies von Marketo Engage {#syncing-leads-without-cookies}

Bisher wurden bei Aktivierung der Marketo Engage-Synchronisation nur bekannte Leads von Dynamic Chat mit einer oder mehreren Cookie-IDs von Marketo Engage synchronisiert. Jetzt werden alle bekannten Leads (Cookie-ID vorhanden oder nicht) mit Dynamic Chat synchronisiert und können für die Personalisierung von Konversationen verwendet werden.

### Übergeben zusätzlicher Besucherdaten an Konversationsflüsse {#pass-additional-visitor-data}

Wenn Sie Besucherinformationen über andere Kanäle wie Formulare oder Anmeldedaten erfassen, können Sie diese Informationen jetzt direkt an Dynamic Chat weitergeben.

![](assets/dynamic-chat-aug-2024-release-5.png)

### Aktualisierte abgeleitete Daten {#refreshed-inferred-data}

Die meisten Unterhaltungen auf einer Website erfolgen mit anonymen Besuchern. Sie können sie weiterhin mithilfe von abgeleiteten Daten ansprechen, die auf Besucher-IPs angewiesen sind. Wir haben unsere Datenbank mit IPs und entsprechenden abgeleiteten Daten aktualisiert, die jetzt viermal mehr IPs unterstützt.

### Ton zur Agent-Browserbenachrichtigung hinzugefügt {#sound-added-to-agent-browser-notification}

Wenn einem Agenten ein Live-Chat zugewiesen wird, erhält er eine Browserbenachrichtigung. Aber gelegentlich sehen sie sie nicht. Wir haben einen [Benachrichtigungs-Sound](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#when-a-live-chat-is-routed-to-an-agent){target="_blank"} hinzugefügt, um zu verhindern, dass in Zukunft verpasste Benachrichtigungen gesendet werden.

![](assets/dynamic-chat-aug-2024-release-6.png)

### Möglichkeit, das Lead-Profil während des Live-Chat zu aktualisieren {#update-lead-profile-during-live-chat}

Während eines Live-Chat möchten Agenten Informationen über den Besucher erfassen und das entsprechende Profil aktualisieren. Es gibt jetzt die Möglichkeit, die Attributwerte von Lead- und Firmenobjekten zu aktualisieren.

![](assets/dynamic-chat-aug-2024-release-7.png)

## Version Juni 2024 {#june-release}

**Veröffentlichungsdatum: Freitag, 6. Juni 2024**

### Konversionsflusskarte {#conversational-flow-card}

Straffen Sie mehrere Schritte in einem Fluss innerhalb Ihrer Dialoge, indem Sie die Karte Konversionsfluss nutzen.

Beispiel: Wenn Sie die Registrierung für Ihr Webinar über mehrere Dialoge durchführen möchten, müssen Sie denselben Fluss über alle Dialoge mit diesem Ziel neu erstellen. Und wenn Sie jedes Detail aktualisieren müssen, müssen Sie jedes einzelne Dialogfeld einzeln bearbeiten. Das ist nicht mehr der Fall, dank der Karte &quot;Conversational Flow&quot;.

Sie können nicht nur die Weiterverwendung von Flüssen über mehrere Dialogfelder hinweg ermöglichen, sondern auch denselben Übergangsprozess zum Trigger über andere Kanäle wie Formulare und Landingpages verwenden.

![](assets/dynamic-chat-june-2024-release-1.png)

### Nutzungsbeschränkungen {#usage-limits}

Auf der Seite Nutzungsbeschränkungen werden wichtige Informationen angezeigt, wie Paketdetails und Ihr Nutzungsbegrenzungsstatus.

![](assets/dynamic-chat-june-2024-release-2.png)

## Version Mai 2024 {#may-release}

**Veröffentlichungsdatum: Donnerstag, 15. Mai 2024**

### Vorab genehmigte Antwortbibliothek {#pre-approved-response-library}

[Erstellen Sie eine Bibliothek, die für das Marketing genehmigt wurde](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md){target="_blank"} mit KI-generierten Fragen und Antworten, um den Generativen KI-Chat in Minuten einzurichten.

![](assets/dynamic-chat-may-2024-release-1.png)

### Unbeantwortete Fragen {#unanswered-questions}

[Verwenden Sie ein Repository mit unbeantworteten Fragen](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/unanswered-questions.md){target="_blank"} aus früheren Konversationen, um neue vorab genehmigte Antworten zu generieren und dabei eine Antwortbibliothek mit den neuesten Informationen zu verwalten.

![](assets/dynamic-chat-may-2024-release-2.png)

### Konversationszusammenfassungen {#conversation-summaries}

[Geben Sie Vertriebsmitarbeitern zusammengefasste Gespräche](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#conversation-summary){target="_blank"}, einschließlich Einblicken in wichtige Diskussionsthemen im Vorfeld von Sitzungen, um die Vorbereitungszeit zu verkürzen und Vertriebsmitarbeiter mit den neuesten Informationen besser zu rüsten.

![](assets/dynamic-chat-may-2024-release-3.png)

### Tastenkombinationen für GenAI {#genai-sales-shortcuts}

[Bieten Sie Live-Chat-Agenten schnellere Möglichkeiten](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#shortcuts){target="_blank"}, um auf KI-generierte Antworten zuzugreifen, vorhandene generierte Antworten zu bearbeiten und nach zusätzlichen Inhalten zu suchen, die während der Konversation an Käufer gesendet werden.

![](assets/dynamic-chat-may-2024-release-4.png)

### Unterhaltungshilfe {#conversation-assist}

Hilfe für Vertriebsmitarbeiter bei Live-Unterhaltungen mit von Ihrem Marketing-Team vorab genehmigten Antworten.

### Diskussionsforen {#conversation-nudges}

Fügen Sie Webbesuchern einen Aktionsaufruf hinzu, um Gespräche zum Abschluss zu bringen.

<p>

## Version April 2024 {#april-release}

**Veröffentlichungsdatum: Mittwoch, 23. April 2024**

### Konversationsflüsse jetzt für alle Benutzer verfügbar {#conversational-flows-available-to-all-users}

Gestalten Sie Ihre Formulare und Landingpages kommunikativer und verkürzen Sie den Verkaufstrichter, indem Sie qualifizierten Leads erlauben, ein Meeting oder einen Chat mit Sales unmittelbar nach der Formularübermittlung mit Conversational Forms zu buchen, der jetzt für alle Dynamic Chat-Benutzer voll verfügbar ist.&#42;

_&#42;Zuvor als Testfunktion mit 100 Lebensdauerinteraktionen verfügbar. Die Interaktionen mit dem Konversationsfluss werden jetzt auf die monatliche Begrenzung von 250 Interaktionen angerechnet, die für Benutzer mit dem Select-Paket erforderlich sind._

### Callback-Funktionen {#callback-functions}

[Callback-Funktionen](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/callback-functions.md){target="_blank"} ermöglichen es Ihnen, Dynamic Chat-Analytics-Ereignisse in externen Systemen wie Adobe Analytics oder Google Analytics zu erfassen, wenn Besucher mit Dynamic Chat-Konversationen interagieren. Sie aktivieren Dynamic Chat-Analytics-Ereignisse, indem Sie einen Callback mit der API registrieren, um die Ereignisse zu überwachen. Auf diese Weise können Sie eine ganzheitlichere Sicht auf Ihre Dynamic Chat-Interaktion im Zusammenhang mit anderen wichtigen Daten wie dem Web-Traffic haben.

### Verfügbarkeitsbedingungen für Live-Agenten zu bedingter Verzweigung hinzugefügt {#live-agent-availability-conditional-branching}

Zusätzlich zu nativen und benutzerdefinierten Marketo Engage-Feldern können Sie jetzt bedingte Verzweigungen verwenden, um Verzweigungen basierend auf der Verfügbarkeit von Agenten zu erstellen. Dies ist nützlich, wenn Sie Besuchern nur die Möglichkeit bieten möchten, mit einem Live-Agenten zu sprechen, wenn Live-Agenten verfügbar sind.

![](assets/dynamic-chat-release-1.png)

### Bedingung für intelligente Liste zu bedingter Verzweigung hinzugefügt {#smart-list-condition}

Durch das Hinzufügen der neuen Marketo Engage-Smart-List-Bedingung zur bedingten Verzweigung können Sie Verzweigungen erstellen, die auf bereits in Marketo Engage erstellten bereits bestehenden Zielgruppen basieren, anstatt die Verzweigungsbedingungen für Zielgruppen im Dynamic Chat zu definieren.

![](assets/dynamic-chat-release-2.png)

### Bedingte Verzweigung für konversale Flüsse {#conditional-branching-for-conversational-flows}

Wir haben Anfang dieses Jahres bedingte Verzweigungen für Dialoge veröffentlicht, und jetzt können Sie auch die bedingte Verzweigung in Konversationsflüssen nutzen! Bedingte Verzweigungen ermöglichen es Ihnen, Verzweigungen in Ihrem Fluss basierend auf unterschiedlichen Bedingungen zu erstellen.

### Live-Chat für Konversationsflüsse {#live-chat-for-conversational-flows}

Wir haben 2023 die Live-Chatfunktion für Dialoge veröffentlicht und jetzt können Sie auch Live-Chatinteraktionen zu Ihren Konversationsflüssen hinzufügen. Wenn Sie Konversionsflüsse mit Ihren Marketo Engage-Formularen verwenden, können Sie jetzt qualifizierten Besuchern erlauben, unmittelbar nach der Formularübermittlung mit einem Live-Agenten zu chatten!

### Letzte Marketo Engage-Aktivitäten im Agent-Posteingang {#recent-marketo-engage-activities-in-agent-inbox}

Wir haben die letzten Marketo Engage-Aktivitäten zum Abschnitt &quot;Letzte Aktivitäten&quot;des Agenten-Posteingangs hinzugefügt. Wenn ein Site-Besucher also einen Chat mit einem Agenten anfordert, kann der Agent schnell erkennen, ob der Besucher kürzlich eine der folgenden Marketo Engage-Aktivitäten ausgeführt hat (letzte 25 Aktivitäten):

* Hat E-Mail geöffnet
* Besuchte Webseite
* Ausgefülltes Formular
* Hatte interessanten Moment

![](assets/dynamic-chat-release-3.png)

### Verbindungsstatus des Kalenders in der Agentenverwaltung {#calendar-connection-status-in-agent-management}

Administratoren können nun leicht erkennen, welche Agenten mit Buchungsberechtigungen für Meetings ihre Kalender in Dynamic Chat verbunden haben. Dadurch können Sie sicherstellen, dass Ihr gesamtes Vertriebsteam verbunden ist und die Möglichkeit hat, Besprechungsanfragen von Dynamic Chat zu akzeptieren.

![](assets/dynamic-chat-release-4.png)

### Mindestmeldeeinstellung in der Konfiguration des Agentkalenkalenders {#minimum-notice-setting-in-agent-calendar-configuration}

Benutzer berichteten, dass Webbesucher mit nur 10 Minuten erweiterter Benachrichtigung Sitzungen in ihrem Kalender buchten. Daher haben wir in die Agentenkalenderkonfiguration eine Mindestwarnungseinstellung eingeführt und die standardmäßige Vorlaufzeit auf 24 Stunden festgelegt.

![](assets/dynamic-chat-release-5.png)

### Benutzerverhalten aktualisiert hinzufügen/entfernen {#add-remove-user-behavior-updated}

Einige Benutzer gaben an, dass beim Hinzufügen und Entfernen von Agenten im dynamischen Chat Probleme aufgetreten seien. Daher haben wir einige Änderungen vorgenommen, um diese Probleme zu beheben.

Wenn ein Benutzer zur Admin Console mit einer Live-Chat- oder Sitzungsbuchungsberechtigung hinzugefügt wird, wird er sofort in der Liste der Agentenverwaltung angezeigt und kann zu Dialogfeldern, Gesprächsflüssen, Routing-Regeln und Teams hinzugefügt werden.

Wenn ein Benutzer mit einer Sitzungsbuchung oder Live-Chat-Berechtigung aus der Admin Console entfernt wird, wird er sofort aus dem Dynamic Chat entfernt, ist nicht mehr für Live-Chat oder Meeting-Routing verfügbar und wird nicht mehr mit Lizenzbeschränkungen gezählt.

### Verbesserte Berichtleistung auf Konversationsebene {#improved-conversation-level-report-performance}

Berichte auf Ebene einzelner Dialogfelder und Konversationsflüsse sind jetzt leistungsfähiger und genauer. Bisher konnte das Laden von Dialogfeldberichten mehrere Sekunden dauern und die Daten waren gelegentlich nicht mit den globalen Leistungsberichten konsistent. Jetzt werden Ihre einzelnen Dialogfeldberichte sofort geladen und die Daten werden immer mit den globalen Berichtsdaten abgestimmt.

![](assets/dynamic-chat-release-6.png)

### Berechtigungsaktualisierungen {#permission-updates}

Wir haben die Berechtigungsstruktur und -benennung in Adobe Admin Console bereinigt, um die Berechtigungsverwaltung intuitiver zu gestalten.

* Die Kategorie &quot;Unterhaltungsverwaltung&quot;heißt nun &quot;Konversationen&quot;.
* Die Kategorie &quot;Meetings&quot;heißt jetzt &quot;Aktivitäten&quot;
* Die Kategorie &quot;Agenteneinstellungen&quot;heißt jetzt &quot;Agenten&quot;.
* Die Kategorie &quot;Admin-Einstellungen&quot;heißt jetzt &quot;Konfiguration&quot;
* Die Kategorie &quot;Live-Chat&quot;wurde entfernt und alle Live-Chat-Berechtigungen wurden in die Kategorie &quot;Agenten&quot;verschoben.

![](assets/dynamic-chat-release-7.png)

### Unterstützung für Hyperlinks im Agent Inbox {#support-for-hyperlinks-in-agent-inbox}

Wenn jetzt Live-Chat-Agenten URLs mit Besuchern im Chat teilen, werden diese URLs per Hyperlink verknüpft, sodass Besucher einfach auf sie klicken können, um zur Seite zu navigieren, anstatt die URL kopieren und in ihren Browser einfügen zu müssen.

### Eingabe des Schlüsselverhaltens, das im Agent-Posteingang aktualisiert wurde {#enter-key-behavior-updated-in-agent-inbox}

Wir haben das Verhalten der Eingabetaste im Agent Inbox umgestellt. Drücken Sie also die Eingabe- oder Eingabetaste, um Ihre Nachricht zu senden, und drücken Sie Umschalt+Eingabetaste, um einen Zeilenumbruch zu erzeugen.

![](assets/dynamic-chat-release-8.png)

### Round Robin-Seite entfernt {#round-robin-page-removed}

Mach dir keine Sorgen! Das Round Robin Routing ist noch voll funktionsfähig und funktioniert genauso wie immer. Wir haben gerade die Seite entfernt, die eine häufig ungenaue Liste von Agenten und deren Reihenfolge in der Round Robin Routing-Warteschlange anzeigte.

Als wir 2022 Dynamic Chat herausbrachten, gab es keine Unterstützung für Live-Chat, nur Meetingbuchungen, und die Round Robin Routing-Seite wurde nur unter Berücksichtigung der Buchung konzipiert. Mit der Einführung des Live-Chat im letzten Jahr wurde die Round Robin-Seite überholt, da sie nicht genau die komplexere Art des Round Robin Routing zwischen Agenten mit sowohl Sitzungsbuchung als auch Live-Chat-Berechtigungen widerspiegelt. Wir haben verschiedene Möglichkeiten untersucht, um dieses Problem zu lösen, aber letztlich beschlossen wir, dass die vollständige Abschaffung die beste Option ist, um Verwirrung zu minimieren.

![](assets/dynamic-chat-release-9.png)

## Version Februar 2024 {#february-release}

**Versionsdatum: Freitag, 22. Februar 2024**

### Seite &quot;Konversationen&quot; {#conversations-page}

Auf der neuen Seite &quot;Konversationen&quot;finden Sie eine zentrale Anlaufstelle, um Transkripte für alle Konversationen (automatisiert und live) anzuzeigen, die für Ihre Instanz stattgefunden haben, sowohl für bekannte als auch für anonyme Leads. So erhalten Sie eine bessere Übersicht darüber, wie Ihre Kunden mit Ihren Dialogfeldern, Konversationsflüssen und Live-Agenten interagieren.

![](assets/dynamic-chat-release-10.png)

### Der Datumsbereich im globalen Dashboard wurde von 90 Tagen auf 24 Monate erhöht {#date-range-in-global-dashboard}

Du hast gefragt, und wir haben geliefert. Sie können jetzt Dynamic Chat-Interaktionsdaten für bis zu zwei Jahre in allen Analyse-Dashboards sehen.

### Bedingte Verzweigung in Dialogfeldern {#conditional-branching-in-dialogues}

Die bedingte Verzweigung ermöglicht es Ihnen, Verzweigungen in Ihren Dialogfeldern basierend auf unterschiedlichen Bedingungen zu erstellen. Jetzt können Sie verschiedene Inhalte für verschiedene Personen im selben Dialogfeld darstellen, basierend auf den Lead- und Firmenattributen in Marketo Engage.

## Version Januar 2024 {#january-release}

**Versionsdatum: Donnerstag, 24. Januar 2024**

### Begrenzung für gleichzeitige Live-Chat-Vorgänge in der Agentenverwaltung {#Concurrent-live-chat-limit-setting}

Standardmäßig kann jeder Live-Chat-Agent in Ihrer Instanz maximal fünf Live-Chat-Sitzungen gleichzeitig abhalten. Wir haben eine neue Einstellung für die Agentenverwaltung eingeführt, mit der Sie diese Grenze von 1 auf 10 anpassen können.

![](assets/dynamic-chat-release-11.png)
