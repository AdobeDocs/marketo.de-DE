---
description: Übersicht über den Verlauf von Konversationen - Marketo-Dokumente - Produktdokumentation
title: Übersicht über den Konversationsfluss
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 2f5b79e9fb0340dd1ed65b00f2ec3ac487b7b7ca
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Übersicht über den Konversationsfluss {#conversational-flow-overview}

Gestalten Sie einen Konversationsfluss und weisen Sie ihn jedem Trigger basierend auf einer bestimmten Aktion zu (z. B. Klicken auf eine Aktionsaufruf-Schaltfläche, beim Laden der Seite, Besuchszeit pro Seite usw.).

![](assets/conversational-flow-overview-1.png)

## Dialoge im Vergleich zu konversativen Flüssen {#dialogues-vs-conversational-flows}

Dialoge und Konversationsflüsse weisen zwar mehrere Ähnlichkeiten auf, sind aber zwei separate Funktionen.

<table> 
 <tbody> 
  <tr> 
   <th style="width:50%">Dialoge</th> 
   <th style="width:50%">Konversationsflüsse</th>
  </tr> 
  <tr> 
   <td>Dialogfelder werden als Zielgruppe ausgewählt - Sie gestalten eine Konversation für eine bestimmte Seite und Zielgruppe basierend auf den von Ihnen implementierten Parametern.</td> 
   <td>Konversationsflüsse werden ausgelöst - Sie gestalten eine Konversation, die basierend auf der Aktion eines Besuchers ausgelöst werden kann, z. B. das Ausfüllen eines Formulars, das Klicken auf einen Link usw.</td>
  </tr>
   <tr> 
   <td>Wird nur in der Chatbot-Oberfläche unterstützt.</td> 
   <td>Aktuell in einer Popup-Oberfläche unterstützt, für die weitere Schnittstellen geplant sind.</td>
  </tr>
  </tr>
   <tr> 
   <td>Für dasselbe Lead-Segment können mehrere Dialogfelder mit einer Prioritätsreihenfolge erstellt werden, sodass jeder Besucher das Dialogfeld nach Priorität sieht, während er weiterhin interagiert.</td> 
   <td>Konversationsflüsse haben keine Prioritätsreihenfolge und können basierend auf dem festgelegten Aktionsaufruf beliebig oft durch denselben Lead ausgelöst werden.</td>
  </tr>
  <tr>
   <td>Chatbot-Konversationen werden durch Dialoge unterstützt.</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat-two/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Conversation Forms</a> in Marketo Engage werden von Konversationsflüssen angetrieben.</td>
  </tr>
 </tbody> 
</table>

## Registerkarte &quot;Stream-Designer&quot; {#stream-designer-tab}

Der Stream-Designer für Konversationsflüsse ist fast identisch mit dem für Dialogfelder. [Hier erfahren Sie alles darüber.](/help/marketo/product-docs/demand-generation/dynamic-chat-two/automated-chat/stream-designer.md){target="_blank"}.

![](assets/conversational-flow-overview-2.png)

## Tab Berichte {#reports-tab}

Auf der Registerkarte Berichte können Sie Metriken zur Leistung Ihres Konversionsflusses anzeigen.

![](assets/conversational-flow-overview-3.png)

Anzeigen von Interaktionsrate, Konversionsrate, Filtern nach bekannten und/oder unbekannten Besuchern und mehr.

![](assets/conversational-flow-overview-4.png)

## Registerkarte &quot;Einstellungen&quot; {#settings-tab}

![](assets/conversational-flow-overview-5.png)

In der oberen Hälfte der Registerkarte Einstellungen können Sie den Namen des Konversionsflusses aktualisieren, eine optionale Beschreibung hinzufügen und die Sprache ändern.

![](assets/conversational-flow-overview-6.png)

>[!NOTE]
>
>Wenn Sie eine andere Sprache auswählen, wird nur die Sprache des Systemtextes geändert. Sie sind für die Übersetzung von Inhalten verantwortlich.

### Konversations-SDK {#conversations-sdk}

Passen Sie in der unteren Hälfte der Registerkarte Einstellungen den Trigger Konversation (auch als Conversations SDK bezeichnet) an. Sie können entscheiden, ob die Konversation auf Ihrer Website ausgelöst wird, wenn ein Besucher auf einen Link klickt, oder ob sie beim Laden der Seite aufgerufen wird.

![](assets/conversational-flow-overview-7.png)

>[!TIP]
>
>Siehe [Konversations-SDK](https://experienceleague.adobe.com/tools/marketo-dynamic-chatbot/conversations-sdk/){target="_blank"} in Aktion!

>[!MORELIKETHIS]
>
>[Konversationsfluss erstellen](/help/marketo/product-docs/demand-generation/dynamic-chat-two/automated-chat/create-a-conversational-flow.md){target="_blank"}