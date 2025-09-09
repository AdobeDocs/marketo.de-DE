---
description: Dynamic Chat-Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Dynamic Chat-Versionshinweise
feature: Release Information, Dynamic Chat
exl-id: 0447dc47-b9c5-42e1-8f66-73bf67c7871d
source-git-commit: 0c0dd3355f979577ec194f9e8f935615515905c0
workflow-type: tm+mt
source-wordcount: '3414'
ht-degree: 97%

---

# Dynamic Chat-Versionshinweise {#dynamic-chat-release}

Die Versionen von Adobe Dynamic Chat basieren auf einem Modell der kontinuierlichen Bereitstellung, das einen besser skalierbaren Ansatz für die Bereitstellung von Funktionen ermöglicht. Manchmal gibt es mehrere Versionen in einem Monat, schauen Sie daher regelmäßig nach den aktuellsten Informationen.

Die Standardseite mit den Versionshinweisen für Marketo Engage [finden Sie hier](/help/marketo/release-notes/current.md){target="_blank"}.

## Version Juni 2025 {#june-2025-release}

**Veröffentlichungsdatum: Dienstag, 30. Juni 2025**

### Überarbeitung der Routing-Logik {#routing-logic-revamp}

Die Routing-Logik des Live-Chats in Dynamic Chat wurde überarbeitet, um über alle Routing-Typen hinweg (Konto, benutzerdefiniert, Team und Round Robin) für ein intelligenteres und besser vorhersehbares Interaktionsverhalten zu sorgen. Die neue Logik vereinfacht Routing-Abläufe und verbessert Ausweichmöglichkeiten, wenn keine Agentinnen oder Agenten verfügbar sind.

#### Wichtige Verbesserungen im Routing-Verhalten

* **Bis zu zwei Interaktionsversuche pro Sitzung**

   * Das System versucht, eine Verbindung mit bis zu zwei Agentinnen oder Agenten herzustellen (maximal), jedoch ausschließlich innerhalb der primären Routing-Regel.

   * Wenn eine Agentin oder ein Agent verfügbar ist, aber nicht reagiert (z. B. den Chat ablehnt oder verpasst), versucht das System, eine Verbindung zu einer anderen Agentin oder einem anderen Agenten aus demselben Pool herzustellen.

   * Die Ausweichlogik (wie etwa Round Robin) wird nur aktiviert, wenn bei der ersten Auflösung keine geeigneten Agentinnen oder Agenten gefunden werden, jedoch nicht für ein erneutes Versuchen nach einer fehlgeschlagenen Interaktion.

* **Spezifisches Verhalten für eine Routing-Regel**

##### – Konto-Routing –

Wenn die E-Mail-Domain einer Besucherin oder eines Besuchers einem bekannten Konto zugeordnet ist, wird die als Agentin bzw. Agent zugeordnete Person immer priorisiert.

Wenn diese Person verfügbar ist, wird der Chat direkt an sie weitergeleitet.

Wenn sie nicht verfügbar ist, tut das System Folgendes:

* Versucht keinen anderen Agenten, auch wenn Round Robin als Ausweichlösung aktiviert ist.

* Stattdessen gilt Folgendes:

   * Es zeigt den Meeting-Kalender der als Agentin bzw. Agent zugeordneten Person an (falls aktiviert),
– oder –
   * Kehrt zu einer Standardmeldung zurück (im schlimmsten Fall).

Die Routing-Regel auf Kartenebene (z. B. Team, benutzerdefiniert) wird nur berücksichtigt, wenn das Konto-Routing nicht zulässig ist (keine übereinstimmende Domain oder Agentin bzw. Agent).

##### – Benutzerdefiniertes Routing/Team-Routing –

Diese Regeln können mehrere geeignete Agentinnen oder Agenten zurückgeben.

Wenn die erste als Agentin bzw. Agent verfügbare Person nicht interagiert, versucht das System eine weitere Person aus derselben Liste.

Nur weil eine Person nicht reagiert, wird nicht gleich ein Round-Robin-Fallback ausgelöst.

Wenn sich keine Agentin bzw. kein Agent meldet, passiert Folgendes:

* Das System zeigt den Kalender der ersten Person an, die als Agentin bzw. Agent angefragt wurde (falls aktiviert).
– oder –
* Es zeigt die standardmäßige Fallback-Nachricht an.

##### – Round-Robin-Routing –

Bei Verwendung als primäre Routing-Regel führt das System Folgendes durch:

* Es versucht, die erste als Agentin bzw. Agent verfügbare Person aus dem Round-Robin-Pool zu kontaktieren.

* Wenn die erste Person nicht antwortet, erfolgt ein erneuter Versuch mit der am nächstbesten geeigneten Person.

Wenn Round Robin als Fallback verwendet wird, wird es nur aktiviert, wenn von der primären Regel keine Agentinnen oder Agenten aufgelöst werden.

##### Besuchererlebnisfluss

Das System prüft, ob Konto-Routing anwendbar ist.

* Falls ja und wenn eine Agentin oder ein Agent verfügbar ist, wird sofort eine Verbindung hergestellt.

