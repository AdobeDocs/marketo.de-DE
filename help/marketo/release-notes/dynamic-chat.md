---
description: Dynamic Chat-Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Versionshinweise zu Dynamic Chat
feature: Release Information, Dynamic Chat
exl-id: 0447dc47-b9c5-42e1-8f66-73bf67c7871d
source-git-commit: fddc2f24d9a66146f567c762305ab2825c2f29ae
workflow-type: tm+mt
source-wordcount: '2571'
ht-degree: 2%

---

# Versionshinweise zu Dynamic Chat {#dynamic-chat-release}

Adobe Dynamic Chat-Versionen basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren Ansatz für die Bereitstellung von Funktionen ermöglicht. Manchmal gibt es mehrere Versionen in einem Monat, daher schauen Sie regelmäßig nach den aktuellsten Informationen.

Die Seite mit den standardmäßigen Versionshinweisen für Marketo Engage [finden Sie hier](/help/marketo/release-notes/current.md){target="_blank"}.

## Version April/Mai 2025 {#apr-may-25-release}

### Benachrichtigungssound {#message-notification-sound}

Jetzt haben Sie die Möglichkeit, jedes Mal, wenn der Chatbot in einer Sitzung ausgelöst wird, einen Ton für den Besucher zu aktivieren. Es stehen mehrere Sounds zur Auswahl.

### POKE-Nachrichten auf Mobilgeräten aktivieren {#enable-poke-messages-on-mobile}

„Poke“, der die Eröffnungsfrage neben dem Chat-Symbol anzeigt, ohne dass der Besucher darauf klicken muss, um es zu sehen, ist jetzt eine Option, die für Besucher, die ein Mobilgerät verwenden, aktiviert werden kann.

### Standardmäßige Fallback-Aktualisierung {#default-fallback-update}

Für benutzerdefinierte Regeln/Teams als Live-Chat-Karte - wenn keine Agenten verfügbar sind (oder der Chat keine Verbindung herstellen kann), wird für verfügbare Agenten (alle, die zu diesem Zeitpunkt verfügbar sind, unabhängig davon, welche Routing-Logik/Regel im Stream platziert wurde) auf Round Robin zurückgesetzt.

### Demandbase-Integration {#demandbase-integration}

Demandbase-Benutzer können Demandbase-Personenattribute für Dialog-Targeting, bedingtes Branding und benutzerdefiniertes Routing in Dynamic Chat verwenden.

## Version September/Oktober 2024 {#sep-oct-release}

### Erweiterte Live-Chat-Analyse {#enhanced-live-chat-analytics}

Das Analytics-Dashboard wurde u. a. in folgenden Punkten verbessert:

* Gesamtzahl der angeforderten Live-Chats: Anzahl der Besucher, die für einen „Chat mit dem Agenten“ angefordert wurden

* Total Connected Live Chat: Anzahl der verbundenen Besucher im Vergleich zur Gesamtzahl der angeforderten Besucher für einen „Chat mit Agent“

* Gesamtzahl der verpassten Live-Chat-Anfragen: Anzahl der Besucher ohne Anwesenheit im Vergleich zur Gesamtzahl der Anfragen für einen „Chat mit Agent“

* Durchschnittliche Chatlänge in Minuten: Analysieren Sie die „durchschnittliche Chatlänge“ zwischen Besuchern und Ihren Agenten

* Durchschnittliche Reaktionszeit des Agenten in Sekunden: Analysieren Sie die „durchschnittliche Zeit“, die Agenten benötigen, um auf Fragen und Antworten zum Live-Chat zu reagieren.

* Tägliches Dashboard: Live-Chat-Anfragen erfolgreich verbunden, Live-Chat-Anfragen verpasst, letzte Live-Chat-Aktivitäten sortiert und gefiltert

![](assets/dynamic-chat-sep-oct-2024-release-1.png)

### Konversationsbewertung {#conversation-scoring}

Quantifizieren Sie Ihre Leads basierend auf der Qualität ihrer Chat-Interaktion und verwenden Sie diese Metrik als Trigger/Filter in Marketo Engage Smart Campaign. Verwenden Sie das neue Attribut _Konversationswert_ für die folgenden Aktivitäten:

