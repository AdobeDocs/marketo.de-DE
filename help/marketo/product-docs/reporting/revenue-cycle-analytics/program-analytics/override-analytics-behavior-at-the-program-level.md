---
unique-page-id: 2360421
description: Analytics-Verhalten auf Programmebene außer Kraft setzen - Marketo Docs - Produktdokumentation
title: Analytics-Verhalten auf Programmebene überschreiben
exl-id: 2fd86279-99ae-494d-a6f8-2572b7dcd892
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 1%

---

# Analytics-Verhalten auf Programmebene überschreiben {#override-analytics-behavior-at-the-program-level}

Sie können das Analytics-Verhalten [auf Admin-Ebene auf Kanälen](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers.md) festlegen, es aber auch auf Programmebene überschreiben. Gehen Sie wie folgt vor:

1. Wechseln Sie zum Bereich **Marketingaktivitäten** .

   ![](assets/image2014-9-24-11-3a40-3a46.png)

1. Wählen Sie Ihr Programm aus.

   ![](assets/image2014-9-24-11-3a40-3a57.png)

1. Ziehen Sie unter der Registerkarte **Einrichtung** das Analytics-Verhalten auf die Arbeitsfläche.

   ![](assets/image2014-9-24-11-3a41-3a2.png)

1. Wählen Sie das gewünschte Analytics-Verhalten aus.

   >[!NOTE]
   >
   >**Definition**
   >
   >* **Einschließlich** - Mit dieser Option wird sichergestellt, dass das Programm für die Berichterstellung in Umsatz-Explorer und Analyzern verfügbar ist, unabhängig davon, ob Sie einen Zeitraumpreis angegeben haben oder nicht.
   >* **Operativ** - Diese Option führt dazu, dass das Programm weder in den Umsatz-Explorer noch in den Analyzern angezeigt wird.

   >[!NOTE]
   >
   >Das Standardverhalten (wenn diese Einstellung nicht angewendet wird) besteht darin, dass das Programm NUR dann in Analytics **enthalten ist, wenn mindestens ein Zeitraumkosten** vorliegt, selbst wenn einem Wert 0 zugewiesen ist.

   ![](assets/image2014-9-24-11-3a42-3a0.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2014-9-24-11-3a42-3a6.png)

Schön gemacht! Jetzt wissen Sie, wie Sie das Analyseverhalten auf Programmebene überschreiben können.

>[!NOTE]
>
>Die Änderungen werden am nächsten Tag wirksam und entweder bereitgestellt oder aus dem Umsatz-Explorer und den Analyzern abgerufen.
