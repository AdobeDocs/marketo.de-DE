---
unique-page-id: 1146997
description: Verwenden Sie ein Datums-Token in einem Wartezeitschritt - MarketingToDocs - Produktdokumentation
title: Verwenden eines Datums-Tokens in einem Wartezeitschritt
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# Verwenden Sie ein Datums-Token in einem Warteflussschritt {#use-a-date-token-in-a-wait-flow-step}

Mit dem Schritt zum Warten können Sie die Journey einer Person durch eine intelligente Kampagne anhalten, bis zu einem bestimmten Datum, das ein Datums-Token verwendet. Sie können das Enddatum auch um einige Tage ändern.

>[!NOTE]
>
>Dies gilt nur für Kampagnen des Triggers. Sie können diese Funktion nicht in Batch-Kampagnen verwenden.

1. Ziehen Sie in der Registerkarte &quot;Smart-Kampagne **Fluss**&quot;über den Textfluss **Wait**.

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. Klicken Sie auf das Zahnradsymbol rechts.

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. Wählen Sie aus der Dropdownliste **Typ** **Datumszeichen**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. Wählen Sie ein Datums-Token, um anzugeben, wann der Warten-Schritt enden soll:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. Wenn Sie bis zum nächsten Jahrestag des Datums im aktuellen oder nächsten Kalenderjahr warten möchten, markieren Sie das entsprechende Kästchen.

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >Verwenden Sie diese Option für Datums-Token, die sich auf Daten aus der Vergangenheit beziehen, wie z. B. ein Geburtstag oder ein Beginn.

1. Optional können Sie das Enddatum um eine angegebene Anzahl von Tagen ändern.

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >Sie können auch die Anzahl der Tage mit einem Token des Typs `{{lead.` oder `{{company.` angeben, das ein ganzzahliges Feld oder ein Token des Typs `{{my.` darstellt.

1. Klicken Sie auf **Speichern**.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [Verwenden einer Dauer in einem Wartezeitschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
   >* [Verwenden eines bestimmten Datums in einem Schritt mit einem Wartefluss](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)

