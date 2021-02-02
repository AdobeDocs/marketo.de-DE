---
unique-page-id: 4719283
description: Die Salesforce-Synchronisierung - Marketing Docs - Produktdokumentation
title: Die Salesforce-Synchronisierung
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Die Salesforce-Synchronisierung {#understanding-the-salesforce-sync}

Marketo und Salesforce verbinden sich wie Erbsen und Karotten. Wir halten Ihre Verkaufs- und Marketingdaten synchron.

## Funktionsweise der Synchronisierung {#how-sync-works}

Marketo synchronisiert jeden Tag mit Salesforce. Jede Synchronisierung dauert einige Zeit und hält dann 5 Minuten an, dann werden die Beginn erneut angehalten.

>[!NOTE]
>
>Die erste Synchronisierung in Ihrem Abonnement kann Stunden oder sogar Tage dauern, da Marketo die gesamte Datenbank aus Salesforce kopiert. Danach dauert die Synchronisierung in der Regel Sekunden oder Minuten und es werden nur die geänderten Daten synchronisiert.

![](assets/sync-illustration.png)

Die Synchronisierung zwischen Salesforce und Marketo erfolgt bidirektional nur für Interessenten, Kontakte und Salesforce-Kampagnen. In diesen Fällen werden Ihre Aktualisierungen bei Änderungen in Salesforce oder Marketo in beiden Systemen übernommen. Alle anderen Syncs sind nur von Salesforce bis Marketo. Klicken Sie auf die unten stehenden Links, um Einzelheiten zu den einzelnen Links anzuzeigen.

## Was wird zwischen Marketo und Salesforce synchronisiert? {#what-is-synced-between-marketo-and-salesforce}

* [Interessenten](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md)
* [Kontakte](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)
* [Konten](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)
* [Benutzer](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [Chancen](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Salesforce-Kampagnen](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [Benutzerdefinierte Objekte](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [Aktivität](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>Die [Anmeldedaten, die Sie in Marketo für Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) eingeben, werden zum Synchronisieren der Daten verwendet. Es werden nur Daten einbezogen, auf die diese Anmeldeinformationen Zugriff haben.

Marketo&#39;s Synchronisierung mit Salesforce ist die mächtigste seiner Art auf der Welt. Es fühlt sich wie Zauberei an. Es wird eine Änderung vorgenommen und das andere System ist bald auf dem neuesten Stand.
