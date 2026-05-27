---
unique-page-id: 2359947
description: Erfahren Sie, wie Sie Übergangsregeln einrichten, um Personen zwischen Interaktionsströmen zu bewegen. Definieren Sie Regeln für den Stream, in den Sie Daten übertragen möchten.
title: Transferieren von Personen zwischen Interaktionsströmen
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
feature: Engagement Programs
TQID: https://experienceleague.adobe.com/viGLYAkvGqF-9K5bhAHWDSOMYaiBuKRe8F2QginuYps
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 243
ht-degree: 6%

---

# Transferieren von Personen zwischen Interaktionsströmen {#transition-people-between-engagement-streams}

Interaktionsprogramme können mehr als einen Stream haben. Wenn Sie [einen Stream hinzufügen](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md) definieren Sie eine Möglichkeit für Personen, von einem Stream zum anderen zu wechseln. Diese werden **Übergangsregeln“**

1. Navigieren Sie zu **[!UICONTROL Marketing-Aktivitäten]**.

   ![](assets/ma.png)

1. Wählen Sie Ihr Multi-Streaming-Interaktionsprogramm aus und navigieren Sie zu **[!UICONTROL Streams]**.

   ![](assets/multistream.jpg)

1. Klicken Sie **[!UICONTROL Übergangsregeln]** für den Stream, den Sie aus anderen Streams abrufen möchten, und klicken Sie dann auf **[!UICONTROL Übergangsregeln bearbeiten]**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >Übergangsregeln rufen einen Stream ab. Definieren Sie immer die Regeln für den Stream, in den Sie wechseln möchten.

   Sobald sich das Fenster für die Übergangsregel öffnet, suchen Sie den gewünschten Trigger und ziehen Sie ihn in den entsprechenden Bereich. In diesem Beispiel werden Personen in das [!UICONTROL Mid-Stadium] verschoben, wenn sie zu einer Opportunity hinzugefügt werden.

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. Stellen Sie den Operator auf **[!UICONTROL ist beliebig]** ein, damit die Personen für jede zusätzliche Gelegenheit zu ihm wechseln.

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >Sie können einer Übergangsregel mehrere Trigger und Filter hinzufügen, aber die Übergangsregel verwendet alle Filter (die einzige Option ist die Verwendung aller Filter). Wenn Sie ODER in einer Übergangsregel verwenden müssen, wird empfohlen, stattdessen eine externe intelligente Kampagne einzurichten.

1. Klicken Sie auf **[!UICONTROL Schließen]**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   Jetzt wird jede Person in Ihrem Interaktionsprogramm, die zu einer Opportunity hinzugefügt wird, in den [!UICONTROL Mid-Stage]-Stream verschoben.

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >Die oben beschriebenen Schritte *tun* gelten auch für Personen[ die ](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md) anhalten.
