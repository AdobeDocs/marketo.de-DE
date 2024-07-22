---
description: Übersicht über den Verlauf von Konversationen - Marketo-Dokumente - Produktdokumentation
title: Übersicht über den Konversationsfluss
feature: Dynamic Chat
exl-id: c741886d-d672-471f-8902-208d25898afa
source-git-commit: 14ccfe39059b9c900a5e5e00b082146bb500d79d
workflow-type: tm+mt
source-wordcount: '339'
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
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Konversationaler Forms</a> in Marketo Engage wird von Konversationsflüssen angetrieben.</td>
  </tr>
 </tbody> 
</table>

## Designer-Registerkarte streamen {#stream-designer-tab}

Der Stream Designer for Conversational Flows ist fast identisch mit dem für Dialoge. [Hier erfahren Sie alles darüber](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"}.

![](assets/conversational-flow-overview-2.png)

## Registerkarte &quot;Berichte&quot; {#reports-tab}

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
>Siehe [Conversations SDK](https://experienceleague.adobe.com/tools/marketo-dynamic-chatbot/conversations-sdk/){target="_blank"} in Aktion!

>[!MORELIKETHIS]
>
>[Erstellen eines Konversationsflusses](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-conversational-flow.md){target="_blank"}
