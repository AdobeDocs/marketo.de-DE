---
unique-page-id: 2359947
description: Personen zwischen Interaktionsströmen wechseln - Marketo-Dokumente - Produktdokumentation
title: Personen zwischen Interaktionsströmen wechseln
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
feature: Engagement Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 1%

---

# Personen zwischen Interaktionsströmen wechseln {#transition-people-between-engagement-streams}

Interaktionsprogramme können mehr als einen Stream haben. Wenn Sie [einen Stream hinzufügen](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md), sollten Sie eine Möglichkeit definieren, wie Personen von einem Stream zum anderen wechseln können. Diese werden **Übergangsregeln“**

1. Navigieren Sie **[!UICONTROL Marketing-Aktivitäten]**.

   ![](assets/ma.png)

1. Wählen Sie Ihr Multi-Streaming-Interaktionsprogramm aus und navigieren Sie zu **[!UICONTROL Streams]**.

   ![](assets/multistream.jpg)

1. Klicken Sie **[!UICONTROL Übergangsregeln]** für den Stream, den Sie aus anderen Streams abrufen möchten, und klicken Sie dann auf **[!UICONTROL Übergangsregeln bearbeiten]**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >Übergangsregeln rufen einen Stream ab. Definieren Sie immer die Regeln für den Stream, in den Sie wechseln möchten.

   Sobald sich das Fenster für die Übergangsregel öffnet, suchen Sie den gewünschten Trigger und ziehen Sie ihn in den entsprechenden Bereich. In diesem Fall möchten wir Personen in das [!UICONTROL Mid-Stadium“ ], wenn es zu einer Opportunity hinzugefügt wird.

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. Stellen wir den Operator auf &quot;**[!UICONTROL &quot; ein]** damit die Benutzer für jede zusätzliche Möglichkeit zu ihm wechseln.

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >Sie können einer Übergangsregel mehrere Trigger und Filter hinzufügen, aber die Übergangsregel verwendet alle Filter (die einzige Option ist die Verwendung aller Filter). Wenn Sie ODER in einer Übergangsregel verwenden müssen, empfehlen wir, stattdessen eine externe intelligente Kampagne einzurichten.

1. Klicken Sie auf **[!UICONTROL Schließen]**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   Sehr gut! Jetzt wird jede Person in Ihrem Interaktionsprogramm, die zu einer Opportunity hinzugefügt wird, in den [!UICONTROL Mid-Stage]-Stream verschoben.

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >Die oben beschriebenen Schritte *tun* gelten auch für Personen[ die ](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md) anhalten.
