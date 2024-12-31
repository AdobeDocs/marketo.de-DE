---
unique-page-id: 1146980
description: Verwenden der Option „Auswahl hinzufügen“ in einem Flussschritt - Marketo-Dokumente - Produktdokumentation
title: Verwenden von Auswahl hinzufügen in einem Flussschritt
exl-id: 50ffcd60-48ee-4341-94d8-170c63bc9ecb
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Verwenden von Auswahl hinzufügen in einem Flussschritt {#use-add-choice-in-a-flow-step}

>[!PREREQUISITES]
>
>[Hinzufügen eines Flussschritts zu einer Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

Mit „Auswahl hinzufügen“ können Sie einen Flussschritt verwenden und sagen „Es kommt darauf an“, wenn Sie die Details auswählen.

1. Fügen Sie auf der **[!UICONTROL Fluss]** der Smart-Kampagne einen beliebigen Flussschritt hinzu und klicken Sie dann auf **[!UICONTROL Auswahl hinzufügen]**.

   ![](assets/use-add-choice-in-a-flow-step-1.png)

1. Wählen Sie die Auswahlbedingung aus.

   ![](assets/use-add-choice-in-a-flow-step-2.png)

1. Wählen Sie den Auswahloperator aus und geben Sie einen Auswahlwert ein. Dadurch werden Ihre Kriterien oder Auswahlmöglichkeiten festgelegt.

   ![](assets/use-add-choice-in-a-flow-step-3.png)

1. Geben Sie einen Flussschrittwert für die Auswahl ein.

   ![](assets/use-add-choice-in-a-flow-step-4.png)

   >[!CAUTION]
   >
   >Token funktionieren _nicht_ im Bedingungsteil eines Auswahlflussschritts.

1. Wiederholen Sie die obigen Schritte, um mehrere Auswahlmöglichkeiten hinzuzufügen, und fügen Sie dann den Standardwert hinzu bzw. passen Sie ihn an.

   ![](assets/use-add-choice-in-a-flow-step-5.png)

   >[!TIP]
   >
   >Sie können einen Ihrer Flussschritte auf —Nichts tun— einstellen. In diesem Fall wird keine Aktion für diese Auswahl durchgeführt.

   >[!CAUTION]
   >
   >Nur die erste übereinstimmende Auswahl wird auf den Flussschritt angewendet. Erfahren Sie, wie [ „Auswahl hinzufügen“ in einer Flussaktion neu anordnen ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}.

   Sehr gut! Sie können jetzt eine einzelne intelligente Kampagne mit Flussschritt-Auswahlmöglichkeiten erstellen, anstatt für jede Auswahl mehrere intelligente Kampagnen zu erstellen.

   >[!MORELIKETHIS]
   >
   >[Auswahl in einem Flussschritt neu anordnen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}
