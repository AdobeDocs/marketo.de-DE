---
unique-page-id: 4719283
description: Erläuterungen zur Salesforce-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Erläuterungen zur Salesforce-Synchronisierung
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 10%

---

# Erläuterungen zur Salesforce-Synchronisierung {#understanding-the-salesforce-sync}

Marketo und Salesforce vereinen sich wie Erbsen und Karotten. Wir halten Ihre Verkaufs- und Marketingdaten synchron.

## Funktionsweise der Synchronisierung {#how-sync-works}

Marketo synchronisiert jeden Tag mit Salesforce. Jede Synchronisation dauert einige Zeit, hält dann 5 Minuten an und beginnt dann erneut.

>[!NOTE]
>
>Die allererste Synchronisation in Ihrem Abonnement kann Stunden oder sogar Tage dauern, da Marketo die gesamte Datenbank aus Salesforce kopiert. Danach dauert eine Synchronisation meist nur Sekunden oder Minuten; neu synchronisiert werden nur die Daten, die sich geändert haben.

![](assets/sync-illustration.png)

Die Synchronisierung zwischen Salesforce und Marketo erfolgt nur für Leads, Kontakte und Salesforce-Kampagnen bidirektional. In diesen Fällen spiegeln sich Ihre Aktualisierungen in beiden Systemen wider, sobald Sie Änderungen in Salesforce oder Marketo vornehmen. Alle anderen Synchronisationen stammen nur von Salesforce bis Marketo. Klicken Sie auf die folgenden Links, um Details zu den einzelnen Links zu erhalten.

## Was wird zwischen Marketo und Salesforce synchronisiert? {#what-is-synced-between-marketo-and-salesforce}

* [Leads](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md)
* [Kontakte](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)
* [Konten](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)
* [Benutzer](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [Opportunities](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Salesforce Kampagnen](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [Benutzerdefinierte Objekte](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [Aktivität](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>Die [Anmeldedaten, die Sie in Marketo für Salesforce eingeben](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) werden zum Synchronisieren von Daten verwendet. Es werden nur Daten einbezogen, auf die diese Anmeldeinformationen Zugriff haben.

Die Synchronisation von Marketo mit Salesforce ist die leistungsfähigste dieser Art auf der Welt. Es fühlt sich wie Zauberei an, es wird eine Veränderung vorgenommen und das andere System ist bald auf dem neuesten Stand.
