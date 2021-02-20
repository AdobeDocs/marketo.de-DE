---
unique-page-id: 10097873
description: Definieren Sie eine intelligente Liste für Predictive Content-Aktivitäten - Marketing-Dokumente - Produktdokumentation
title: Definieren einer intelligenten Liste für Predictive Content-Aktivitäten
translation-type: tm+mt
source-git-commit: f1d7b270454ba41db5197a069e0dcc2caebdec63
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---


# Definieren Sie eine intelligente Liste für Aktivitäten mit prognostiziertem Inhalt {#define-a-smart-list-for-predictive-content-activities}

Sie können Aktivitäten mit vorhersehbarem Inhalt in Triggern und Filtern verwenden, wenn Sie eine intelligente Liste in einer intelligenten Kampagne definieren. Sie können eine Aktion für alle Benutzer, die auf Prognoseinhalte klicken, über die [Rich Media-Vorlage](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md), die [Inhaltsempfehlung-Leiste](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md) oder über eine [E-Mail](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md)-Trigger ausführen.

1. Navigieren Sie in Ihrer intelligenten Kampagne zur Registerkarte **Intelligente Liste**.

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >Intelligente Listen können erstaunliche Dinge tun. Weitere Informationen finden Sie unter [smart Liste Deep Dive](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md).

1. Suchen Sie nach dem Trigger und ziehen Sie ihn per Drag &amp; Drop auf die Arbeitsfläche.

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >Eine intelligente Kampagne mit Triggern wird im Trigger-Modus ausgeführt. Er wird auf der Grundlage von ausgelösten Ereignissen und hinzugefügten Filtern einzeln ausgeführt.

1. Klicken Sie auf die Dropdownliste **Name** und wählen Sie einen Operator aus.

   ![](assets/smart-list-dropdown-hands.png)

1. Definieren Sie den Trigger.

   ![](assets/smart-lislt-select-content-hands.png)

1. hinzufügen Sie die Beschränkung **Typ**.

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. Wählen Sie die Quelle aus, die Sie für Ihre intelligente Liste benötigen.

   ![](assets/pc-add-constraint.png)

1. Wenn Sie die E-Mail-Quelle für Ihren Prognoseinhalt verwenden, fügen Sie den Trigger **Klicks Link in E-Mail** hinzu. Wählen Sie Ihre E-Mail aus und fügen Sie die Beschränkung **Ist Vorhersagekraft** hinzu, die als **true** definiert ist.

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. hinzufügen Sie ggf. weitere Filter.

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >In einer klugen Kampagne mit Triggern und Filtern gehen die Trigger an die Spitze. Bei Auslösung durchlaufen nur Personen, die die Filterkriterien erfüllen, den Fluss.

   >[!NOTE]
   >
   >Bei mehreren Triggern durchläuft eine Person den Fluss, wenn einer der Trigger aktiviert wird.

   Um die Kampagne gleichzeitig für eine Gruppe von Personen auszuführen, erfahren Sie, wie Sie [eine intelligente Liste für eine intelligente Batch-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md) definieren.

   >[!MORELIKETHIS]
   >
   >* [Intelligente Liste für intelligente Kampagne definieren | Stapel](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [hinzufügen eines Flussschritts zu einer intelligenten Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [Definieren einer intelligenten Liste für Aktivitäten zur Web-Personalisierung](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [Predictive Content für Web Rich Media aktivieren](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [Symbolleiste für die Inhaltsempfehlung aktivieren](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)

