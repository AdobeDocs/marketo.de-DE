---
unique-page-id: 1146940
description: Erfahren Sie, wie Sie die Smart-Liste für eine Smart-Batch-Kampagne definieren. Wählen Sie aus, wer mit Filtern in die Kampagne eintritt.
title: Definieren einer intelligenten Liste für eine intelligente Kampagne | Stapel
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
feature: Smart Campaigns
source-git-commit: 60c5603fa29bb1039b9d477633beb2c6f5c63486
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 5%

---

# Definieren einer intelligenten Liste für eine intelligente Kampagne | Stapel {#define-smart-list-for-smart-campaign-batch}

Smart Lists sind in Marketo Engage der Mechanismus, mit dem definiert wird, „wer“ (welche Personen) einbezogen werden sollen, unabhängig davon, ob es sich um einen Bericht, eine Liste oder eine Smart Campaign handelt.

>[!CAUTION]
>
>Die Bearbeitung von Smart List- oder Flow Step-Elementen an einer aktiven Kampagne kann deren Funktionalität beeinträchtigen. Wenn Sie sich dafür entscheiden, gehen Sie mit Vorsicht vor.

1. Wählen Sie eine Smart-Kampagne aus und klicken Sie dann auf **[!UICONTROL Smart-Liste]**.

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. Tippen Sie, um nach einem Filter zu suchen und ihn per Drag-and-Drop auf die Arbeitsfläche zu ziehen. Wiederholen Sie dies für mehrere Filter.

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >Eine Smart Campaign mit nur Filtern wird im _Batch_-Modus ausgeführt. Er findet Personen in der Datenbank, die sich anhand der Filter qualifizieren, und führt alle gleichzeitig durch den Fluss.

   >[!NOTE]
   >
   >Sie können eine Smart-Kampagne auf der Grundlage von Live-Ereignissen einzeln ausführen lassen, indem Sie Trigger hinzufügen. Dadurch wird die Smart-Kampagne in den Trigger __ versetzt.

1. Klicken Sie auf das Dropdown-Menü und wählen Sie einen Filteroperator für den ausgewählten Filter.

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >Rote schielende Linien zeigen Fehler oder fehlende Informationen an. Wenn die Kampagne nicht korrigiert wird, ist sie ungültig und wird nicht ausgeführt.

1. Geben Sie den Filterwert ein.

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >Standardmäßig sind Personen qualifiziert, die ALLE Regeln der Smart-Liste erfüllen. Dies kann Ihren Kampagnenanforderungen entsprechend geändert werden. Weitere Informationen finden [&#x200B; unter „Regeln für intelligente Listen &#x200B;](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"} komplexe Logik“.

   Um Trigger auf Live-Ereignisse einzeln durchzuführen, erfahren Sie hier, wie Sie [Smart-Liste für Smart-Kampagnen definieren | Trigger &#x200B;](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}.

   >[!MORELIKETHIS]
   >
   >* [Definieren der Smart-Liste für Smart-Kampagnen | Trigger &#x200B;](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
   >* [Hinzufügen eines Flussschritts zu einer Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
