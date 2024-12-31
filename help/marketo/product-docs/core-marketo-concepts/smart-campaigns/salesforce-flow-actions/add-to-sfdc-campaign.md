---
unique-page-id: 1147034
description: Hinzufügen zu SFDC Campaign - Marketo-Dokumente - Produktdokumentation
title: Zu SFDC-Kampagne hinzufügen
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 5%

---

# Zu SFDC-Kampagne hinzufügen {#add-to-sfdc-campaign}

Dieser Flussschritt kann in Marketo Engage-Kampagnen oder als einzelner Flussschritt verwendet werden, um Personen als Leads in einer Salesforce-Kampagne hinzuzufügen. Wenn der Lead noch nicht in Salesforce vorhanden ist, wird er automatisch synchronisiert und der Kampagne mit dem angegebenen Status hinzugefügt.

>[!NOTE]
>
>Nur verfügbar, wenn mit Salesforce integriert.

![](assets/add-to-sfdc-campaign-1.png)

## Nutzung {#usage}

1. Suchen Sie die Salesforce-Kampagne, der Sie Ihre Leads hinzufügen möchten, und wählen Sie sie aus.

   ![](assets/add-to-sfdc-campaign-2.png)

   >[!TIP]
   >
   >Wenn eine Salesforce-Kampagne nicht in der Kampagnenliste angezeigt wird:
   >
   >  1. Stellen Sie sicher[ dass die Kampagnensynchronisierung aktiviert ](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}.
   >  1. Vergewissern Sie sich, dass Ihr [Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}Synchronisierungsbenutzer[ ein „Marketing-](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}&quot; in Salesforce ist.

   >[!TIP]
   >
   >Sie können Salesforce Campaign [Meine Token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"} verwenden, um das Klonen von Programmen zu vereinfachen.

1. Wählen Sie den Salesforce-Kampagnenmitgliedsstatus aus, den Sie Leads zuweisen möchten, wenn sie hinzugefügt werden.

   ![](assets/add-to-sfdc-campaign-3.png)

   >[!CAUTION]
   >
   >Wenn eine Person bereits ein Lead-Mitglied der Salesforce-Kampagne ist, wird sie übersprungen und ihr Status wird NICHT aktualisiert. Sie können stattdessen [Status in einer SFDC-Kampagne ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"} verwenden.
