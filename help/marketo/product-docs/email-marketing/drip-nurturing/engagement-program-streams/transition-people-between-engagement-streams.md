---
unique-page-id: 2359947
description: Transition von Personen zwischen Interaktionsströmen - Marketing-Dokumente - Produktdokumentation
title: Transition von Personen zwischen Interaktionsströmen
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---


# Transition von Personen zwischen Interaktionsströmen {#transition-people-between-engagement-streams}

Interaktions-Programm können über mehr als einen Stream verfügen. Wenn Sie einen Stream [](../../../../product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md)hinzufügen, möchten Sie eine Möglichkeit definieren, wie Benutzer von einem Stream zu einem anderen wechseln können. Diese werden als **Transitionen bezeichnet.**

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

1. Gehen Sie zu **Marketing-Aktivitäten**.

   ![](assets/ma.png)

1. Wählen Sie Ihr Multi-Streaming-Programm aus und gehen Sie zu **Streams**.

   ![](assets/multistream.jpg)

1. Klicken Sie auf **Transitionen** für den Stream, den Sie aus anderen Streams übernehmen möchten, und klicken Sie dann auf **Transitionen bearbeiten. **

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >Transitionen ziehen in einen Stream; definieren Sie immer die Regeln für den Stream, in den Sie ziehen möchten.

   Sobald sich das Fenster für die Transition öffnet, suchen Sie den Auslöser Ihrer Wahl und ziehen Sie ihn. In diesem Fall wollen wir Menschen in die Mid-Stage verschieben, wenn sie zu einer Gelegenheit hinzugefügt wird.
` ![](assets/image2014-9-15-18-3a10-3a46.png)

   `

1. Setzen wir den Operator auf** ist beliebige*, damit die Leute für jede zusätzliche Gelegenheit umziehen.

   ` ![](assets/image2014-9-15-18-3a11-3a14.png)

   `

   >[!TIP]
   >
   >Sie können einer Transitionen-Regel mehrere Auslöser und Filter hinzufügen. Die Transition verwendet jedoch alle Filter (nur bei Verwendung von ALLE Filter). Wenn Sie ODER in einer Transition verwenden müssen, sollten Sie stattdessen eine externe Smart-Kampagne einrichten.

1. Klicken Sie auf **Schließen**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   Großartig! Nun wird jede Person in Ihrem Interaktionsnetzwerk, die einer Gelegenheit hinzugefügt wird, in den Mid-Stage-Stream verschoben.

   ` ![](assets/image2014-9-15-18-3a11-3a29.png)

   `

   >[!NOTE]
   >
   >Die oben beschriebenen Schritte *gelten* auch für Personen, die [Pause](http://docs.marketo.com/display/DOCS/Pause+People+in+an+Engagement+Program) haben.

