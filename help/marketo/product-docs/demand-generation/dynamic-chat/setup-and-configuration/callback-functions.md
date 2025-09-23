---
description: Rückruffunktionen - Marketo-Dokumente - Produktdokumentation
title: Rückruffunktionen
feature: Dynamic Chat
exl-id: 5ae7f6cb-5c57-4257-8a1a-992c9602cfaa
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 8%

---

# Rückruffunktionen {#callback-functions}

Sie können Rückruffunktionen von Dynamic Chat-Widgets verwenden, um Konversationsereignisse an beliebige Drittanbieterplattformen zu senden.

## Erste Schritte {#getting-started}

Dieses Ereignis zeigt an, dass das Dynamic Chat-Widget einsatzbereit ist und ausgelöst wird, wenn alle Skripte, die sich auf Dynamic Chat beziehen, auf der Web-Seite geladen werden.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    // code here will execute when chatbot scripts are loaded in a webpage
});
```

## Konversationsereignisse {#conversation-events}

Diese Ereignisse stehen im Zusammenhang mit einer Konversation, die auf einer bestimmten Seite für einen bestimmten Besucher stattfindet.

### Konversation ausgelöst

Ein Gespräch (z. B. ein Dialogfeld), das für einen Website-Besucher vorgesehen ist, wird aufgelöst und ihm der Chatbot angezeigt.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => {
 // code here will execute when the chatbot is loaded for a visitor
    });
});
```

### Unterhaltung eingestellt {#conversation-engaged}

Der Besucher interagierte (z. B. mit seiner ersten Antwort) mit dem Chatbot.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_ENGAGED, (event) => {
 // code here will execute when a visitor engages with the chatbot
     });
});
```

### Konversation abgeschlossen {#conversation-completed}

Der Besucher hat das Ende des Gesprächs erreicht.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_COMPLETED, (event) => {
 // code here will execute when a conversation is completed
     });
});
```

### Unterhaltung geschlossen

Der Besucher hat das Gespräch geschlossen, bevor er das Ende erreicht.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_CLOSED, (event) => {
 // code here will execute when a conversation is closed
    });
});
```

Der `event` ist ein Objekt mit Metadaten, die sich auf die Konversation beziehen. Sie können auf diese Metadaten zugreifen, indem Sie `event.data`.

Im Folgenden finden Sie einige wichtige Metadatenwerte, auf die Sie zugreifen können:

<table>
<thead>
  <tr>
    <th style="width:75%">Metadaten</th>
    <th style="width:25%">Attribute</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Konversationsname</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Gesprächs-ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Unterhaltungstyp (Dialogfeld/Unterhaltungsfluss)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI-Typ (Popup/Chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>Sitzungs-ID</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## Besuchereingabeereignisse

Diese Ereignisse werden ausgelöst, wenn ein Besucher, der an einem Gespräch teilnimmt, seine Kontaktinformationen (z. B. Telefonnummer oder E-Mail-Adresse) bereitstellt. Im Folgenden finden Sie die Ereignisse, die unter diese Kategorie fallen.

### Telefonnummer {#phone-number}

Dieses Ereignis wird ausgelöst, wenn ein Besucher während des Gesprächs seine Telefonnummer angibt.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_INPUT_PHONE, (event) => {
 // code here will execute when a visitor provides their phone number
    });
});
```

### E-Mail-ID {#email-id}

Dieses Ereignis wird ausgelöst, wenn ein Besucher während des Gesprächs seine E-Mail-Adresse angibt.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_INPUT_EMAIL, (event) => {
 // code here will execute when a visitor provides their email address
    });
});
```

Der `event` ist ein Objekt mit Metadaten, die sich auf die Konversation beziehen. Sie können auf diese Metadaten zugreifen, indem Sie `event.data`.

Im Folgenden finden Sie einige wichtige Metadatenwerte, auf die Sie zugreifen können:

<table>
<thead>
  <tr>
    <th style="width:75%">Metadaten</th>
    <th style="width:25%">Attribute</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Konversationsname</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Gesprächs-ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Unterhaltungstyp (Dialogfeld/Unterhaltungsfluss)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI-Typ (Popup/Chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>Sitzungs-ID</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## Besprechungsbuchungsereignisse {#meeting-booking-events}

Diese Ereignisse werden ausgelöst, wenn ein Besucher ein Meeting mit Ihrem Unternehmensvertreter bucht.

Im Folgenden finden Sie die Ereignisse, die unter diese Kategorie fallen.

### Besprechung gebucht {#meeting-booked}

Dieses Ereignis wird ausgelöst, wenn ein Besucher ein Meeting über den Kalender eines Agenten bucht.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_MEETING_BOOKED, (event) => {
 // code here will execute when a meeting is booked
    });
});
```

