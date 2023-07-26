---
unique-page-id: 2359947
description: Transition von Personen zwischen Interaktions-Streams - Marketo-Dokumente - Produktdokumentation
title: Übergang von Personen zwischen Interaktionsströmen
exl-id: 2367852c-3dcf-4188-a50c-7c6f0b0ff7bc
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 1%

---

# Übergang von Personen zwischen Interaktionsströmen {#transition-people-between-engagement-streams}

Interaktionsprogramme können mehrere Streams aufweisen. Wenn Sie [Stream hinzufügen](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-a-stream.md), möchten Sie eine Möglichkeit definieren, wie Personen von einem Stream zum anderen wechseln können. Diese werden **Übergangsregeln.**

1. Navigieren Sie zu **Marketingaktivitäten**.

   ![](assets/ma.png)

1. Wählen Sie Ihr Multi-Streaming-Interaktionsprogramm aus und navigieren Sie zu **Streams**.

   ![](assets/multistream.jpg)

1. Klicks **Übergangsregeln** für den Stream, in den Sie aus anderen Streams abrufen möchten, klicken Sie auf **Übergangsregeln bearbeiten**.

   ![](assets/image2014-9-15-18-3a10-3a18.png)

   >[!NOTE]
   >
   >Übergangsregeln ziehen in einen Stream. Definieren Sie immer die Regeln im Stream, in den Sie ziehen möchten.

   Sobald das Fenster der Übergangsregel geöffnet ist, suchen und ziehen Sie den gewünschten Trigger. In diesem Fall möchten wir Menschen in die Mid-Stage verschieben, wenn sie zu einer Chance hinzugefügt wird.

   ![](assets/image2014-9-15-18-3a10-3a46.png)

1. Setzen wir den Operator auf **ist** damit die Menschen für jede zusätzliche Gelegenheit umziehen.

   ![](assets/image2014-9-15-18-3a11-3a14.png)

   >[!TIP]
   >
   >Sie können einer Übergangsregel mehrere Trigger und Filter hinzufügen. Die Übergangsregel verwendet jedoch alle Filter (nur mit ALLEN Filtern). Wenn Sie ODER in einer Übergangsregel verwenden müssen, empfehlen wir stattdessen die Einrichtung einer externen Smart-Kampagne.

1. Klicken Sie auf **Schließen**.

   ![](assets/image2014-9-15-18-3a11-3a23.png)

   Sehr gut! Jetzt wird jede Person in Ihrem Interaktionsprogramm, die zu einer Gelegenheit hinzugefügt wird, in den Mid-Stage-Stream verschoben.

   ![](assets/image2014-9-15-18-3a11-3a29.png)

   >[!NOTE]
   >
   >Die oben beschriebenen Schritte *do* sich auf Personen beziehen, die [bei Pause](/help/marketo/product-docs/email-marketing/drip-nurturing/using-engagement-programs/pause-people-in-an-engagement-program.md) sowie.
