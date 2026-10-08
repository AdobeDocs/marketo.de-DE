---
unique-page-id: 2360421
description: Erfahren Sie mehr über das Überschreiben des Analytics-Verhaltens auf Programmebene in Marketo Engage, einschließlich des Überschreiben des Analytics-Verhaltens. Machen Sie den nächsten Schritt selbstbewusst.
title: Überschreiben von Analyseverhalten auf Programmebene
exl-id: 2fd86279-99ae-494d-a6f8-2572b7dcd892
feature: Reporting, Revenue Cycle Analytics
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
    internal-label: Reporting
  - id: 126e34f9-e02a-505e-9978-ea36537f3ef9
    internal-label: Revenue Cycle Analytics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 10%
---
# Überschreiben des Analyseverhaltens auf Programmebene {#override-analytics-behavior-at-the-program-level}

Sie können das [Analytics-Verhalten auf der Admin-Ebene für Kanäle &#x200B;](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers.md), es kann aber auch auf Programmebene überschrieben werden. So geht&#39;s:

1. Navigieren Sie zum Bereich **[!UICONTROL Marketing-Aktivitäten]**.

   ![](assets/image2014-9-24-11-3a40-3a46.png)

1. Suchen und wählen Sie Ihr Programm aus.

   ![](assets/image2014-9-24-11-3a40-3a57.png)

1. Ziehen Sie auf **[!UICONTROL Registerkarte]** Setup“ [!UICONTROL Analytics Behavior] auf die Arbeitsfläche.

   ![](assets/image2014-9-24-11-3a41-3a2.png)

1. Wählen Sie das [!UICONTROL Analytics-Verhalten] aus, das Sie möchten.

   >[!NOTE]
   >
   >**Definition**
   >
   >* **Einschließlich** - Mit dieser Option wird sichergestellt, dass das Programm für das Reporting im Umsatz-Explorer und in Analyzern verfügbar ist, unabhängig davon, ob Sie einen Kostenzeitraum einbezogen haben oder nicht.
   >* **Operativ** - Diese Option führt dazu, dass das Programm weder im Umsatz-Explorer noch in Analyzern angezeigt wird.

   >[!NOTE]
   >
   >Das Standardverhalten (wenn diese Einstellung nicht angewendet wird) besteht darin, dass das Programm in Analytics eingeschlossen wird **NUR bei Kosten für mindestens einen Zeitraum** auch nur für einen mit null Dollar.

   ![](assets/image2014-9-24-11-3a42-3a0.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2014-9-24-11-3a42-3a6.png)

Gut gemacht! Jetzt wissen Sie, wie Sie das Analytics-Verhalten auf Programmebene überschreiben.

>[!NOTE]
>
>Die Änderungen treten am nächsten Tag in Kraft und werden entweder bereitgestellt oder aus dem Revenue Explorer und Analyzer abgerufen.
