---
unique-page-id: 10097873
description: Definieren einer Smart-Liste für Aktivitäten mit prädiktiven Inhalten - Marketo-Dokumente - Produktdokumentation
title: Definieren einer intelligenten Liste für prädiktive Inhaltsaktivitäten
exl-id: 2c72b215-8c0b-48b4-8492-8e3fe832fae9
feature: Predictive Content
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 5%

---

# Definieren einer intelligenten Liste für prädiktive Inhaltsaktivitäten {#define-a-smart-list-for-predictive-content-activities}

Sie können prädiktive Inhaltsaktivitäten in Triggern und Filtern verwenden, wenn Sie in einer Smart-Kampagne eine Smart-Liste definieren. Sie können einen Trigger für eine Aktion für alle erstellen, die über die [Rich-Media-Vorlage](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md), die [Inhaltsempfehlungsleiste](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md) oder in einer [E-Mail](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md) auf prädiktive Inhalte klicken.

1. Navigieren Sie in Ihrer Smart-Kampagne zur Registerkarte **[!UICONTROL Smart-Liste]** .

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >Intelligente Listen können erstaunliche Dinge bewirken. Weitere Informationen finden Sie in [Smart List Deep Dive](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md).

1. Suchen Sie nach dem Trigger und ziehen Sie ihn dann per Drag-and-Drop auf die Arbeitsfläche.

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >Eine Smart-Kampagne mit Triggern wird im Trigger-Modus ausgeführt. Sie wird immer nur für eine Person ausgeführt, basierend auf den ausgelösten Ereignissen und den hinzugefügten Filtern.

1. Klicken Sie auf **[!UICONTROL Name]** und wählen Sie einen Operator aus.

   ![](assets/smart-list-dropdown-hands.png)

1. Definieren Sie den Trigger.

   ![](assets/smart-lislt-select-content-hands.png)

1. Fügen Sie die **[!UICONTROL Type]**-Einschränkung hinzu.

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. Wählen Sie die Quelle aus, die Sie für Ihre Smart-Liste benötigen.

   ![](assets/pc-add-constraint.png)

1. Wenn Sie die E-Mail-Quelle für Ihren prädiktiven Inhalt verwenden, fügen Sie den Trigger **[!UICONTROL Klicks-Link in E-Mail]** hinzu. Wählen Sie Ihre E-Mail aus und fügen Sie die **[!UICONTROL Ist prädiktiv]**-Einschränkung hinzu, die als **[!UICONTROL true“]**.

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. Fügen Sie bei Bedarf weitere Filter hinzu.

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >In einer intelligenten Kampagne mit sowohl Triggern als auch Filtern gehen die Trigger an die Spitze. Wenn sie ausgelöst wird, durchlaufen nur Personen den Fluss, die die Filterkriterien erfüllen.

   >[!NOTE]
   >
   >Bei mehreren Triggern wechselt eine Person in den Fluss, wenn einer der Trigger aktiviert wird.

   Wenn Sie die Kampagne für mehrere Personen gleichzeitig ausführen möchten, erfahren Sie hier, wie [eine Smart-Liste für eine Smart-Batch-Kampagne definieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

   >[!MORELIKETHIS]
   >
   >* [Definieren der Smart-Liste für intelligente Kampagnen | Batch](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [Hinzufügen eines Flussschritts zu einer Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [Definieren einer Smart List für Web Personalization-Aktivitäten](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [Prädiktive Inhalte für Web-Rich-Media aktivieren](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [Aktivieren der Inhaltsempfehlungsleiste](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)
