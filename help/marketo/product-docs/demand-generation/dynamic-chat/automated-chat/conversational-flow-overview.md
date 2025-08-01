---
description: Konversationsflussübersicht - Marketo-Dokumente - Produktdokumentation
title: Konversationsfluss - Übersicht
feature: Dynamic Chat
exl-id: c741886d-d672-471f-8902-208d25898afa
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Konversationsfluss - Übersicht {#conversational-flow-overview}

Konversationsfluss entwerfen und ihn für jeden Besucher auf der Grundlage einer bestimmten Aktion (z. B. Klicken auf eine call-to-action-Schaltfläche, beim Laden der Seite, auf der Seite verbrachte Zeit usw.) Trigger.

![](assets/conversational-flow-overview-1.png)

## Dialoge im Vergleich zu Gesprächsflüssen {#dialogues-vs-conversational-flows}

Dialogfelder und Konversationsflüsse weisen zwar einige Ähnlichkeiten auf, sind aber zwei separate Funktionen.

<table>
 <tbody>
  <tr>
   <th style="width:50%">Dialoge</th>
   <th style="width:50%">Konversationsflüsse</th>
  </tr>
  <tr>
   <td>Dialogfelder sind zielgerichtet: Sie entwerfen eine Konversation für eine bestimmte Seite und Zielgruppe basierend auf den von Ihnen implementierten Parametern.</td>
   <td>Konversationsflüsse werden ausgelöst - Sie entwerfen eine Konversation, die basierend auf der Aktion eines Besuchers ausgelöst werden kann, z. B. beim Ausfüllen eines Formulars, beim Klicken auf einen Link usw.</td>
  </tr>
   <tr>
   <td>Wird nur in der Chatbot-Oberfläche unterstützt.</td>
   <td>Derzeit in einer Popup-Oberfläche unterstützt, weitere Schnittstellen sind geplant.</td>
  </tr>
  </tr>
   <tr>
   <td>Für dasselbe Lead-Segment können mehrere Dialogfelder mit einer Prioritätsreihenfolge erstellt werden, sodass jeder Besucher das Dialogfeld nacheinander nach Priorität sieht, während er weiter interagiert.</td>
   <td>Konversationsflüsse haben keine Prioritätsreihenfolge und können beliebig oft durch denselben Lead ausgelöst werden, basierend auf der ermittelten call-to-action.</td>
  </tr>
  <tr>
   <td>Chatbot-Unterhaltungen basieren auf Dialogfeldern.</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Conversational Forms</a> in Marketo Engage basieren auf Conversational Flows.</td>
  </tr>
 </tbody>
</table>

## Registerkarte Designer streamen {#stream-designer-tab}

Die Stream-Designer für Konversationsflüsse ist fast identisch mit der für Dialoge. [Hier erfahren Sie alles darüber](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"}.

![](assets/conversational-flow-overview-2.png)

## Registerkarte „Berichte“ {#reports-tab}

Auf der Registerkarte Berichte können Sie Metriken zur Leistung Ihres Konversationsflusses anzeigen.

![](assets/conversational-flow-overview-3.png)

Interaktionsrate, Konversionsrate, Filterung nach bekannten und/oder unbekannten Besuchern und mehr anzeigen.

![](assets/conversational-flow-overview-4.png)

## Registerkarte „Einstellungen“ {#settings-tab}

![](assets/conversational-flow-overview-5.png)

In der oberen Hälfte der Registerkarte Einstellungen können Sie den Namen des Konversationsflusses aktualisieren, eine optionale Beschreibung hinzufügen und die Sprache ändern.

![](assets/conversational-flow-overview-6.png)

>[!NOTE]
>
>Wenn Sie eine andere Sprache auswählen, wird nur die Sprache des Systemtexts geändert. Sie sind für die Übersetzung von Inhalten verantwortlich.

### SDK-Unterhaltungen {#conversations-sdk}

Passen Sie in der unteren Hälfte der Registerkarte „Einstellungen“ den Konversations-Trigger an, der auch als Konversations-SDK bezeichnet wird. Sie können entscheiden, ob die Konversation auf Ihrer Website ausgelöst wird, wenn ein Besucher auf einen Link klickt, oder beim Laden der Seite.

![](assets/conversational-flow-overview-7.png)

>[!TIP]
>
>Sehen Sie [Konversationen SDK](https://experienceleague.adobe.com/tools/marketo-dynamic-chatbot/conversations-sdk/){target="_blank"} in Aktion!

>[!MORELIKETHIS]
>
>[Erstellen eines Konversationsflusses](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-conversational-flow.md){target="_blank"}
