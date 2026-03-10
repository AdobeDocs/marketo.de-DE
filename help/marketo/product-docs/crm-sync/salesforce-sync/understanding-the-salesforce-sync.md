---
unique-page-id: 4719283
description: Erfahren Sie, wie die Salesforce-Synchronisierung die Marketo- und Salesforce-Daten synchronisiert. Erfahren Sie, was synchronisiert wird und wie die bidirektionale Synchronisierung für Leads und Kontakte funktioniert.
title: Grundlegendes zur Salesforce-Synchronisierung
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 89%

---

# Grundlegendes zur [!DNL Salesforce]-Synchronisierung {#understanding-the-salesforce-sync}

Marketo Engage und Salesforce ergänzen sich außerordentlich gut. Ihre Vertriebs- und Marketing-Daten bleiben synchron. 

## Funktionsweise der Synchronisierung {#how-sync-works}

Marketo synchronisiert Tag für Tag mit [!DNL Salesforce]. Jede Synchronisierung dauert einige Zeit, wird dann 5 Minuten angehalten und anschließend erneut gestartet.

>[!NOTE]
>
>Die allererste Synchronisierung Ihres Abonnements dauert möglicherweise Stunden oder sogar Tage, da Marketo die gesamte Datenbank aus [!DNL Salesforce] kopiert. Danach dauert eine Synchronisation meist nur Sekunden oder Minuten; neu synchronisiert werden nur die Daten, die sich geändert haben.

![](assets/sync-illustration.png)

Die Synchronisierung zwischen [!DNL Salesforce] und Marketo ist nur für Leads, Kontakte und [!DNL Salesforce]-Kampagnen bidirektional. Wenn Sie in diesen Fällen Änderungen in [!DNL Salesforce] oder Marketo vornehmen, werden diese Aktualisierungen in beiden Systemen angezeigt. Alle anderen Daten werden nur von [!DNL Salesforce] nach Marketo synchronisiert. Klicken Sie auf die unten stehenden Links, um Details anzuzeigen.

## Was wird zwischen Marketo und [!DNL Salesforce] synchronisiert? {#what-is-synced-between-marketo-and-salesforce}

* [Leads](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md){target="_blank"}
* [Kontakte](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"}
* [Konten](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"}
* [Benutzende](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md){target="_blank"}
* [Opportunities](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md){target="_blank"}
* [Salesforce-Kampagnen](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
* [Benutzerdefinierte Objekte](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md){target="_blank"}
* [Aktivität](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md){target="_blank"}

>[!NOTE]
>
>Die [in Marketo für Salesforce eingegebenen Anmeldedaten](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} werden verwendet, um Daten zu synchronisieren. Es werden nur Daten einbezogen, auf die mit diesen Anmeldedaten zugegriffen werden kann.

Die Synchronisierung von Marketo mit [!DNL Salesforce] ist weltweit die leistungsstärkste ihrer Art. Sie wirkt wie Zauberei – eine Änderung wird vorgenommen und das andere System ist kurz darauf aktualisiert.