* Wenn die Person nicht geeignet oder nicht verfügbar ist, wird mit der Routing-Regel auf Kartenebene fortgefahren.

Die Routing-Regel auf Kartenebene (benutzerdefiniert, Team, Round Robin) wird ausgewertet.

* Geeignete Agentinnen und Agenten werden auf Verfügbarkeit geprüft (Berechtigungen, Status).

* Das System greift auf eine Agentin bzw. einen Agenten zu und versucht bei Bedarf eine zweite Person gemäß derselben Regel.

* Wenn keine Interaktion erfolgreich ist, wird eine Ausweichlogik angewendet:

   * Kalender-Fallback (falls aktiviert),
– oder –
   * Standardnachricht.

Round Robin wird als Ausweichlösung nur dann in Betracht gezogen, wenn keine geeigneten Agentinnen oder Agenten gemäß der primären Routing-Regel gefunden werden, aber nicht, wenn einzelne Agentinnen bzw. Agenten nicht reagieren.

##### Anwendungsszenarien

<p>

_&#x200B;**Konto-Routing**&#x200B;_

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Beispiel</th>
    <th>Ergebnis</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>Die Domain der Besucherin bzw. des Besuchers wird einem Konto zugeordnet. Für die als Agentin bzw. Agent zugeordnete Person ist der Live-Chat aktiviert und verfügbar.</td>
    <td>Der Chat stellt eine direkte Verbindung zur als Agentin bzw. Agent zugeordneten Person her.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Die als Agentin bzw. Agent zugeordnete Person ist nicht verfügbar, Round-Robin-Fallback ist aktiviert.</td>
    <td>Das System wählt eine als Agentin bzw. Agent verfügbare Person über Round Robin aus und bindet sie ein. </td>
  </tr>
  <tr>
    <td>Keine Fallback-Agentin bzw. kein Fallback-Agent</td>
    <td>Die als Agentin bzw. Agent zugeordnete Person ist nicht verfügbar, kein Round-Robin-Fallback; Meeting-Buchung ist aktiviert.</td>
    <td>Das System zeigt den Kalender der als Agentin bzw. Agent zugeordneten Person an oder eine standardmäßige Fallback-Nachricht an.</td>
  </tr>
</tbody></table>

_&#x200B;**Benutzerdefiniertes Routing**&#x200B;_

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Beispiel</th>
    <th>Ergebnis</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>Benutzerdefinierte Logik löst eine Liste von Agenten auf. Der erste Agent ist verfügbar und akzeptiert Chat.</td>
    <td>Chat stellt eine Verbindung zur ersten Agentin bzw. zum ersten Agenten her.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Benutzerdefinierte Regel löst keine Agentinnen und Agenten auf, Round-Robin-Fallback ist aktiviert.</td>
    <td>Das System wählt eine als Agentin bzw. Agent verfügbare Person über Round Robin aus und bindet sie ein.</td>
  </tr>
  <tr>
    <td>Keine Fallback-Agentin bzw. kein Fallback-Agent</td>
    <td>Zwei Agentinnen bzw. Agenten wurden aufgelöst. Keine der beiden Personen akzeptiert den Chat; Fallback wird auf den Meeting-Kalender festgelegt.</td>
    <td>Der Kalender des zuerst getesteten Agenten wird angezeigt oder die standardmäßige Fallback-Nachricht wird angezeigt.</td>
  </tr>
</tbody></table>

_&#x200B;**Team-Routing**&#x200B;_

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Beispiel</th>
    <th>Ergebnis</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>Das Team umfasst Agentinnen und Agenten mit Live-Chat. Die erste verfügbare Person akzeptiert den Chat.</td>
    <td>Chat stellt eine Verbindung zu dieser Agentin bzw. diesem Agenten her.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Es ist keine Team-Agentin bzw. kein Team-Agent verfügbar und Round-Robin-Fallback ist aktiviert.</td>
    <td>Das System wählt eine Person aus dem Round-Robin-Pool als Agentin bzw. Agenten aus und stellt eine Verbindung mit ihr her.</td>
  </tr>
  <tr>
    <td>Keine Fallback-Agentin bzw. kein Fallback-Agent</td>
    <td>Zwei Agentinnen bzw. Agenten verfügbar, aber keine der beiden Personen reagiert; Kalender-Fallback aktiviert.</td>
    <td>Der Kalender der zuerst als Agentin bzw. Agent versuchten Person wird angezeigt oder es wird eine Fallback-Nachricht ausgelöst.</td>
  </tr>
</tbody></table>

_&#x200B;**Round-Robin-Routing**&#x200B;_

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Beispiel</th>
    <th>Ergebnis</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>Round Robin Pool hat mehrere Agenten; der zweite Agent nimmt Chat an, nachdem der erste nicht.</td>
    <td>Chat stellt eine Verbindung zur zweiten Person her.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Im Round-Robin-Pool sind keine Agentinnen und Agenten verfügbar. Der Meeting-Kalender ist aktiviert.</td>
    <td>Der Kalender wird für den ersten Agenten in der Liste angezeigt (falls konfiguriert), oder die Fallback-Nachricht wird angezeigt.</td>
  </tr>
  <tr>
    <td>Keine Fallback-Agentin bzw. kein Fallback-Agent</td>
    <td>Keine verfügbaren Agentinnen und Agenten; Fallback ist deaktiviert.</td>
    <td>Der Besucherin bzw. dem Besucher wird eine statische Fallback-Nachricht angezeigt.</td>
  </tr>
