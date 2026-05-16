---
unique-page-id: 1146980
description: Erfahren Sie, wie Sie Auswahl hinzufügen in einem Flussschritt verwenden. Verzweigen Sie Ihren Kampagnenfluss basierend auf Bedingungen mit Auswahllogik.
title: Verwenden von „Auswahl hinzufügen“ in einem Flussschritt
exl-id: 50ffcd60-48ee-4341-94d8-170c63bc9ecb
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/2zIMDjJx0-Hm1NlgnGrQrnJuBwzMh0B2dq-tnJ34bZo
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 204
ht-degree: 6%

---

# Verwenden von „Auswahl hinzufügen“ in einem Flussschritt {#use-add-choice-in-a-flow-step}

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
   >Nur die erste übereinstimmende Auswahl wird auf den Flussschritt angewendet. Erfahren Sie, wie [&#x200B; „Auswahl hinzufügen“ in einer Flussaktion neu anordnen &#x200B;](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}.

   Sie können jetzt eine einzelne intelligente Kampagne mit Flussschritt-Auswahlmöglichkeiten erstellen, anstatt für jede Auswahl mehrere intelligente Kampagnen zu erstellen.

   >[!MORELIKETHIS]
   >
   >[Auswahl in einem Flussschritt neu anordnen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}
