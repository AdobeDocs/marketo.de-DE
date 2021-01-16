---
unique-page-id: 1146940
description: Intelligente Liste für intelligente Kampagne definieren | Batch - Marketing Docs - Produktdokumentation
title: Intelligente Liste für intelligente Kampagne definieren | Stapel
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---


# Intelligente Liste für intelligente Kampagne definieren | Batch {#define-smart-list-for-smart-campaign-batch}

Intelligente Listen sind der Mechanismus, mit dem in ganz Marketo &quot;wer&quot;(welche Personen) definiert werden soll, ob es sich um einen Bericht, eine Liste oder eine intelligente Kampagne handelt. So definieren Sie eine intelligente Liste für eine Batch-Kampagne.

1. Wählen Sie eine intelligente Kampagne und klicken Sie dann auf **Intelligente Liste**.

   ![](assets/campaignchoose-hand.png)

1. Geben Sie ein, um nach einem Filter zu suchen, und ziehen Sie ihn per Drag &amp; Drop auf die Arbeitsfläche. Wiederholen Sie diese Schritte für mehrere Filter.

   ![](assets/dragin.png)

   >[!NOTE]
   >
   >Eine intelligente Kampagne mit nur Filtern wird im Modus **Batch** ausgeführt. Es findet Personen in der Datenbank, die sich auf Grundlage der Filter qualifizieren, und führt sie alle gleichzeitig durch den Fluss.

   >[!NOTE]
   >
   >Sie können eine intelligente Kampagne basierend auf Live-Ereignissen einzeln ausführen lassen, indem Sie Trigger hinzufügen, wodurch die intelligente Kampagne im Modus **Trigger** ausgeführt wird.

1. Klicken Sie auf die Dropdownliste und wählen Sie einen Filteroperator für den ausgewählten Filter.

   ![](assets/programdropdown-hands.png)

   >[!CAUTION]
   >
   >Rote, zitternde Linien weisen auf Fehler oder fehlende Informationen hin. Wenn die Kampagne nicht korrigiert wird, ist sie ungültig und wird nicht ausgeführt.

1. Geben Sie den Filterwert ein.

   ![](assets/chooseprogram.png)

   >[!NOTE]
   >
   >Standardmäßig sind Personen, die ALLE Regeln der intelligenten Liste erfüllen, qualifiziert. Dies kann an Ihre Kampagne angepasst werden. Weitere Informationen finden Sie unter [Intelligente Liste für Complex Logic](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md).

   Um auf Live-Ereignissen einzeln Trigger, lernen Sie [Intelligente Liste für intelligente Kampagne definieren. | Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md).

   >[!MORELIKETHIS]
   >
   >* [Intelligente Liste für intelligente Kampagne definieren | Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [hinzufügen eines Flussschritts zu einer intelligenten Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

