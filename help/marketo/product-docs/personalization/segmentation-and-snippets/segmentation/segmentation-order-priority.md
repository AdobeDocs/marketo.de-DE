---
unique-page-id: 2359500
description: Erfahren Sie mehr über die Priorität der Segmentierungsreihenfolge und darüber, wie sie bestimmt, zu welchem Segment eine Person gehört. Bearbeiten der Segmentreihenfolge in der Datenbank, um die Auswertung von Segmenten zu steuern.
title: Priorität der Segmentierungsreihenfolge
exl-id: c20d07c8-5e53-4f54-a7a3-2e1aa4fb0cdd
feature: Segmentation
source-git-commit: 80b39eb99cdaacf4c9655aa175da3d22548dcca6
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 4%

---

# Priorität der Segmentierungsreihenfolge {#segmentation-order-priority}

Es ist wichtig zu verstehen, wie **Reihenfolge** die Priorität für die Bewertung Ihrer Mitarbeiter in einer Segmentierung festlegt.

>[!PREREQUISITES]
>
>[Segmentierung erstellen](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>[Definieren Sie Segmentregeln](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>Eine Segmentierung kann nur im Entwurfsmodus bearbeitet werden.

1. Navigieren Sie zur **Datenbank**.

   ![](assets/segmentation-order-priority-1.png)

1. Wählen Sie Ihre **Segmentierung** aus. Klicken **[!UICONTROL unter &quot;]**&quot; auf **[!UICONTROL Segmente bearbeiten]**.

   ![](assets/segmentation-order-priority-2.png)

   Auf diesem Bildschirm können Sie die Reihenfolge der Segmente überprüfen oder bearbeiten.

   ![](assets/segmentation-order-priority-3.png)

>[!NOTE]
>
>* Die Segmente schließen sich gegenseitig aus. Eine Person kann immer nur Mitglied eines Segments sein.
>* Wenn sich eine Person für zwei Segmente qualifiziert, gehört sie nur zum ersten Segment in der Liste.
>* Wenn sich eine Person nicht für ein Segment qualifiziert, wird sie Mitglied des Standardsegments.