</tbody></table>

### Pulse-Benachrichtigung {#pulse-notification}

Wenn eine Besucherin bzw. ein Besucher die Verbindung zu einer Agentin bzw. einem Agenten anfordert, stellen wir der Agentin bzw. dem Agenten eine In-App-Browser-Benachrichtigung bereit. Manchmal verpassen Agentinnen und Agenten diese Chats jedoch.

Mit dieser Version kann die Live-Agentin bzw. der Live-Agent eine E-Mail-, Slack-, In-App- und Browser-Benachrichtigung erhalten, wenn eine neue Besucherin bzw. ein neuer Besucher am Chat interessiert ist.

1. Klicken Sie auf Ihrer Adobe Experience Cloud-Homepage auf das Kontosymbol und wählen Sie **Einstellungen** aus.

   ![](assets/dynamic-chat-june-2025-release-1.png)

1. Scrollen Sie nach unten zu _Benachrichtigungen_ und treffen Sie die gewünschten Dynamic Chat-Auswahlen.

   ![](assets/dynamic-chat-june-2025-release-2.png)

>[!NOTE]
>
>Der Inhalt einer Pulse-Benachrichtigung kann mit dem identisch sein, den wir für In-App- und Browser-Benachrichtigungen verwenden.

## Version April/Mai 2025 {#apr-may-25-release}

### Benachrichtigungs-Sound {#message-notification-sound}

Jetzt haben Sie die Möglichkeit, jedes Mal, wenn der Chatbot in einer Sitzung ausgelöst wird, einen Ton für die Besucherin bzw. den Besucher zu aktivieren. Es stehen verschiedene Sounds zur Auswahl.

### Aktivieren von Erinnerungsnachrichten auf einem Mobilgerät {#enable-poke-messages-on-mobile}

Eine Erinnerungsnachricht („Poke“), die die Eröffnungsfrage neben dem Chat-Symbol anzeigt, ohne dass die Besucherin bzw. der Besucher darauf klicken muss, um den Chat zu sehen, kann jetzt für Personen, die ein Mobilgerät verwenden, aktiviert werden.

### Aktualisierung des Standard-Fallbacks {#default-fallback-update}

Bei benutzerdefinierten Regeln/Teams als Live-Chat-Karte: Wenn keine Agentinnen oder Agenten verfügbar sind (oder der Chat keine Verbindung herstellen kann), wird dies für verfügbare Agentinnen und Agenten (alle, die zu diesem Zeitpunkt verfügbar sind, unabhängig davon, welche Routing-Logik/Regel im Stream platziert wurde) auf Round Robin zurückgesetzt.

### Demandbase-Integration {#demandbase-integration}

Demandbase-Benutzende können Demandbase-Personenattribute für Dialog-Targeting, bedingtes Branding und benutzerdefiniertes Routing in Dynamic Chat verwenden.

## Version September/Oktober 2024 {#sep-oct-release}

### Erweiterte Live-Chat-Analyse {#enhanced-live-chat-analytics}

Das Analyse-Dashboard wurde u. a. in folgenden Punkten verbessert:

* Gesamtzahl der angeforderten Live-Chats: Anzahl der Besucherinnen und Besucher, die einen „Chat mit einer Agentin bzw. einem Agenten“ angefordert haben

* Gesamtzahl der verbundenen Live-Chats: Anzahl der verbundenen Besucherinnen und Besucher im Vergleich zur Gesamtzahl der Anforderungen für einen „Chat mit einer Agentin bzw. einem Agenten“

* Gesamtzahl der verpassten Live-Chat-Anfragen: Anzahl der nicht bedienten Besucherinnen und Besucher im Vergleich zur Gesamtzahl der Anfragen für einen „Chat mit einer Agentin bzw. einem Agenten“

* Durchschnittliche Chat-Länge in Minuten: Analysiert die „durchschnittliche Chat-Länge“ zwischen Besucherinnen und Besuchern und Ihren Agentinnen und Agenten

* Durchschnittliche Reaktionszeit von Agentinnen und Agenten in Sekunden: Analysiert die „durchschnittliche Zeit“, die Agentinnen und Agenten benötigen, um auf Fragen und Antworten im Live-Chat zu reagieren

* Tägliches Dashboard: erfolgreich verbundene Live-Chat-Anfragen, verpasste Live-Chat-Anfragen, Sortieren und Filtern der letzten Live-Chat-Aktivitäten

![](assets/dynamic-chat-sep-oct-2024-release-1.png)

### Konversationsbewertung {#conversation-scoring}

Quantifizieren Sie Ihre Leads basierend auf der Qualität ihrer Chat-Interaktion und verwenden Sie diese Metrik als Trigger/Filter in intelligenten Kampagnen mit Marketo Engage. Verwenden Sie das neue Attribut _Konversationsbewertung_ für die folgenden Aktivitäten:

