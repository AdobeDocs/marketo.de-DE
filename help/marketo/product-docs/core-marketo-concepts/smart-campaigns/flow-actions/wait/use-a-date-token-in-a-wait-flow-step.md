---
unique-page-id: 1146997
description: Verwenden eines Datums-Tokens in einem Warteflussschritt - Marketo Docs - Produktdokumentation
title: Verwenden eines Datums-Tokens in einem Warteflussschritt
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Verwenden eines Datums-Tokens in einem Warteflussschritt {#use-a-date-token-in-a-wait-flow-step}

Mit dem Schritt Wartefluss können Sie das Journey einer Person durch eine Smart-Kampagne anhalten, bis zu einem bestimmten Datum, an dem ein Datums-Token verwendet wird. Sie können das Enddatum auch um einige Tage ändern.

>[!NOTE]
>
>Dies gilt nur für Trigger-Kampagnen. Sie können diese Funktion nicht in Batch-Kampagnen verwenden.

1. Ziehen Sie in der Registerkarte **[!UICONTROL Fluss]** Ihrer Smart-Kampagne über den Flussschritt **[!UICONTROL Warten]**.

   ![](assets/use-a-date-token-in-a-wait-flow-step-1.png)

1. Klicken Sie auf das Zahnradsymbol.

   ![](assets/use-a-date-token-in-a-wait-flow-step-2.png)

1. Wählen Sie aus der Dropdownliste **[!UICONTROL Typ]** die Option **[!UICONTROL Datum-Token]** aus.

   ![](assets/use-a-date-token-in-a-wait-flow-step-3.png)

1. Wählen Sie ein Datum-Token aus, um anzugeben, wann der Warten-Schritt beendet werden soll:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/use-a-date-token-in-a-wait-flow-step-4.png)

1. Um bis zum nächsten Jahrestag des Datums zu warten, das im aktuellen oder nächsten Kalenderjahr stattfindet, aktivieren Sie das Kontrollkästchen.

   ![](assets/use-a-date-token-in-a-wait-flow-step-5.png)

   >[!TIP]
   >
   >Verwenden Sie diese Option für Datums-Token, die auf Daten aus der Vergangenheit verweisen, wie z. B. Geburtstag oder Vertragsstartdatum.

1. Optional können Sie das Enddatum um eine angegebene Anzahl von Tagen ändern.

   ![](assets/use-a-date-token-in-a-wait-flow-step-6.png)

   >[!NOTE]
   >
   >Sie können die Anzahl der Tage auch mithilfe eines `{{lead.` - oder `{{company.` -Tokens angeben, das ein ganzzahliges Feld oder ein `{{my.` -Token des Zahlentyps darstellt.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/use-a-date-token-in-a-wait-flow-step-7.png)

   >[!MORELIKETHIS]
   >
   >* [Verwenden einer Dauer in einem Warteflussschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md){target="_blank"}
   >* [Verwenden eines bestimmten Datums in einem Warteflussschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
