---
unique-page-id: 1146940
description: Definieren einer Smart-Liste für eine intelligente Kampagne | Batch - Marketo-Dokumente - Produktdokumentation
title: Definieren einer Smart-Liste für eine intelligente Kampagne | Charge
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
feature: Smart Campaigns
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Definieren einer Smart-Liste für eine intelligente Kampagne | Charge {#define-smart-list-for-smart-campaign-batch}

Smart-Listen sind der Mechanismus, mit dem während der gesamten Marketo Engage definiert wird, wer (welche Personen) einbezogen werden soll, sei es als Bericht, Liste oder Smart-Kampagne. So definieren Sie eine Smart-Liste für eine Batch-Kampagne:

1. Wählen Sie eine Smart-Kampagne aus und klicken Sie auf **[!UICONTROL Smart List]**.

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. Geben Sie ein, um nach einem Filter zu suchen, und ziehen Sie ihn per Drag-and-Drop auf die Arbeitsfläche. Wiederholen Sie diesen Vorgang für mehrere Filter.

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >Eine Smart-Kampagne mit nur Filtern wird in _Batch_ -Modus. Es findet Personen in der Datenbank, die sich auf der Grundlage der Filter qualifizieren, und führt sie alle gleichzeitig durch den Fluss.

   >[!NOTE]
   >
   >Sie können eine Smart-Kampagne auf Basis von Live-Ereignissen einzeln durchführen, indem Sie Trigger hinzufügen, wodurch die Smart-Kampagne aktiviert wird. _Trigger_ -Modus.

1. Klicken Sie auf die Dropdown-Liste und wählen Sie einen Filteroperator für den gewählten Filter aus.

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >Rote eckige Linien zeigen Fehler oder fehlende Informationen an. Wenn die Kampagne nicht korrigiert wird, ist sie ungültig und wird nicht ausgeführt.

1. Geben Sie den Filterwert ein.

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >Standardmäßig werden Personen qualifiziert, die ALLE Regeln der intelligenten Liste erfüllen. Dieser kann Ihren Kampagnenanforderungen entsprechend angepasst werden. Checkout  [Smart List Rules for Complex Logic](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"} , um mehr zu erfahren.

   Lernen Sie, wie Sie Live-Events einzeln Trigger haben [Definieren einer Smart-Liste für eine intelligente Kampagne | TRIGGER](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}.

   >[!MORELIKETHIS]
   >
   >* [Definieren einer Smart-Liste für eine intelligente Kampagne | TRIGGER](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
   >* [Hinzufügen eines Flussschritts zu einer Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
