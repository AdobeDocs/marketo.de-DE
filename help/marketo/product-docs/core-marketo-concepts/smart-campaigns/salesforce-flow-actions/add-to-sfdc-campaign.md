---
unique-page-id: 1147034
description: hinzufügen zur SFDC-Kampagne - Marketo Docs - Produktdokumentation
title: Zu SFDC-Kampagne hinzufügen
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 5%

---

# Der SFDC-Kampagne hinzufügen {#add-to-sfdc-campaign}

>[!NOTE]
>
>Nur verfügbar, wenn in Salesforce integriert.

## Übersicht {#overview}

Dieser Flussschritt kann in Marketo-Kampagnen oder als einzelner Flussschritt verwendet werden, um Personen als Interessenten in einer Salesforce-Kampagne hinzuzufügen. Wenn der Interessent noch nicht in Salesforce vorhanden ist, wird er automatisch synchronisiert und der Kampagne mit dem angegebenen Status hinzugefügt.

![](assets/image2014-9-22-15-3a43-3a36.png)

## Nutzung {#usage}

1. Suchen und wählen Sie die Salesforce-Kampagne aus, der Sie Ihre Interessenten hinzufügen möchten.

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >Wenn in der Liste Kampagne keine Salesforce-Kampagne angezeigt wird:
   >
   >  1. Vergewissern Sie sich, dass [Kampagne-Synchronisierung aktiviert ist](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
   >  1. Vergewissern Sie sich, dass der [Marketo Sync User](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) ein [Marketing-Benutzer](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) in Salesforce ist.


   >[!TIP]
   >
   >Sie können die Salesforce-Kampagne [My Tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) verwenden, um das Klonen von Programmen zu vereinfachen.

1. Wählen Sie den Salesforce-Mitgliedsstatus aus, den Sie Interessenten zuweisen möchten, wenn sie hinzugefügt werden.

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >Wenn eine Person bereits ein Interessentenmitglied der Salesforce-Kampagne ist, wird sie übersprungen und ihr Status wird NICHT aktualisiert. Sie können stattdessen [ihren Status in einer SFDC-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md) ändern.
