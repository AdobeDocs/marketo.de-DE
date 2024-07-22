---
description: Callback-Funktionen - Marketo-Dokumente - Produktdokumentation
title: Callback-Funktionen
feature: Dynamic Chat
exl-id: 5ae7f6cb-5c57-4257-8a1a-992c9602cfaa
source-git-commit: f355022fb7e6f733bb7485229e395b0fe1a9818f
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 7%

---

# Callback-Funktionen {#callback-functions}

Sie können Dynamic Chat Widget-Callback-Funktionen verwenden, um Konversationsereignisse an Drittanbieterplattformen zu senden.

## Erste Schritte {#getting-started}

Dieses Ereignis gibt an, dass das Dynamic Chat-Widget einsatzbereit ist und ausgelöst wird, wenn alle Skripte, die sich auf Dynamic Chat beziehen, auf der Webseite geladen werden.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    // code here will execute when chatbot scripts are loaded in a webpage 
}); 
```

## Konversationsereignisse {#conversation-events}

Diese Ereignisse beziehen sich auf eine Konversation, die auf eine bestimmte Seite für einen bestimmten Besucher ausgerichtet ist.

### Ausgelöste Konversation

Eine Konversation (z. B. ein Dialogfeld), die für einen Website-Besucher angesprochen wird, wird aufgelöst und ihm der Chatbot angezeigt.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => { 
 // code here will execute when the chatbot is loaded for a visitor 
    }); 
});  
```

### Unterhaltung {#conversation-engaged}

Besucher interagiert (z. B. mit der ersten Antwort) mit dem Chatbot.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_ENGAGED, (event) => { 
 // code here will execute when a visitor engages with the chatbot 
     }); 
}); 
```

### Unterhaltung abgeschlossen {#conversation-completed}

Der Besucher hat das Ende der Konversation erreicht.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_COMPLETED, (event) => { 
 // code here will execute when a conversation is completed 
     }); 
}); 
```

### Unterhaltung geschlossen

Der Besucher hat die Konversation abgeschlossen, bevor er das Ende erreicht hat.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_CLOSED, (event) => { 
 // code here will execute when a conversation is closed 
    }); 
}); 
```

Der Parameter `event` ist ein Objekt mit Metadaten, die sich auf die Konversation beziehen. Sie können auf diese Metadaten zugreifen, indem Sie auf `event.data` zugreifen.

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
    <td>Konversationstyp (Dialog-/Konversationsfluss)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI-Typ (Popup/Chat-Bot/Inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>Sitzungs-ID</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## Besuchereingangsereignisse

Diese Ereignisse werden ausgelöst, wenn ein an einer Konversation beteiligter Besucher seine Kontaktinformationen (z. B. Telefonnummer oder E-Mail-Adresse) bereitstellt. Im Folgenden finden Sie die Ereignisse, die unter diese Kategorie fallen.

### Telefonnummer {#phone-number}

Dieses Ereignis wird ausgelöst, wenn ein Besucher während der Unterhaltung seine Telefonnummer angibt.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_INPUT_PHONE, (event) => { 
 // code here will execute when a visitor provides their phone number 
    }); 
});  
```

### E-Mail-ID {#email-id}

Dieses Ereignis wird ausgelöst, wenn ein Besucher während der Konversation seine E-Mail-Adresse angibt.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_INPUT_EMAIL, (event) => { 
 // code here will execute when a visitor provides their email address 
    }); 
}); 
```

Der Parameter `event` ist ein Objekt mit Metadaten, die sich auf die Konversation beziehen. Sie können auf diese Metadaten zugreifen, indem Sie auf `event.data` zugreifen.

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
    <td>Konversationstyp (Dialog-/Konversationsfluss)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI-Typ (Popup/Chat-Bot/Inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>Sitzungs-ID</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## Konferenzbuchungsereignisse {#meeting-booking-events}

Diese Ereignisse werden ausgelöst, wenn ein Besucher ein Treffen mit Ihrem Geschäftsvertreter bucht.

Im Folgenden finden Sie die Ereignisse, die unter diese Kategorie fallen.

### Besprechung gebucht {#meeting-booked}

Dieses Ereignis wird ausgelöst, wenn ein Besucher ein Meeting im Kalender eines Agenten bucht.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_MEETING_BOOKED, (event) => { 
 // code here will execute when a meeting is booked 
    }); 
}); 
```

Der Parameter `event` ist ein Objekt mit Metadaten, die sich auf die Konversation beziehen. Sie können auf diese Metadaten zugreifen, indem Sie auf `event.data` zugreifen.

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
    <td>Konversationstyp (Dialog-/Konversationsfluss)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI-Typ (Popup/Chat-Bot/Inline)</td>
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
    <td>Konferenzinformationen</td>
    <td>payload.meetingInfo</td>
  </tr>
</tbody>
</table>

## Live-Chat-Ereignisse {#live-chat-events}

Diese Ereignisse werden ausgelöst, wenn sich ein Besucher während seiner Interaktion mit dem Chatbot mit einem Live-Agenten verbindet.

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

### Live-Chat initiiert {#live-chat-initiated}

Dieses Ereignis wird ausgelöst, wenn ein Besucher die Option zum Chat mit einem Live-Agenten auswählt und ein Agent den Chat akzeptiert.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_INITIATED, (event) => { 
 // code here will execute after a live agent accepts the chat 
    }); 
}); 
```

### Live-Chat beendet {#live-chat-ended}

Dieses Ereignis wird ausgelöst, wenn eine Konversation zwischen einem Besucher und dem Live-Agenten beendet wird.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_ENDED, (event) => { 
 // code here will execute when a live chat is ended 
    }); 
}); 
```

### Live-Chat-Timeout {#live-chat-timeout}

Dieses Ereignis wird ausgelöst, wenn bei einer Live-Chat-Konversation eine Zeitüberschreitung auftritt, da der Besucher nicht mehr antwortet oder sie fallen gelassen wurden.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    const {addListener, Enum} = window.AdobeDX; 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUEST_TIMEOUT, (event) => { 
 // code here will execute when a visitor abandons a live chat 
    }); 
}); 
```

Der Parameter `event` ist ein Objekt mit Metadaten, die sich auf die Konversation beziehen. Sie können auf diese Metadaten zugreifen, indem Sie auf `event.data` zugreifen.

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
    <td>Konversationstyp (Dialog-/Konversationsfluss)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>UI-Typ (Popup/Chat-Bot/Inline)</td>
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

Wenn Sie eines dieser Ereignisse an eine Analytics-Plattform wie Adobe Analytics oder Google Analytics senden möchten, müssen Sie deren jeweiligen Tracking-Aufruf in diesen Dynamic Chat-Ereignissen hinzufügen. Es würde ungefähr wie im folgenden Beispiel aussehen.

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
