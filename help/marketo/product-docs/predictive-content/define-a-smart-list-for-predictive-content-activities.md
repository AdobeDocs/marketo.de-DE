---
unique-page-id: 10097873
description: Definieren einer Smart-Liste für Predictive Content-Aktivitäten - Marketo Docs - Produktdokumentation
title: Definieren einer Smart-Liste für Predictive Content-Aktivitäten
exl-id: 2c72b215-8c0b-48b4-8492-8e3fe832fae9
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Definieren einer Smart-Liste für Predictive Content-Aktivitäten {#define-a-smart-list-for-predictive-content-activities}

Sie können vorausschauende Inhaltsaktivitäten in Triggern und Filtern verwenden, wenn Sie eine Smart-Liste in einer Smart-Kampagne definieren. Sie können eine Aktion für jeden Trigger erstellen, der auf prädiktive Inhalte über die Vorlage [Rich-Media-Inhalt](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md), die Symbolleiste [Inhaltsempfehlung](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md) oder eine [E-Mail](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md) klickt.

1. Navigieren Sie in Ihrer Smart-Kampagne zur Registerkarte **Smart-Liste** .

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >Intelligente Listen können erstaunliche Dinge tun. Weitere Informationen finden Sie im [Deep-Dive der Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md).

1. Suchen Sie nach dem Trigger und ziehen Sie ihn per Drag-and-Drop auf die Arbeitsfläche.

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >Eine Smart-Kampagne mit Triggern wird im Trigger-Modus ausgeführt. Er wird basierend auf den ausgelösten Ereignissen und den hinzugefügten Filtern für jeweils eine Person ausgeführt.

1. Klicken Sie auf die Dropdownliste **Name** und wählen Sie einen Operator aus.

   ![](assets/smart-list-dropdown-hands.png)

1. Definieren Sie den Trigger.

   ![](assets/smart-lislt-select-content-hands.png)

1. Fügen Sie die Beschränkung **Typ** hinzu.

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. Wählen Sie die Quelle aus, die Sie für Ihre Smart-Liste benötigen.

   ![](assets/pc-add-constraint.png)

1. Wenn Sie die E-Mail-Quelle für Ihren prädiktiven Inhalt verwenden, fügen Sie den Trigger **Klicks-Link in E-Mail** hinzu. Wählen Sie Ihre E-Mail aus und fügen Sie die Beschränkung **Is Predictive** hinzu, die als **true** definiert ist.

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. Fügen Sie nach Bedarf weitere Filter hinzu.

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >In einer intelligenten Kampagne mit Triggern und Filtern stehen die Trigger ganz oben. Wenn sie ausgelöst wird, durchlaufen nur Personen, die die Filterkriterien erfüllen, den Fluss.

   >[!NOTE]
   >
   >Bei mehreren Triggern durchläuft eine Person den Fluss, wenn einer der Trigger aktiviert wird.

   Um die Kampagne für eine Reihe von Personen gleichzeitig auszuführen, erfahren Sie, wie Sie [eine Smart-Liste für eine Batch-Smart-Kampagne definieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

   >[!MORELIKETHIS]
   >
   >* [Definieren einer Smart-Liste für Smart-Campaign | Batch](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [Hinzufügen eines Flussschritts zu einer Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [Definieren einer Smart-Liste für Web-Personalization-Aktivitäten](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [Aktivieren von prädiktivem Inhalt für Web-Rich-Media](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [Aktivieren Sie die Symbolleiste für Inhaltsempfehlungen](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)
