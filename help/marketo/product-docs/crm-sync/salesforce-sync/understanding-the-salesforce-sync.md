---
unique-page-id: 4719283
description: Die Salesforce-Synchronisierung - Marketo Docs - Produktdokumentation
title: Die Salesforce-Synchronisierung
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 10%

---

# Die Salesforce-Synchronisierung {#understanding-the-salesforce-sync}

Marketo und Salesforce gehen wie Erbsen und Karotten zusammen. Wir halten Ihre Verkaufs- und Marketingdaten synchron.

## Funktionsweise der Synchronisierung {#how-sync-works}

Marketo synchronisiert jeden Tag mit Salesforce. Jede Synchronisierung dauert einige Zeit und hält dann 5 Minuten an, dann werden die Beginn erneut angehalten.

>[!NOTE]
>
>Die erste Synchronisierung in Ihrem Abonnement kann Stunden oder sogar Tage dauern, da Marketo die gesamte Datenbank von Salesforce kopiert. Danach dauert eine Synchronisation meist nur Sekunden oder Minuten; neu synchronisiert werden nur die Daten, die sich geändert haben.

![](assets/sync-illustration.png)

Die Synchronisierung zwischen Salesforce und Marketo erfolgt bidirektional nur für Interessenten, Kontakte und Salesforce-Kampagnen. In diesen Fällen werden Ihre Updates bei jeder Änderung in Salesforce oder Marketo in beiden Systemen angezeigt. Alle anderen Syncs sind nur von Salesforce bis Marketo. Klicken Sie auf die unten stehenden Links, um Einzelheiten zu den einzelnen Links anzuzeigen.

## Was wird zwischen Marketo und Salesforce synchronisiert? {#what-is-synced-between-marketo-and-salesforce}

* [Leads](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md)
* [Kontakte](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)
* [Konten](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)
* [Benutzer](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [Opportunities](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Salesforce-Kampagnen](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [Benutzerdefinierte Objekte](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [Aktivität](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>Die [Anmeldedaten, die Sie in Marketo für Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) eingeben, werden zum Synchronisieren der Daten verwendet. Es werden nur Daten einbezogen, auf die diese Anmeldeinformationen Zugriff haben.

Die Synchronisierung Marketos mit Salesforce ist die leistungsstärkste seiner Art auf der Welt. Es fühlt sich wie Zauberei an. Es wird eine Änderung vorgenommen und das andere System ist bald auf dem neuesten Stand.
