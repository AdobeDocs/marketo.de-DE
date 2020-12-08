---
unique-page-id: 1147034
description: hinzufügen zur SFDC-Kampagne - Marketing Docs - Produktdokumentation
title: hinzufügen an die SFDC-Kampagne
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# hinzufügen an die SFDC-Kampagne {#add-to-sfdc-campaign}

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

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
   >    
   >    
   >    1. Stellen Sie sicher, dass die Synchronisierung der [Kampagne aktiviert](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)ist.
   >    1. Vergewissern Sie sich, dass Ihr [MarketingTo-Sync-Benutzer](../../../../product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) ein [Marketing-Benutzer](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) in Salesforce ist.


   >[!TIP]
   >
   >Sie können Salesforce Kampagne [My Tokens](../../../../product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) verwenden, um das Klonen von Programmen zu erleichtern.

1. Wählen Sie den Salesforce-Mitgliedsstatus aus, den Sie Interessenten zuweisen möchten, wenn sie hinzugefügt werden.

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >Wenn eine Person bereits ein Interessentenmitglied der Salesforce-Kampagne ist, wird sie übersprungen und ihr Status wird NICHT aktualisiert. Sie können ihren Status in einer SFDC-Kampagne [](change-status-in-sfdc-campaign.md) ändern.