* Hat einen Dialog geführt
* Interagiert mit einem Gesprächsfluss
* Interagiert mit einem Agenten

**Zu beachten:**

* Der Wert der Punktzahl liegt zwischen 0, 1, 2, 3 (der Standardwert ist null)

* Nach Abschluss oder Ablegen des Gesprächs kann der Scoring-Wert nicht mehr bearbeitet werden

* Punktzahl festlegen:

   * Im Posteingang des Agenten - Während eines Live-Chats kann der Agent einen Wert für die Konversation aktualisieren oder festlegen, der in der Konversationsaktivität gespeichert wird

   * Im Stream-Designer - auf der Zielkarte kann der Benutzer eine Punktzahl für die Konversation aktualisieren oder festlegen

![](assets/dynamic-chat-sep-oct-2024-release-2.png)

![](assets/dynamic-chat-sep-oct-2024-release-3.png)

![](assets/dynamic-chat-sep-oct-2024-release-4.png)

### Neue Logik zur Lead-Erstellung {#new-lead-creation-logic}

Wenn ein Lead ein Formular mit der E-Mail-`abc@test.com` ausfüllt und als „xyz“ gekocht wird, füllt er dasselbe Formular später mit der E-Mail-`def@test.com` aus, es wird ein neuer Personendatensatz erstellt, aber das Cookie „xyz“ wird mit der neuen Person verknüpft und aus der `abc@test.com` entfernt.

Wenn also ein Besucher mit dem Cookie abc auf einer Seite landet und eine E-Mail-ID wie `abc@test.com` bereitstellt:

<table><thead>
  <tr>
    <th>Visitor</th>
    <th>Cookie</th>
    <th>E-Mail bereitgestellt</th>
    <th>Erwartetes Verhalten</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Anonym</td>
    <td>ABC</td>
    <td>Existiert nicht in der Datenbank</td>
    <td>Neue Person erstellen</td>
  </tr>
  <tr>
    <td>Anonym</td>
    <td>ABC</td>
    <td>Existiert in Datenbank</td>
    <td>Person fusionieren</td>
  </tr>
  <tr>
    <td>Anonym</td>
    <td>xyz</td>
    <td>Existiert in Datenbank</td>
    <td>Person fusionieren</td>
  </tr>
  <tr>
    <td>Bekannte Person</td>
    <td>ABC</td>
    <td>Gleich wie vorhandene Person</td>
    <td>Person aktualisieren</td>
  </tr>
  <tr>
    <td>Bekannte Person</td>
    <td>ABC</td>
    <td>Anders als bei vorhandener Person</td>
    <td>Wenn bereits eine bekannte Person vorhanden ist, übertragen Sie das Cookie und lösen Sie dieses Profil auf. Wenn mit dieser E-Mail keine Person existiert, erstellen Sie einen neuen Personendatensatz und übertragen Sie das Cookie</td>
  </tr>
  <tr>
    <td>Bekannte Person</td>
    <td>xyz</td>
    <td>Gleich wie vorhandene Person</td>
    <td>Hinzufügen eines neuen Cookies zu derselben Person</td>
  </tr>
  <tr>
    <td>Bekannte Person</td>
    <td>xyz</td>
    <td>Anders als bei vorhandener Person</td>
    <td>Dieses Szenario ist nicht möglich, als wäre es ein neues Cookie von   Standard als neues anonymes Profil betrachtet</td>
  </tr>
</tbody></table>

### Option zum Übernehmen der Schriftart {#option-to-inherit-font}

Sie können jetzt den Chatbot aktivieren, um die Schriftart direkt von der Web-Seite zu erben, auf der sie gehostet wird, anstatt die Markenschriftart in Dynamic Chat zu verwalten. Wenn Sie diese Option aktivieren, übernimmt der Chatbot die Schriftart, die für `<body>` Tag der Seite definiert ist.

![](assets/dynamic-chat-sep-oct-2024-release-5.png)

### Demandbase-Integration mit Dynamic Chat {#demandbase-integration-with-dynamic-chat}

Demandbase-Benutzer können ihre eigene Lizenz von Demandbase mitbringen und die Integration aktivieren. Verwenden Sie Demandbase-Personenattribute für Dialog-Targeting, bedingtes Branding und benutzerdefiniertes Routing.