* Hat einen Dialog geführt
* Hatte eine Interaktion mit einem Konversationsfluss
* Involviert mit einer Agentin oder einem Agenten

**Zu beachten:**

* Der Wert beträgt 0, 1, 2 oder 3 (der Standardwert ist null).

* Wenn die Konversation abgeschlossen oder abgebrochen wurde, kann der Scoring-Wert nicht mehr bearbeitet werden.

* So wird eine Bewertung festgelegt:

   * Im Posteingang der Agentin bzw. des Agenten – Während eines Live-Chats kann die Agentin bzw. der Agent einen Wert für die Konversation aktualisieren oder festlegen, der in der Konversationsaktivität gespeichert wird.

   * Im Stream-Designer – Auf der Zielkarte kann die Benutzerin bzw. der Benutzer einen Wert für die Konversation aktualisieren oder festlegen.

![](assets/dynamic-chat-sep-oct-2024-release-2.png)

![](assets/dynamic-chat-sep-oct-2024-release-3.png)

![](assets/dynamic-chat-sep-oct-2024-release-4.png)

### Neue Logik für die Lead-Erstellung {#new-lead-creation-logic}

Wenn ein Lead ein Formular mit der E-Mail-Adresse `abc@test.com` ausfüllt (wofür ein Cookie „xyz“ gesetzt wird) und später dann dasselbe Formular mit der E-Mail-Adresse `def@test.com` ausfüllt, wird ein neuer Personendatensatz erstellt. Das Cookie „xyz“ wird jedoch mit der neuen Person verknüpft und aus der Person `abc@test.com` entfernt.

Wenn also eine Besucherin bzw. ein Besucher mit dem Cookie „abc“ auf einer Seite landet und eine E-Mail-ID wie `abc@test.com` angibt:

<table><thead>
  <tr>
    <th>Besucherin bzw. Besucher</th>
    <th>Cookie</th>
    <th>Angegebene E-Mail-Adresse</th>
    <th>Erwartetes Verhalten</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Anonym</td>
    <td>abc</td>
    <td>Existiert nicht in der Datenbank</td>
    <td>Erstellen einer neuen Person</td>
  </tr>
  <tr>
    <td>Anonym</td>
    <td>abc</td>
    <td>Existiert in Datenbank</td>
    <td>Fusionieren der Person</td>
  </tr>
  <tr>
    <td>Anonym</td>
    <td>xyz</td>
    <td>Existiert in Datenbank</td>
    <td>Fusionieren der Person</td>
  </tr>
  <tr>
    <td>Bekannte Person</td>
    <td>abc</td>
    <td>Gleich wie vorhandene Person</td>
    <td>Aktualisieren der Person</td>
  </tr>
  <tr>
    <td>Bekannte Person</td>
    <td>abc</td>
    <td>Jemand anderes als die vorhandene Person</td>
    <td>Wenn bereits eine bekannte Person vorhanden ist, wird das Cookie übertragen und dieses Profil aufgelöst. Wenn keine Person mit dieser E-Mail-Adresse existiert, wird ein neuer Personendatensatz erstellt und das Cookie übertragen.</td>
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
    <td>Jemand anderes als die vorhandene Person</td>
    <td>Dieses Szenario ist nicht möglich, als wäre es ein neues Cookie von   Standard als neues anonymes Profil betrachtet</td>
  </tr>
</tbody></table>

### Option zum Übernehmen der Schriftart {#option-to-inherit-font}

Sie können den Chatbot jetzt so einstellen, dass er die Schriftart direkt von der Web-Seite übernimmt, auf der er gehostet wird, anstatt die Markenschriftart in Dynamic Chat zu verwalten. Wenn Sie diese Option aktivieren, übernimmt der Chatbot die Schriftart, die im Tag `<body>` der Seite definiert ist.

![](assets/dynamic-chat-sep-oct-2024-release-5.png)

### Demandbase-Integration mit Dynamic Chat {#demandbase-integration-with-dynamic-chat}

Demandbase-Benutzende können ihre eigene Lizenz von Demandbase mitbringen und die Integration aktivieren. Verwenden Sie Demandbase-Personenattribute für Dialog-Targeting, bedingtes Branding und benutzerdefiniertes Routing.

Die Auflösung dieser Attributwerte gegenüber einer Person erfolgt in Echtzeit und wird im jeweiligen Personenprofil gespeichert.

### Optimierte Ladezeit des Konversationsflusses {#optimized-conversation-flow-load-time}

Um das Kundenerlebnis zu verbessern, wird jetzt beim Laden des Konversationsflusses ein schimmernder Ladeanzeiger anstelle einer leeren Fläche angezeigt.

**Vorher**

![](assets/dynamic-chat-sep-oct-2024-release-6.png)

**Nachher**

![](assets/dynamic-chat-sep-oct-2024-release-7.gif)

## Version August 2024 {#august-release}

**Veröffentlichungsdatum: Samstag, 23. August 2024**

### Benutzerdefiniertes Formatieren Ihrer Konversationsnachrichten {#custom-format-conversation-messages}

