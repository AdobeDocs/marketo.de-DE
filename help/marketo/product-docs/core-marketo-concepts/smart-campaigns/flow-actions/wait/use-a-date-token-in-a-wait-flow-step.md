---
unique-page-id: 1146997
description: Verwenden eines Datums-Tokens in einem Warteflussschritt - Marketo-Dokumente - Produktdokumentation
title: Verwenden eines Datums-Tokens in einem Warteflussschritt
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 9%

---

# Verwenden eines Datums-Tokens in einem Warteflussschritt {#use-a-date-token-in-a-wait-flow-step}

Sie können den Schritt „Fluss warten“ verwenden, um den Journey einer Person über eine Smart-Kampagne bis zu einem bestimmten Datum anzuhalten, das ein Datums-Token verwendet. Sie können das Enddatum auch nach einer bestimmten Anzahl von Tagen ändern.

>[!NOTE]
>
>Dies gilt nur für Trigger-Kampagnen. Sie können diese Funktion nicht in Batch-Kampagnen verwenden.

1. Ziehen Sie in der Registerkarte **[!UICONTROL Fluss]** der Smart-Kampagne den **[!UICONTROL Warten]**-Flussschritt.

   ![](assets/use-a-date-token-in-a-wait-flow-step-1.png)

1. Klicken Sie auf das Zahnradsymbol.

   ![](assets/use-a-date-token-in-a-wait-flow-step-2.png)

1. Wählen Sie in **[!UICONTROL Dropdown]** Typ“ die Option **[!UICONTROL Datumstoken]** aus.

   ![](assets/use-a-date-token-in-a-wait-flow-step-3.png)

1. Wählen Sie ein [!UICONTROL Datums-Token], um anzugeben, wann der Warteschritt beendet werden soll:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/use-a-date-token-in-a-wait-flow-step-4.png)

1. Um bis zum nächsten Jahrestag des Datums zu warten, das im aktuellen oder nächsten Kalenderjahr stattfindet, aktivieren Sie das Kontrollkästchen.

   ![](assets/use-a-date-token-in-a-wait-flow-step-5.png)

   >[!TIP]
   >
   >Verwenden Sie diese Option für Datumstoken, die auf frühere Daten verweisen, z. B. ein Geburtstags- oder Vertragsstartdatum.

1. Optional können Sie das Enddatum um eine bestimmte Anzahl von Tagen ändern.

   ![](assets/use-a-date-token-in-a-wait-flow-step-6.png)

   >[!NOTE]
   >
   >Sie können die Anzahl der Tage auch mithilfe eines `{{lead.`- oder `{{company.`-Tokens angeben, das ein ganzzahliges Feld darstellt, oder mithilfe eines `{{my.`-Tokens vom Typ Zahl .

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/use-a-date-token-in-a-wait-flow-step-7.png)

   >[!MORELIKETHIS]
   >
   >* [Verwenden Sie eine Dauer in einem Warteflussschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md){target="_blank"}
   >* [Verwenden eines bestimmten Datums in einem Warteflussschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
