---
unique-page-id: 1146940
description: Definieren einer Smart-Liste für eine intelligente Kampagne | Batch - Marketo-Dokumente - Produktdokumentation
title: Definieren einer Smart-Liste für eine intelligente Kampagne | Batch
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
feature: Smart Campaigns
source-git-commit: c3aa1a29b084cb1c1add9d22cdbfc23bdcf7512b
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Definieren einer Smart-Liste für eine intelligente Kampagne | Batch {#define-smart-list-for-smart-campaign-batch}

Smart-Listen sind der Mechanismus, mit dem während der gesamten Marketo Engage definiert wird, wer (welche Personen) einbezogen werden soll, sei es als Bericht, Liste oder Smart-Kampagne. So definieren Sie eine Smart-Liste für eine Batch-Kampagne:

>[!CAUTION]
>
>Die Bearbeitung von Smart-Listen- oder Flussschritt-Bearbeitungen an einer aktiven Kampagne kann möglicherweise deren Funktionalität beeinträchtigen. Gehen Sie dabei mit Vorsicht vor.

1. Wählen Sie eine Smart-Kampagne und klicken Sie dann auf **[!UICONTROL Smart-Liste]**.

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. Geben Sie ein, um nach einem Filter zu suchen, und ziehen Sie ihn per Drag-and-Drop auf die Arbeitsfläche. Wiederholen Sie diesen Vorgang für mehrere Filter.

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >Eine Smart-Kampagne mit nur Filtern wird im Modus _Batch_ ausgeführt. Es findet Personen in der Datenbank, die sich auf der Grundlage der Filter qualifizieren, und führt sie alle gleichzeitig durch den Fluss.

   >[!NOTE]
   >
   >Sie können eine Smart-Kampagne auf der Basis von Live-Ereignissen für eine Person ausführen lassen, indem Sie Trigger hinzufügen, wodurch die Smart-Kampagne in den Modus _Trigger_ versetzt wird.

1. Klicken Sie auf die Dropdown-Liste und wählen Sie einen Filteroperator für den gewählten Filter aus.

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >Rote eckige Linien zeigen Fehler oder fehlende Informationen an. Wenn die Kampagne nicht korrigiert wird, ist sie ungültig und wird nicht ausgeführt.

1. Geben Sie den Filterwert ein.

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >Standardmäßig werden Personen qualifiziert, die ALLE Regeln der intelligenten Liste erfüllen. Dieser kann Ihren Kampagnenanforderungen entsprechend angepasst werden. Weitere Informationen finden Sie unter [Smart List Rules for Complex Logic](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"} .

   Informationen zum individuellen Trigger von Live-Ereignissen finden Sie unter [Definieren einer Smart-Liste für Smart-Campaign | Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}.

   >[!MORELIKETHIS]
   >
   >* [Definieren einer Smart-Liste für Smart-Campaign | Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
   >* [Hinzufügen eines Flussschritts zu einer Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