Die Auflösung dieser Attributwerte gegenüber einer Person erfolgt in Echtzeit und wird im jeweiligen Personenprofil gespeichert.

### Optimierte Ladezeit des Konversationsflusses {#optimized-conversation-flow-load-time}

Um das Benutzererlebnis zu verbessern, wird jetzt beim Laden des Konversationsflusses anstelle eines Leerraums ein Schimmerlader angezeigt.

**vor**

![](assets/dynamic-chat-sep-oct-2024-release-6.png)

**nachher**

![](assets/dynamic-chat-sep-oct-2024-release-7.gif)

## Version August 2024 {#august-release}

**Veröffentlichungsdatum: Samstag, 23. August 2024**

### Benutzerdefiniertes Formatieren Ihrer Konversationsnachrichten {#custom-format-conversation-messages}

Stream-Designer unterstützen jetzt [Einfügen von HTML](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#create-a-stream){target="_blank"} um das Erscheinungsbild Ihrer Unterhaltungen anzupassen.

![](assets/dynamic-chat-aug-2024-release-1.png)

### Chatbot scrollen nach unten {#chatbot-scroll-to-bottom}

Im Chatbot wurde ein Symbol hinzugefügt, über das Web-Besucher direkt zur letzten Nachricht springen können. Auf diese Weise können Besucher den Text durchscrollen, um schnell zur Konversation zurückzukehren.

![](assets/dynamic-chat-aug-2024-release-2.png)

### Core-Puls-Benachrichtigungen {#core-pulse-notifications}

Benutzer erhalten jetzt eine [E-Mail-Benachrichtigung](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#failed-action-notifications){target="_blank"} wenn eine Besprechungsbuchung oder ein Live-Chat fehlschlägt.

![](assets/dynamic-chat-aug-2024-release-3.png)

### Unterstützung für mehrere Konversationen {#support-for-multiple-conversations}

Der Chatbot unterstützt jetzt mehrere Konversationen. Website-Besucherinnen und -Besucher können sich gleichzeitig an verschiedenen Konversationen auf verschiedenen Seiten beteiligen und zwischen ihnen wechseln.

![](assets/dynamic-chat-aug-2024-release-4.png)

### Standardsortierung für Inhalte {#default-sorting-for-content}

Standardmäßig werden Ihre Konversationsprotokolle, unbeantwortete Fragen und Fragenerierungstabellen nach Erstellungsdatum (vom letzten zum ältesten) sortiert.

### Echtzeit-Lead-Auflösung {#real-time-lead-resolution}

Während eines Gesprächs mit einem anonymen Lead und einer E-Mail-ID klären wir, ob ein bekannter Lead-Datensatz mit dieser E-Mail-ID vorhanden ist, und verwenden diesen Datensatz für die Personalisierung in Echtzeit. Wenn wir mehrere Datensätze finden, führen wir sie in Echtzeit zusammen. Dieses Verhalten ist sowohl für Dialogfelder als auch für Konversationsflüsse implementiert.

### Synchronisieren von Leads ohne Cookies von Marketo Engage {#syncing-leads-without-cookies}

Zuvor, als die Marketo Engage-Synchronisierung aktiviert wurde, synchronisierte Dynamic Chat nur bekannte Leads mit einer oder mehreren Cookie-IDs von Marketo Engage. Jetzt werden alle bekannten Leads (Cookie-ID vorhanden oder nicht) mit Dynamic Chat synchronisiert und können für die Personalisierung von Konversationen verwendet werden.

### Weitergeben zusätzlicher Besucherdaten an Konversationsflüsse {#pass-additional-visitor-data}

Wenn Sie Besucherinformationen über andere Kanäle wie Formulare oder Anmeldung erfassen, können Sie diese Informationen jetzt direkt an Dynamic Chat weitergeben.

![](assets/dynamic-chat-aug-2024-release-5.png)

### Abgeleitete Daten aktualisiert {#refreshed-inferred-data}

Die meisten Gespräche auf einer Website werden mit anonymen Besuchern geführt. Sie können sie weiterhin über abgeleitete Daten ansprechen, die auf Besucher-IPs angewiesen sind. Wir haben unsere IP-Datenbank und die entsprechenden abgeleiteten Daten aktualisiert, sodass jetzt viermal so viele IP-Adressen unterstützt werden.

### Ton zur Browser-Benachrichtigung des Agenten hinzugefügt {#sound-added-to-agent-browser-notification}

Wenn ein Live-Chat einem Agenten zugewiesen wird, erhält er eine Browser-Benachrichtigung. Aber gelegentlich sehen sie sie nicht. Wir haben einen [Benachrichtigungston“ hinzugefügt](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#when-a-live-chat-is-routed-to-an-agent){target="_blank"} um verpasste Benachrichtigungen in Zukunft zu vermeiden.

![](assets/dynamic-chat-aug-2024-release-6.png)

### Möglichkeit, das Lead-Profil während des Live-Chats zu aktualisieren {#update-lead-profile-during-live-chat}

Während eines Live-Chats möchten Kundendienstmitarbeiter Informationen über den Besucher erfassen und das jeweilige Profil aktualisieren. Es gibt jetzt eine Option, um Attributwerte von Lead- und Unternehmensobjekten zu aktualisieren.

![](assets/dynamic-chat-aug-2024-release-7.png)

## Version Juni 2024 {#june-release}

**Veröffentlichungsdatum: Freitag, 6. Juni 2024**

### Dialogfeldkarte {#conversational-flow-card}

Optimieren Sie mehrere Schritte in einem Fluss in Ihren Dialogfeldern, indem Sie die Karte „Konversativer Fluss“ verwenden.

Beispiel: Wenn Ihr Ziel darin besteht, Registrierungen für Ihr Webinar über mehrere Dialogfelder voranzutreiben, müssen Sie denselben Fluss über alle Dialogfelder hinweg neu erstellen, die dieses Ziel haben. Und wenn Sie Details aktualisieren müssen, müssen Sie jedes einzelne Dialogfeld einzeln bearbeiten. Das ist dank der Conversational Flow-Karte nicht mehr der Fall.

Zusätzlich zur Neuverwendung von Flüssen über mehrere Dialogfelder hinweg können Sie denselben Übergangsfluss auch für Trigger über andere Kanäle wie Formulare und Landingpages verwenden.

![](assets/dynamic-chat-june-2024-release-1.png)

### Nutzungsbeschränkungen {#usage-limits}

Die Seite „Nutzungsbeschränkungen“ enthält wichtige Informationen wie Paketdetails und den Status Ihrer Nutzungsbeschränkung.

![](assets/dynamic-chat-june-2024-release-2.png)

## Version Mai 2024 {#may-release}

**Veröffentlichungsdatum: Donnerstag, 15. Mai 2024**

### Bibliothek mit vorab genehmigten Antworten {#pre-approved-response-library}

[Erstellen Sie eine vom Marketing genehmigte Bibliothek](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md){target="_blank"} mit von KI generierten Fragen und Antworten, um in Minutenschnelle einen Chat mit generativer KI einzurichten.

![](assets/dynamic-chat-may-2024-release-1.png)

### Unbeantwortete Fragen {#unanswered-questions}

[Verwenden Sie ein Repository mit unbeantworteten Fragen](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/unanswered-questions.md){target="_blank"} aus früheren Unterhaltungen, um neue vorab genehmigte Antworten zu generieren und eine Antwortbibliothek mit den neuesten Informationen zu verwalten.

![](assets/dynamic-chat-may-2024-release-2.png)

### Zusammenfassung der Unterhaltung {#conversation-summaries}

[Geben Sie den Vertriebsmitarbeitern zusammengefasste ](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#conversation-summary){target="_blank"}, einschließlich Einblicken in wichtige Diskussionsthemen, bevor Meetings stattfinden, um die Vorbereitungszeit zu verkürzen und die Vertriebsmitarbeiter besser mit den neuesten Informationen zu versorgen.

![](assets/dynamic-chat-may-2024-release-3.png)

### Vertriebs-Shortcuts für GenAI {#genai-sales-shortcuts}

[Liefern Sie Live-Chat-Agenten schnellere Möglichkeiten](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#shortcuts){target="_blank"} um auf KI-generierte Antworten zuzugreifen, vorhandene generierte Antworten zu bearbeiten und nach zusätzlichen Inhalten zu suchen, die während des Gesprächs an Käufer gesendet werden können.

![](assets/dynamic-chat-may-2024-release-4.png)

### Unterhaltungshilfe {#conversation-assist}

Helfen Sie den Vertriebsmitarbeitern, bei Live-Gesprächen mithilfe von Antworten, die vorab von Ihrem Marketing-Team genehmigt wurden, genau zu reagieren.

### Unterhaltungs-Stupser {#conversation-nudges}

Anspornen Sie Web-Besucher mit einer call-to-action, um die Gespräche zum Abschluss zu bringen.

<p>

## Version April 2024 {#april-release}

**Veröffentlichungsdatum: Mittwoch, 23. April 2024**

### Konversationsflüsse sind jetzt für alle Benutzer verfügbar {#conversational-flows-available-to-all-users}

Gestalten Sie Ihre Formulare und Landingpages dialogfähiger und verkürzen Sie den Verkaufstrichter, indem Sie qualifizierten Leads erlauben, sofort nach einer Formularübermittlung mit Conversational Forms, die jetzt für alle Dynamic Chat-Benutzenden vollständig verfügbar ist, ein Meeting zu buchen &#42; mit dem Vertrieb zu chatten.

_&#42;Zuvor als Testfunktion mit 100 lebenslangen Interaktionen verfügbar. Gespräche werden jetzt für das monatliche Limit von 250 Gesprächen gezählt, die Benutzende mit dem Select-Paket führen._

### Rückruffunktionen {#callback-functions}

[Rückruffunktionen](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/callback-functions.md){target="_blank"} ermöglichen es Ihnen, Dynamic Chat-Analyseereignisse in externen Systemen wie Adobe Analytics oder Google Analytics zu erfassen, wenn Besucherinnen und Besucher mit Dynamic Chat-Konversationen interagieren. Sie aktivieren Dynamic Chat-Analyseereignisse, indem Sie einen Callback bei der -API registrieren, um auf die Ereignisse zu warten. Auf diese Weise erhalten Sie einen ganzheitlicheren Überblick über Ihre Dynamic Chat-Interaktion, da sie sich auf andere wichtige Daten wie Web-Traffic bezieht.

### Live Agent-Verfügbarkeitsbedingungen zu bedingter Verzweigung hinzugefügt {#live-agent-availability-conditional-branching}

Zusätzlich zu nativen und benutzerdefinierten Marketo Engage-Feldern können Sie jetzt eine bedingte Verzweigung verwenden, um je nach Verfügbarkeit des Agenten Verzweigungen zu erstellen. Dies ist nützlich, wenn Sie Besuchern nur die Möglichkeit bieten möchten, mit einem Live Agent zu sprechen, wenn Live Agents verfügbar sind.

![](assets/dynamic-chat-release-1.png)

### Smart-List-Bedingung zur bedingten Verzweigung hinzugefügt {#smart-list-condition}

Durch Hinzufügen der neuen Smart-List-Bedingung von Marketo Engage in der bedingten Verzweigung können Sie Verzweigungen basierend auf bereits vorhandenen Zielgruppen erstellen, die Sie bereits in Marketo Engage erstellt haben, anstatt die Bedingungen für die Verzweigung von Zielgruppen in Dynamic Chat zu definieren.

![](assets/dynamic-chat-release-2.png)

### Bedingte Verzweigung für Konversationsflüsse {#conditional-branching-for-conversational-flows}

Wir haben in diesem Jahr bedingte Verzweigungen für Dialoge veröffentlicht, und jetzt können Sie auch die bedingte Verzweigung in Conversational Flows nutzen! Mit bedingter Verzweigung können Sie basierend auf verschiedenen Bedingungen Verzweigungen in Ihrem Fluss erstellen.

### Live-Chat für Konversationsflüsse {#live-chat-for-conversational-flows}

Im Jahr 2023 haben wir Live-Chat-Funktionen für Dialoge veröffentlicht. Jetzt können Sie auch Live-Chat-Interaktionen zu Ihren Gesprächsflüssen hinzufügen. Wenn Sie Konversationsflüsse mit Ihren Marketo Engage-Formularen verwenden, können Sie jetzt qualifizierten Besucherinnen und Besuchern erlauben, sofort nach der Formularübermittlung mit einem Live-Agenten zu chatten!

### Kürzliche Marketo Engage-Aktivitäten im Agenten-Posteingang {#recent-marketo-engage-activities-in-agent-inbox}

Wir haben dem Abschnitt Letzte Aktivitäten des Agenten-Posteingangs kürzlich Marketo Engage-Aktivitäten hinzugefügt. Wenn also ein Site-Besucher einen Chat mit einem Agenten anfordert, kann der Agent schnell sehen, ob der Besucher kürzlich eine der folgenden Marketo Engage-Aktivitäten ausgeführt hat (letzte 25 Aktivitäten):

* Hat E-Mail geöffnet
* Web-Seite besucht
* Ausgefülltes Formular
* Hatte interessanten Moment

![](assets/dynamic-chat-release-3.png)

### Kalenderverbindungsstatus in der Agentenverwaltung {#calendar-connection-status-in-agent-management}

Administratoren können jetzt leicht erkennen, welche Agenten mit Besprechungsbuchungsberechtigungen ihre Kalender in Dynamic Chat verbunden haben. Auf diese Weise können Sie sicherstellen, dass Ihr gesamtes Vertriebsteam verbunden ist und Besprechungsanfragen von Dynamic Chat akzeptiert.

![](assets/dynamic-chat-release-4.png)

### Einstellung „Mindest-Hinweis“ in der Agentenkalender-Konfiguration {#minimum-notice-setting-in-agent-calendar-configuration}

Benutzer berichteten, dass Web-Besucher Meetings in ihrem Kalender mit nur 10 Minuten Vorankündigung buchten. Daher haben wir in der Konfiguration des Agentenkalenders eine Mindestankündigungseinstellung eingeführt und die standardmäßige Vorlaufzeit auf 24 Stunden festgelegt.

![](assets/dynamic-chat-release-5.png)

### Aktualisiertes Benutzerverhalten hinzufügen/entfernen {#add-remove-user-behavior-updated}

Einige Benutzer gaben an, dass sie Probleme mit dem Hinzufügen und Entfernen von Agenten im dynamischen Chat haben. Daher haben wir einige Änderungen vorgenommen, um diese Probleme zu beheben.

Wenn ein(e) Benutzende(r) mit der Berechtigung Live-Chat oder Besprechungsbuchung zu Admin Console hinzugefügt wird, wird er/sie sofort in der Agentenverwaltungsliste angezeigt und kann zu Dialogen, Gesprächsflüssen, Routing-Regeln und Teams hinzugefügt werden.

Wenn ein(e) Benutzende(r) mit Berechtigungen zum Buchen von Meetings oder zum Live-Chat aus Admin Console entfernt wird, wird er/sie sofort aus Dynamic Chat entfernt, ist nicht mehr für den Live-Chat oder das Meeting-Routing verfügbar und wird nicht mehr auf die Lizenzbeschränkungen angerechnet.

### Verbesserte Berichtsleistung auf Konversationsebene {#improved-conversation-level-report-performance}

Die Berichte auf individueller Dialog- und Gesprächsebene sind jetzt leistungsfähiger und genauer. Zuvor dauerte das Laden von Dialogberichten mehrere Sekunden, und die Daten waren gelegentlich nicht mit den globalen Leistungsberichten konsistent. Jetzt werden Ihre individuellen Dialogberichte im Handumdrehen geladen und die Daten werden immer mit den globalen Berichtsdaten abgestimmt.

![](assets/dynamic-chat-release-6.png)

### Berechtigungsaktualisierungen {#permission-updates}

Die Berechtigungsstruktur und die Benennung in Adobe Admin Console wurden bereinigt, um die Berechtigungsverwaltung intuitiver zu gestalten.

* Die Kategorie „Konversationsverwaltung“ heißt jetzt „Konversationen“
* Die Kategorie „Meetings“ heißt jetzt „Aktivitäten“
* Die Kategorie „Agenteneinstellungen“ heißt jetzt „Agenten“
* Die Kategorie „Admin-Einstellungen“ heißt jetzt „Konfiguration“
* Die Kategorie „Live-Chat“ wurde entfernt und alle Live-Chat-Berechtigungen wurden in die Kategorie Agenten verschoben

![](assets/dynamic-chat-release-7.png)

### Unterstützung für Hyperlinks im Agenten-Posteingang {#support-for-hyperlinks-in-agent-inbox}

Wenn Live-Chat-Agenten jetzt URLs für Besucher im Chat freigeben, werden diese URLs mit Hyperlinks versehen, sodass Besucher einfach darauf klicken können, um zur Seite zu navigieren, anstatt die URL kopieren und in ihren Browser einfügen zu müssen.

### Aktualisiertes Schlüsselverhalten im Agenten-Posteingang eingeben {#enter-key-behavior-updated-in-agent-inbox}

Das Verhalten der Eingabetaste im Agenten-Posteingang wurde geändert. Wenn Sie die Eingabetaste drücken, wird die Nachricht gesendet, und durch Drücken von Umschalt+Eingabetaste wird ein Zeilenumbruch erstellt.

![](assets/dynamic-chat-release-8.png)

### Round-Robin-Seite entfernt {#round-robin-page-removed}

Keine Sorge! Das Round Robin Routing ist immer noch voll funktionsfähig und funktioniert genauso wie immer. Wir haben gerade die Seite entfernt, die eine oft ungenaue Liste von Agenten und ihre Reihenfolge in der Routing-Warteschlange der Round Robins zeigte.

Als wir Dynamic Chat im Jahr 2022 veröffentlichten, gab es keine Unterstützung für Live-Chat, sondern nur für die Besprechungsbuchung, und die Routing-Seite für Round Robin wurde nur mit Blick auf die Besprechungsbuchung entwickelt. Mit der Einführung des Live-Chats im letzten Jahr wurde die Round-Robin-Seite veraltet, da sie die komplexere Natur des Round-Robin-Routings zwischen Agenten mit sowohl Besprechungsbuchungs- als auch Live-Chat-Berechtigungen nicht genau widerspiegelt. Wir haben ein paar verschiedene Möglichkeiten untersucht, um das anzugehen, sind aber letztlich zu dem Schluss gekommen, dass die beste Möglichkeit, Verwirrung zu minimieren, darin besteht, es ganz zu beseitigen.

![](assets/dynamic-chat-release-9.png)

## Version Februar 2024 {#february-release}

**Versionsdatum: Freitag, 22. Februar 2024**

### Seite „Unterhaltungen“ {#conversations-page}

Die neue Seite Konversationen bietet eine zentrale Anlaufstelle, um Transkripte aller Konversationen (automatisiert und live) anzuzeigen, die für Ihre Instanz stattgefunden haben, und zwar sowohl von bekannten als auch von anonymen Leads. So erhalten Sie einen besseren Einblick in die Interaktion Ihrer Kunden mit Ihren Dialogen, Konversationsflüssen und Live-Agenten.

![](assets/dynamic-chat-release-10.png)

### Datumsbereich im globalen Dashboard wurde von 90 Tagen auf 24 Monate erhöht {#date-range-in-global-dashboard}

Du hast gefragt und wir haben geliefert. Sie können jetzt Dynamic Chat-Interaktionsdaten für bis zu zwei Jahre in allen Analytics-Dashboards sehen.

### Bedingte Verzweigung in Dialogfeldern {#conditional-branching-in-dialogues}

Mit bedingter Verzweigung können Sie basierend auf verschiedenen Bedingungen Verzweigungen in Ihren Dialogfeldflüssen erstellen. Jetzt können Sie verschiedene Inhalte basierend auf Lead- und Unternehmensattributen in Marketo Engage verschiedenen Personen im selben Dialogfeld präsentieren.

## Version Januar 2024 {#january-release}

**Versionsdatum: Donnerstag, 24. Januar 2024**

### Limit für gleichzeitigen Live-Chat in der Agentenverwaltung festgelegt {#Concurrent-live-chat-limit-setting}

Standardmäßig kann jeder Live-Chat-Agent in Ihrer Instanz maximal fünf Live-Chat-Sitzungen gleichzeitig durchführen. Wir haben eine neue Einstellung für die Agentenverwaltung eingeführt, mit der Sie diese Grenze von 1 bis 10 anpassen können.

![](assets/dynamic-chat-release-11.png)