Der `event` ist ein Objekt mit Metadaten, die sich auf die Konversation beziehen. Sie können auf diese Metadaten zugreifen, indem Sie `event.data`.

Im Folgenden finden Sie einige wichtige Metadatenwerte, auf die Sie zugreifen können:

<table>
<thead>
  <tr>
    <th style="width:75%">Metadaten</th>
    <th style="width:25%">Attribute</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Konversationsname</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Gesprächs-ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Unterhaltungstyp (Dialogfeld/Unterhaltungsfluss)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI-Typ (Popup/Chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>Sitzungs-ID</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>Agentenname </td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>Agenten-ID</td>
    <td>payload.agentID</td>
  </tr>
  <tr>
    <td>Besprechungsinformationen</td>
    <td>payload.meetingInfo</td>
  </tr>
</tbody>
</table>

## Live-Chat-Ereignisse {#live-chat-events}

Diese Ereignisse werden ausgelöst, wenn ein Besucher während seiner Interaktion mit dem Chatbot eine Verbindung zu einem Live-Agenten herstellt.

Im Folgenden finden Sie die Ereignisse, die unter diese Kategorie fallen.

### Live-Chat angefordert {#live-chat-requested}

Dieses Ereignis wird ausgelöst, wenn ein Besucher die Option zum Chat mit einem Live-Agenten auswählt und ein verfügbarer Agent aufgelöst wird.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUESTED, (event) => {
 // code here will execute when a visitor requests a live chat
    });
});
```

### Live-Chat gestartet {#live-chat-initiated}

Dieses Ereignis wird ausgelöst, wenn ein Besucher die Option auswählt, mit einem Live-Agenten zu chatten, und ein Agent den Chat akzeptiert.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_INITIATED, (event) => {
 // code here will execute after a live agent accepts the chat
    });
});
```

### Live-Chat beendet {#live-chat-ended}

Dieses Ereignis wird ausgelöst, wenn eine Konversation zwischen einem Besucher und dem Live Agent beendet wird.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_ENDED, (event) => {
 // code here will execute when a live chat is ended
    });
});
```

### Live-Chat-Zeitüberschreitung {#live-chat-timeout}

Dieses Ereignis wird ausgelöst, wenn ein Live-Chat-Gespräch die zulässige Zeit überschreitet, da der Besucher nicht mehr reagiert oder ihn fallen gelassen hat.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUEST_TIMEOUT, (event) => {
 // code here will execute when a visitor abandons a live chat
    });
});
```

Der `event` ist ein Objekt mit Metadaten, die sich auf die Konversation beziehen. Sie können auf diese Metadaten zugreifen, indem Sie `event.data`.

Im Folgenden finden Sie einige wichtige Metadatenwerte, auf die Sie zugreifen können:

<table>
<thead>
  <tr>
    <th style="width:75%">Metadaten</th>
    <th style="width:25%">Attribute</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Konversationsname</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Gesprächs-ID</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Unterhaltungstyp (Dialogfeld/Unterhaltungsfluss)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI-Typ (Popup/Chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>Sitzungs-ID</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>Agentenname </td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>Agenten-ID</td>
    <td>payload.agentID</td>
  </tr>
</tbody>
</table>

Wenn Sie eines dieser Ereignisse an eine Analyseplattform wie Adobe Analytics oder Google Analytics senden möchten, müssen Sie den entsprechenden Tracking-Aufruf innerhalb dieser Dynamic Chat-Ereignisse hinzufügen. Dies würde in etwa wie im folgenden Beispiel aussehen.

```javascript
window.addEventListener('adobedx.conversations.ready', () => {
    const {addListener, Enum} = window.AdobeDX;
    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => {
 // Enter Adobe Analytics or Google Analytics function here
    ga('send', 'event', {
      eventCategory: Dynamic Chat Conversations',
      eventAction: 'Conversation Triggered',
      eventLabel: event.data.payload.id,
    });
    });
});
```
