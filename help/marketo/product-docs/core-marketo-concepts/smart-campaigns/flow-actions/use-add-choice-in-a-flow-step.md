---
unique-page-id: 1146980
description: Auswahl in einem Flussschritt hinzufügen - Marketo-Dokumente - Produktdokumentation
title: Auswahl in einem Flussschritt hinzufügen
exl-id: 50ffcd60-48ee-4341-94d8-170c63bc9ecb
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Auswahl in einem Flussschritt hinzufügen {#use-add-choice-in-a-flow-step}

>[!PREREQUISITES]
>
>[Hinzufügen eines Flussschritts zu einer Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

Mit &quot;Auswahl hinzufügen&quot;können Sie einen Flussschritt verwenden und bei der Auswahl der Details &quot;Es kommt darauf an&quot;.

1. Fügen Sie auf der Registerkarte **[!UICONTROL Fluss]** der Smart-Kampagne einen beliebigen Flussschritt hinzu und klicken Sie auf **[!UICONTROL Auswahl hinzufügen]**.

   ![](assets/use-add-choice-in-a-flow-step-1.png)

1. Wählen Sie die Auswahlbedingung aus.

   ![](assets/use-add-choice-in-a-flow-step-2.png)

1. Wählen Sie den Auswahloperator aus und geben Sie einen Auswahlwert ein. Dadurch werden Ihre Kriterien oder Auswahlmöglichkeiten festgelegt.

   ![](assets/use-add-choice-in-a-flow-step-3.png)

1. Geben Sie einen Flussstufenwert für die Auswahl ein.

   ![](assets/use-add-choice-in-a-flow-step-4.png)

   >[!CAUTION]
   >
   >Token funktionieren im Bedingungsabschnitt eines Auswahlflussschritts _nicht_.

1. Wiederholen Sie die obigen Schritte, um mehrere Auswahlmöglichkeiten hinzuzufügen, und fügen Sie dann den Standardwert hinzu/passen Sie ihn an.

   ![](assets/use-add-choice-in-a-flow-step-5.png)

   >[!TIP]
   >
   >Sie können einen beliebigen Durchsatzschritt auf &quot;Nichts tun&quot;festlegen. In diesem Fall wird keine Aktion für diese Auswahl durchgeführt.

   >[!CAUTION]
   >
   >Nur die erste passende Auswahl wird auf den Flussschritt angewendet. Erfahren Sie, wie Sie &quot;[in einer Flussaktion die Option &quot;Auswahl hinzufügen&quot;neu anordnen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}.

   Sehr gut! Sie können jetzt eine einzelne Smart-Kampagne mit Flussschritt-Optionen erstellen, anstatt mehrere Smart-Kampagnen für jede Auswahl zu erstellen.

   >[!MORELIKETHIS]
   >
   >[Neuanordnen der Option &quot;Hinzufügen&quot;in einem Flussschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}
