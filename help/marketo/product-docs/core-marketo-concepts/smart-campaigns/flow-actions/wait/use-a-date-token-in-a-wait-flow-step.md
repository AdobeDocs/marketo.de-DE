---
unique-page-id: 1146997
description: Verwenden eines Datums-Tokens in einem Warteflussschritt - Marketo Docs - Produktdokumentation
title: Verwenden eines Datums-Tokens in einem Warteflussschritt
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Verwenden eines Datums-Tokens in einem Warteflussschritt {#use-a-date-token-in-a-wait-flow-step}

Mit dem Schritt Wartefluss können Sie das Journey einer Person durch eine intelligente Kampagne anhalten, bis zu einem bestimmten Datum, an dem ein Datums-Token verwendet wird. Sie können das Enddatum auch um einige Tage ändern.

>[!NOTE]
>
>Dies gilt nur für Trigger-Kampagnen. Sie können diese Funktion nicht in Batch-Kampagnen verwenden.

1. In Ihrer intelligenten Kampagne **Fluss** Registerkarte, ziehen Sie über die **Warten** Flussschritt.

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. Klicken Sie auf das Zahnradsymbol rechts.

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. Aus dem **Typ** Dropdown-Liste auswählen **Date Token**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. Wählen Sie ein Datum-Token aus, um anzugeben, wann der Warten-Schritt beendet werden soll:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. Um bis zum nächsten Jahrestag des Datums zu warten, das im aktuellen oder nächsten Kalenderjahr stattfindet, aktivieren Sie das Kontrollkästchen.

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >Verwenden Sie diese Option für Datums-Token, die auf Daten aus der Vergangenheit verweisen, wie z. B. Geburtstag oder Vertragsstartdatum.

1. Optional können Sie das Enddatum um eine angegebene Anzahl von Tagen ändern.

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >Sie können die Anzahl der Tage auch mithilfe einer `{{lead.` oder `{{company.` Token, das ein ganzzahliges Feld oder ein `{{my.` Token des Zahlentyps.

1. Klicks **Speichern**.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [Verwenden einer Dauer in einem Warteflussschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
   >* [Verwenden eines bestimmten Datums in einem Warteflussschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
