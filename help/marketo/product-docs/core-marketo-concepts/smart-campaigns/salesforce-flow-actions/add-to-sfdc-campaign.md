---
unique-page-id: 1147034
description: Zu SFDC Campaign hinzufügen - Marketo Docs - Produktdokumentation
title: Zu SFDC-Kampagne hinzufügen
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 5%

---

# Zu SFDC-Kampagne hinzufügen {#add-to-sfdc-campaign}

>[!NOTE]
>
>Nur verfügbar bei Integration mit Salesforce.

## Überblick {#overview}

Dieser Flussschritt kann in Marketo-Kampagnen oder als Einzeldurchsatzschritt verwendet werden, um Personen als Leads in einer Salesforce-Kampagne hinzuzufügen. Wenn der Lead noch nicht in Salesforce vorhanden ist, wird er automatisch synchronisiert und der Kampagne mit dem angegebenen Status hinzugefügt.

![](assets/image2014-9-22-15-3a43-3a36.png)

## Nutzung {#usage}

1. Suchen und wählen Sie die Salesforce-Kampagne aus, der Sie Ihre Leads hinzufügen möchten.

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >Wenn eine Salesforce-Kampagne nicht in der Kampagnenliste angezeigt wird:
   >
   >  1. Stellen Sie sicher, dass [Kampagnensynchronisation ist aktiviert](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}.
   >  1. Vergewissern Sie sich, dass [Marketo Sync User](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} is a [Marketing User](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"} in Salesforce.

   >[!TIP]
   >
   >Sie können Salesforce-Kampagne verwenden [Meine Token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"} um das Klonen von Programmen zu erleichtern.

1. Wählen Sie den Salesforce-Kampagnenstatus aus, den Sie Leads zuweisen möchten, wenn sie hinzugefügt werden.

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >Wenn eine Person bereits Lead-Mitglied der Salesforce-Kampagne ist, wird sie übersprungen und ihr Status wird NICHT aktualisiert. Sie können [Status in einer SFDC-Kampagne ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"} anstatt.