Stream-Designer unterstützen jetzt das [Einfügen von HTML](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#create-a-stream){target="_blank"}, um das Look-and-Feel Ihrer Konversationen anzupassen.

![](assets/dynamic-chat-aug-2024-release-1.png)

### Chatbot nach unten scrollen {#chatbot-scroll-to-bottom}

Im Chatbot wurde ein Symbol hinzugefügt, über das Web-Besucherinnen und -Besucher direkt zur letzten Nachricht springen können. So können Besucherinnen und Besucher den Text durchscrollen, um schnell zur Konversation zurückzukehren.

![](assets/dynamic-chat-aug-2024-release-2.png)

### Zentrale Pulse-Benachrichtigungen {#core-pulse-notifications}

Benutzende erhalten jetzt eine [E-Mail-Benachrichtigung](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#failed-action-notifications){target="_blank"}, wenn eine Meeting-Buchung oder ein Live-Chat fehlschlägt.

![](assets/dynamic-chat-aug-2024-release-3.png)

### Unterstützung für mehrere Konversationen {#support-for-multiple-conversations}

Der Chatbot unterstützt jetzt mehrere Konversationen. Website-Besucherinnen und -Besucher können sich gleichzeitig an verschiedenen Konversationen auf verschiedenen Seiten beteiligen und zwischen ihnen wechseln.

![](assets/dynamic-chat-aug-2024-release-4.png)

### Standardsortierung für Inhalte {#default-sorting-for-content}

Standardmäßig werden Ihre Konversationsprotokolle, unbeantwortete Fragen und Fragengenerierungstabellen nach dem Erstellungsdatum (vom letzten zum ältesten) sortiert.

### Lead-Auflösung in Echtzeit {#real-time-lead-resolution}

Während einer Konversation mit einem anonymen Lead und einer angegebenen E-Mail-Adresse klären wir, ob ein bekannter Lead-Eintrag mit dieser E-Mail-Adresse vorhanden ist, und verwenden diesen Eintrag für Personalisierung in Echtzeit. Wenn wir mehrere Einträge finden, führen wir sie in Echtzeit zusammen. Dieses Verhalten ist sowohl für Dialogfelder als auch für Konversationsflüsse implementiert.

### Synchronisieren von Leads ohne Cookies von Marketo Engage {#syncing-leads-without-cookies}

Zuvor, wenn die Marketo Engage-Synchronisierung aktiviert wurde, synchronisierte Dynamic Chat ausschließlich bekannte Leads mit einer oder mehreren Cookie-IDs von Marketo Engage. Jetzt werden alle bekannten Leads (ob Cookie-ID vorhanden oder nicht) mit Dynamic Chat synchronisiert und können für die Personalisierung von Konversationen verwendet werden.

### Weitergeben zusätzlicher Besucherdaten an Konversationsflüsse {#pass-additional-visitor-data}

Wenn Sie Besucherdaten über andere Kanäle wie Formulare oder Anmeldungen erfassen, können Sie diese Daten jetzt direkt an Dynamic Chat übermitteln.

![](assets/dynamic-chat-aug-2024-release-5.png)

### Abgeleitete Daten aktualisiert {#refreshed-inferred-data}

Die meisten Konversationen auf einer Website werden mit anonymen Besucherinnen und Besuchern geführt. Sie können sie trotzdem über abgeleitete Daten ansprechen, wofür Besucher-IPs benötigt werden. Wir haben unsere IP-Datenbank und die entsprechenden abgeleiteten Daten aktualisiert, sodass jetzt viermal so viele IP-Adressen unterstützt werden.

### Sound zur Browser-Benachrichtigung für Agentinnen und Agenten hinzugefügt {#sound-added-to-agent-browser-notification}

Wenn ein Live-Chat einer Agentin oder einem Agenten zugewiesen wird, erhält diese Person eine Browser-Benachrichtigung. Aber gelegentlich sieht sie diese nicht. Darum haben wir einen [Benachrichtigungs-Sound](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#when-a-live-chat-is-routed-to-an-agent){target="_blank"} hinzugefügt, um ein Verpassen von Benachrichtigungen in Zukunft zu verhindern.

![](assets/dynamic-chat-aug-2024-release-6.png)

### Möglichkeit, ein Lead-Profil während des Live-Chats zu aktualisieren {#update-lead-profile-during-live-chat}

Bei einem Live-Chat möchten Agentinnen und Agenten Informationen über die Besucherin bzw. den Besucher erfassen und das jeweilige Profil aktualisieren. Es gibt jetzt eine Option, um Attributwerte von Lead- und Unternehmensobjekten zu aktualisieren.

![](assets/dynamic-chat-aug-2024-release-7.png)

## Version Juni 2024 {#june-release}

**Veröffentlichungsdatum: Freitag, 6. Juni 2024**

### Karte „Konversationsfluss“ {#conversational-flow-card}

Vereinfachen Sie in Ihren Dialogfeldern mehrere Schritte in einem Fluss, indem Sie die Karte „Konversationsfluss“ verwenden.

Beispiel: Wenn Ihr Ziel darin besteht, Registrierungen für Ihr Webinar über verschiedene Dialogfelder voranzubringen, müssten Sie denselben Fluss über alle Dialogfelder hinweg neu erstellen, die dieses Ziel haben. Und wenn Sie Details aktualisieren wollen, müssten Sie jedes einzelne Dialogfeld einzeln bearbeiten. Das ist dank der Karte „Konversationsfluss“ jetzt nicht mehr nötig.

Zusätzlich zur Neuverwendung von Flüssen über mehrere Dialogfelder hinweg können Sie denselben Übergangsfluss auch für Trigger über andere Kanäle (wie Formulare und Landingpages) verwenden.

![](assets/dynamic-chat-june-2024-release-1.png)

### Nutzungs-Limits {#usage-limits}

Die Seite „Nutzungs-Limits“ enthält wichtige Informationen wie Paketdetails und den Status Ihrer Nutzungs-Limits.

![](assets/dynamic-chat-june-2024-release-2.png)

## Version Mai 2024 {#may-release}

**Veröffentlichungsdatum: Donnerstag, 15. Mai 2024**

### Bibliothek mit vorab genehmigten Antworten {#pre-approved-response-library}

[Erstellen Sie eine vom Marketing genehmigte Bibliothek](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md){target="_blank"} mit KI-generierten Fragen und Antworten, um mit generativer KI in Minutenschnelle einen Chat einzurichten.

![](assets/dynamic-chat-may-2024-release-1.png)

### Unbeantwortete Fragen {#unanswered-questions}

[Verwenden Sie ein Repository mit unbeantworteten Fragen](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/unanswered-questions.md){target="_blank"} aus früheren Konversationen, um neue, vorab genehmigte Antworten zu generieren und eine Antwortbibliothek mit den neuesten Informationen zu verwalten.

![](assets/dynamic-chat-may-2024-release-2.png)

### Zusammenfassung von Konversationen {#conversation-summaries}

[Geben Sie Vertriebspersonal zusammengefasste Konversationen an die Hand](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#conversation-summary){target="_blank"}, einschließlich Einblicken in wichtige Diskussionsthemen, bevor Meetings stattfinden, um die Vorbereitungszeit zu verkürzen und das Vertriebspersonal besser mit aktuellen Informationen zu versorgen.

![](assets/dynamic-chat-may-2024-release-3.png)

### Vertriebs-Kurzbefehle für GenAI {#genai-sales-shortcuts}

[Bieten Sie Agentinnen und Agenten im Live-Chat schnellere Möglichkeiten](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#shortcuts){target="_blank"}, um auf KI-generierte Antworten zuzugreifen, vorhandene generierte Antworten zu bearbeiten und nach zusätzlichen Inhalten zu suchen, die während der Konversation an Kaufinteressierte gesendet werden können.

![](assets/dynamic-chat-may-2024-release-4.png)

### Hilfe bei Konversationen {#conversation-assist}

Helfen Sie Vertriebspersonal, bei Live-Konversationen mithilfe von Antworten, die vorab von Ihrem Marketing-Team genehmigt wurden, präzise zu reagieren.

### Konversations-Stupser {#conversation-nudges}

Bringen Sie Web-Besucher mit einem Handlungsaufruf dazu, Konversationen zum Abschluss zu bringen.

<p>

## Version April 2024 {#april-release}

**Veröffentlichungsdatum: Mittwoch, 23. April 2024**

### Konversationsflüsse sind jetzt für alle Benutzenden verfügbar {#conversational-flows-available-to-all-users}

Gestalten Sie Ihre Formulare und Landingpages dialogfähiger und verkürzen Sie den Vertriebstrichter, indem Sie qualifizierten Leads erlauben, sofort nach einer Formularübermittlung mit Konversationsformularen ein Meeting zu buchen oder mit dem Vertrieb zu chatten. Jetzt für alle Dynamic Chat-Benutzenden vollständig verfügbar&#42;.

_&#42;Zuvor als Testfunktion mit lebenslang 100 Interaktionen verfügbar. Interaktionen im Rahmen von Konversationsflüssen werden nun für Benutzende mit dem Select-Paket auf das monatliche Limit von 250 Interaktionen angerechnet._

### Rückruffunktionen {#callback-functions}

[Rückruffunktionen](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/callback-functions.md){target="_blank"} ermöglichen es Ihnen, Dynamic Chat-Analyseereignisse in externen Systemen wie Adobe Analytics oder Google Analytics zu erfassen, wenn Besuchende mit Dynamic Chat-Konversationen interagieren. Sie aktivieren Dynamic Chat-Analyseereignisse, indem Sie einen Rückruf bei der API registrieren, damit auf die Ereignisse gewartet wird. So erhalten Sie einen ganzheitlicheren Überblick über Ihre Dynamic Chat-Interaktion, was andere wichtige Daten wie Web-Traffic angeht.

### Verfügbarkeitsbedingungen von Live-Agentinnen und -Agenten zu bedingter Verzweigung hinzugefügt {#live-agent-availability-conditional-branching}

Zusätzlich zu nativen und benutzerdefinierten Marketo Engage-Feldern können Sie jetzt eine bedingte Verzweigung nutzen, um je nach Verfügbarkeit der Agentinnen und Agenten Verzweigungen zu erstellen. Dies ist nützlich, wenn Sie Besuchenden nur dann die Möglichkeit bieten möchten, mit einer Live-Agentin oder einem Live-Agenten zu sprechen, wenn solche verfügbar sind.

![](assets/dynamic-chat-release-1.png)

### Bedingung für intelligente Liste zu bedingter Verzweigung hinzugefügt {#smart-list-condition}

Durch Hinzufügen der neuen Bedingung für intelligente Listen von Marketo Engage in der bedingten Verzweigung können Sie Verzweigungen anhand von bereits vorhandenen Zielgruppen einrichten, die Sie bereits in Marketo Engage erstellt haben, anstatt die Verzweigungsbedingungen für Zielgruppen in Dynamic Chat zu definieren.

![](assets/dynamic-chat-release-2.png)

### Bedingte Verzweigung für Konversationsflüsse {#conditional-branching-for-conversational-flows}

Wir haben in diesem Jahr eine bedingte Verzweigung für Dialoge veröffentlicht. Jetzt können Sie bedingte Verzweigung auch in Konversationsflüssen nutzen! Mit bedingten Verzweigungen können Sie in Ihrem Fluss Verzweigungen anhand verschiedener Bedingungen erstellen.

### Live-Chat für Konversationsflüsse {#live-chat-for-conversational-flows}

Im Jahr 2023 haben wir Live-Chat-Funktionen für Dialoge veröffentlicht. Jetzt können Sie auch Live-Chat-Interaktionen zu Ihren Konversationsflüssen hinzufügen. Wenn Sie Konversationsflüsse mit Ihren Marketo Engage-Formularen verwenden, können Sie qualifizierten Besuchenden jetzt erlauben, sofort nach der Formularübermittlung mit einer Live-Agentin oder einem Live-Agenten zu chatten!

### Kürzliche Marketo Engage-Aktivitäten im Agenten-Posteingang {#recent-marketo-engage-activities-in-agent-inbox}

Wir haben dem Abschnitt „Letzte Aktivitäten“ des Agenten-Posteingangs kürzlich Marketo Engage-Aktivitäten hinzugefügt. Wenn also eine Besucherin oder ein Besucher der Site einen Chat mit einer Agentin oder einem Agenten anfordert, können letztere schnell sehen, ob die Person kürzlich eine der folgenden Marketo Engage-Aktivitäten ausgeführt hat (letzte 25 Aktivitäten):

* Hat E-Mail geöffnet
* Hat Web-Seite besucht
* Hat Formular ausgefüllt
* Hatte interessanten Moment

![](assets/dynamic-chat-release-3.png)

### Kalenderverbindungsstatus in der Agenten-Verwaltung {#calendar-connection-status-in-agent-management}

Admins können jetzt leicht erkennen, welche Agentinnen und Agenten mit Berechtigungen zur Meeting-Buchung ihre Kalender in Dynamic Chat verknüpft haben. So können Sie sicherstellen, dass Ihr gesamtes Vertriebs-Team untereinander vernetzt ist und Meeting-Anfragen von Dynamic Chat akzeptiert.

![](assets/dynamic-chat-release-4.png)

### Einstellung „Mindestankündigung“ in der Konfiguration des Agentenkalenders {#minimum-notice-setting-in-agent-calendar-configuration}

Benutzende berichteten, dass manche Web-Besucherinnen und -Besucher Meetings in ihrem Kalender mit nur 10 Minuten Vorankündigung buchten. Daher haben wir in der Konfiguration des Agentenkalenders eine Einstellung für eine Mindestankündigungszeit eingeführt und die standardmäßige Vorlaufzeit auf 24 Stunden festgelegt.

![](assets/dynamic-chat-release-5.png)

### Hinzufügen/Entfernen von Benutzerverhalten aktualisiert {#add-remove-user-behavior-updated}

Einige Benutzende gaben an, dass sie Probleme mit dem Hinzufügen und Entfernen von Agentinnen und Agenten im dynamischen Chat hatten. Daher haben wir einige Änderungen vorgenommen, um diese Probleme zu beheben.

Wenn eine Benutzerin oder ein Benutzer mit der Berechtigung zur Meeting-Buchung oder zum Live-Chat zur Admin Console hinzugefügt wird, wird diese Person sofort in der Agenten-Verwaltungsliste angezeigt und kann zu Dialogen, Konversationsflüssen, Routing-Regeln und Teams hinzugefügt werden.

Wenn eine Benutzerin oder ein Benutzer mit Berechtigungen zur Meeting-Buchung oder zum Live-Chat aus der Admin Console entfernt wird, wird diese Person sofort aus Dynamic Chat entfernt, ist nicht mehr für den Live-Chat oder das Routing von Meetings verfügbar und wird nicht mehr auf die Lizenzbeschränkungen angerechnet.

### Verbesserte Leistung von Berichten auf Konversationsebene {#improved-conversation-level-report-performance}

Berichte auf individueller Dialog- und Konversationsflussebene sind jetzt leistungsfähiger und genauer. Zuvor dauerte das Laden von Dialogberichten mehrere Sekunden, und die Daten waren gelegentlich nicht mit globalen Leistungsberichten konsistent. Jetzt werden Ihre individuellen Dialogberichte im Handumdrehen geladen und die Daten immer mit globalen Berichtsdaten abgestimmt.

![](assets/dynamic-chat-release-6.png)

### Berechtigungsaktualisierungen {#permission-updates}

Die Berechtigungsstruktur und die Benennungen in Adobe Admin Console wurden bereinigt, um die Berechtigungsverwaltung intuitiver zu gestalten.

* Die Kategorie „Konversationsverwaltung“ heißt jetzt „Konversationen“
* Die Kategorie „Meetings“ heißt jetzt „Aktivitäten“
* Die Kategorie „Agenteneinstellungen“ heißt jetzt „Agentinnen und Agenten“
* Die Kategorie „Admin-Einstellungen“ heißt jetzt „Konfiguration“
* Die Kategorie „Live-Chat“ wurde entfernt und alle Live-Chat-Berechtigungen wurden in die Kategorie „Agentinnen und Agenten“ verschoben

![](assets/dynamic-chat-release-7.png)

### Unterstützung für Hyperlinks im Agenten-Posteingang {#support-for-hyperlinks-in-agent-inbox}

Wenn Live-Chat-Agentinnen und -Agenten jetzt URLs für Besuchende im Chat freigeben, werden diese URLs mit Hyperlinks versehen, sodass Benutzende einfach darauf klicken können, um zur Seite zu navigieren, anstatt die URL kopieren und in den Browser einfügen zu müssen.

### Verhalten der Eingabetaste im Agent-Posteingang aktualisiert {#enter-key-behavior-updated-in-agent-inbox}

Das Verhalten der Eingabetaste im Agenten-Posteingang wurde geändert. Beim Drücken der Eingabetaste wird nun die Nachricht gesendet, und durch Drücken von Umschalt+Eingabetaste wird ein Zeilenumbruch erstellt.

![](assets/dynamic-chat-release-8.png)

### Round-Robin-Seite entfernt {#round-robin-page-removed}

Keine Sorge! Das Round-Robin-Routing ist weiterhin voll funktionsfähig und läuft genauso wie immer ab. Wir haben lediglich die Seite entfernt, die eine oft ungenaue Liste der Agentinnen und Agenten und ihre Reihenfolge in der Warteschlange für das Round-Robin-Routing zeigte.

Als wir Dynamic Chat im Jahr 2022 veröffentlicht haben, gab es noch keine Unterstützung für Live-Chat, sondern nur für die Meeting-Buchung. Die Seite für Round-Robin-Routing wurde nur mit Blick auf die Meeting-Buchung entwickelt. Mit der Einführung des Live-Chats im letzten Jahr wurde die Round-Robin-Seite hinfällig, da sie die komplexere Natur des Round-Robin-Routings zwischen Agentinnen und Agenten, die sowohl über Meeting-Buchungs- als auch über Live-Chat-Berechtigungen verfügen, nicht genau widerspiegelte. Wir haben uns verschiedene Optionen angesehen, um das anzugehen, sind aber letztlich zu dem Schluss gekommen, dass die beste Möglichkeit, Verwirrung zu vermeiden, darin bestand, die Seite ganz zu beseitigen.

![](assets/dynamic-chat-release-9.png)

## Version Februar 2024 {#february-release}

**Versionsdatum: Freitag, 22. Februar 2024**

### Seite „Konversationen“ {#conversations-page}

Die neue Seite „Konversationen“ dient als zentrale Anlaufstelle zur Anzeige von Transkripten aller Konversationen (automatisiert und live), die für Ihre Instanz stattgefunden haben, und zwar sowohl von bekannten als auch von anonymen Leads. So erhalten Sie einen besseren Einblick darin, wie Kundschaft mit Ihren Dialogen, Konversationsflüssen und Live-Agentinnen bzw. -Agenten interagiert.

![](assets/dynamic-chat-release-10.png)

### Datumsbereich im globalen Dashboard von 90 Tagen auf 24 Monate erhöht {#date-range-in-global-dashboard}

Sie haben darum gebeten – und wir haben geliefert. Sie können jetzt in allen Analytics-Dashboards Daten von Dynamic Chat-Interaktionen für bis zu zwei Jahre anzeigen.

### Bedingte Verzweigungen in Dialogen {#conditional-branching-in-dialogues}

Mit bedingten Verzweigungen können Sie anhand verschiedener Bedingungen Verzweigungen in Ihren Dialogflüssen erstellen. Nun können Sie in Marketo Engage je nach Lead- und Unternehmensattributen verschiedene Inhalte verschiedenen Personen im selben Dialog präsentieren.

## Version Januar 2024 {#january-release}

**Versionsdatum: Donnerstag, 24. Januar 2024**

### Limit für gleichzeitige Live-Chats in der Agenten-Verwaltung festgelegt {#Concurrent-live-chat-limit-setting}

Standardmäßig kann jede Live-Chat-Agentin bzw. jeder Live-Agent in Ihrer Instanz maximal 5 Live-Chat-Sitzungen gleichzeitig durchführen. Wir haben eine neue Einstellung für die Agenten-Verwaltung eingeführt, mit der Sie dieses Limit auf einen Wert von 1 bis 10 anpassen können.

![](assets/dynamic-chat-release-11.png)
