---
description: Agent-Posteingang - Marketo-Dokumente - Produktdokumentation
title: Agenten-Posteingang
feature: Dynamic Chat
exl-id: 65f13879-36d2-4a23-a029-271f5aea1229
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 2%

---

# Agenten-Posteingang {#agent-inbox}

Agenten können Live-Chats im Agenten-Posteingang abfragen. Zusätzlich zu den aktiven Unterhaltungen können sie vergangene Unterhaltungen, Besucherinformationen und mehr sehen.

![](assets/agent-inbox-1.png)

## Verfügbarkeits-Umschalter {#availability-toggle}

In der rechten oberen Ecke des Bildschirms Agentenposteingang haben Sie die Möglichkeit, Ihren Status als „Verfügbar“ oder „Nicht verfügbar“ festzulegen.

![](assets/agent-inbox-2.png)

>[!IMPORTANT]
>
>**Dadurch wird die** Live[Chat-Verfügbarkeit](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md#live-chat-availability){target="_blank"} überschrieben, die Sie in den Agenteneinstellungen festgelegt haben. Der Status bleibt erhalten, bis Sie ihn entweder zurückwechseln oder auf den nächsten Block Ihrer Verfügbarkeit wechseln.

>[!NOTE]
>
>Wenn Sie Ihren Status auf Nicht verfügbar setzen, wirkt sich dies nicht auf aktive Chats aus.

## Live-Chat-Benachrichtigungen {#live-chat-notifications}

Weitere Informationen zu Benachrichtigungen finden Sie in der [Live-Chat - Übersicht](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/live-chat-overview.md#live-chat-notifications){target="_blank"}.

## Konversationen {#conversations}

Auf der linken Seite des Bildschirms des Agenten-Posteingangs können Sie festlegen, ob nur die aktiven Unterhaltungen oder alle angezeigt werden sollen.

![](assets/agent-inbox-4.png)

>[!NOTE]
>
>Während Sie vergangene (inaktive) Unterhaltungen von sich selbst und anderen Agenten sehen können, können Sie nur Ihre eigenen aktiven Unterhaltungen sehen.

## Besucherinformationen {#visitor-information}

Auf der rechten Seite des Bildschirms des Agenten-Posteingangs sehen Sie (von oben nach unten) ihren Namen, ihre Stellenbezeichnung, ihre E-Mail-Adresse, ihre Telefonnummer und ihren CRM-Status. Alle nicht weitergegebenen Informationen werden als Bindestrich (-) angezeigt.

![](assets/agent-inbox-5.png)

## Beenden einer Sitzung {#end-a-session}

Agenten können eine Sitzung manuell beenden, indem sie einfach auf die Schaltfläche **Sitzung beenden** neben den Besucherinformationen klicken.

![](assets/agent-inbox-6.png)

## Tastaturbefehle {#shortcuts}

>[!NOTE]
>
>Diese Funktion ist Teil der generativen KI, die über das Dynamic Chat Prime-Abonnement verfügbar ist. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).

Shortcuts, unterstützt durch die generative AI [Response Library](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md), sind eine hervorragende Möglichkeit, während des Chats mit einem Besucher schnell Hilfe zu erhalten. Geben Sie einfach einen Schrägstrich (`/`) in das Textfeld ein und wählen Sie `ask` oder `search`.

![](assets/agent-inbox-7.png)

**Fragen** ist Hilfe bei Antworten auf eine Frage.

1. Geben Sie `/ask` in das Textfeld ein oder wählen Sie es aus. Geben Sie Ihre Frage ein und drücken Sie die Eingabetaste auf der Tastatur.

   ![](assets/agent-inbox-8.png)

1. Eine Antwort wird angezeigt. Klicken Sie auf das Kopiersymbol, um es in das Textfeld einfügen zu lassen. Sie können den Text bearbeiten, bevor Sie ihn an den Besucher senden.

   ![](assets/agent-inbox-9.png)

**Suche** dient der Hilfe bei der Suche nach Seiten, die sich auf einen bestimmten Text beziehen.

1. Geben Sie `/search` in das Textfeld ein oder wählen Sie es aus.

   ![](assets/agent-inbox-10.png)

1. Geben Sie ein, wonach Sie suchen möchten, und drücken Sie die Eingabetaste auf der Tastatur.

   ![](assets/agent-inbox-11.png)

1. Die entsprechenden Links werden angezeigt. Klicken Sie auf das Kopiersymbol, um sie in das Textfeld einfügen zu lassen. Sie können Änderungen vornehmen, bevor Sie die Informationen an den Besucher senden.

   ![](assets/agent-inbox-12.png)

## Aktivitätsverlauf {#activity-history}

Unter den Besucherinformationen finden Sie den Aktivitätsverlauf. Zeigen Sie Aktivitätstypen und -daten an und zeigen Sie sogar Chattranskripte an.

![](assets/agent-inbox-13.png)

>[!NOTE]
>
>Die Informationen werden nur für die letzten 90 Tage angezeigt.

## Kalenderfreigabe {#calendar-sharing}

Am unteren Rand des Live-Chat-Fensters befindet sich ein Symbol, mit dem Sie den Kalender Ihres oder eines anderen Agenten für den Chat-Besucher freigeben können.

1. Klicken Sie auf das Kalendersymbol.

   ![](assets/agent-inbox-14.png)

1. Wählen Sie den gewünschten Agentenkalender aus und klicken Sie auf **Senden**.

   ![](assets/agent-inbox-15.png)

1. Der Chat-Besucher kann ein Meeting buchen.

   ![](assets/agent-inbox-16.png)

## Zusammenfassung des Gesprächs {#conversation-summary}

>[!NOTE]
>
>Diese Funktion ist Teil der generativen KI, die über das Dynamic Chat Prime-Abonnement verfügbar ist. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).

Konversationszusammenfassung generiert eine schnelle Zusammenfassung für Sie in Echtzeit, einschließlich Themen, an denen der Besucher Interesse gezeigt hat. Er ist in der rechten unteren Ecke jedes Chatbildschirms verfügbar.

![](assets/agent-inbox-17.png)

>[!NOTE]
>
>Eine abgeschlossene Zusammenfassung einer Konversation finden Sie auch im Aktivitätsprotokoll des Personendatensatzes des Besuchers in Ihrer Marketo Engage-Datenbank.
