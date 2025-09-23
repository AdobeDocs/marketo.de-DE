---
unique-page-id: 4719283
description: Informationen zur Synchronisierung mit Salesforce - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zur Salesforce-Synchronisierung
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 10%

---

# Grundlegendes zur [!DNL Salesforce] {#understanding-the-salesforce-sync}

Marketo Engage und Salesforce passen gut zusammen wie Erbsen und Karotten. Wir halten Ihre Verkaufs- und Marketingdaten synchron.

## Funktionsweise der Synchronisierung {#how-sync-works}

Marketo synchronisiert mit [!DNL Salesforce] Tag für Tag. Jede Synchronisierung dauert einige Zeit, wird dann 5 Minuten angehalten und dann erneut gestartet.

>[!NOTE]
>
>Die erste Synchronisierung in Ihrem Abonnement kann Stunden oder sogar Tage dauern, da Marketo die gesamte Datenbank aus [!DNL Salesforce] kopiert. Danach dauert eine Synchronisation meist nur Sekunden oder Minuten; neu synchronisiert werden nur die Daten, die sich geändert haben.

![](assets/sync-illustration.png)

Die Synchronisation zwischen [!DNL Salesforce] und Marketo erfolgt nur für Leads, Kontakte und [!DNL Salesforce]. In diesen Fällen werden Ihre Aktualisierungen bei jeder Änderung, die Sie an [!DNL Salesforce] oder Marketo vornehmen, auf beiden Systemen angezeigt. Alle anderen Synchronisierungen werden nur von [!DNL Salesforce] nach Marketo durchgeführt. Klicken Sie auf die unten stehenden Links, um Details zu jedem anzuzeigen.

## Was wird zwischen Marketo und [!DNL Salesforce] synchronisiert? {#what-is-synced-between-marketo-and-salesforce}

* [Leads](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md){target="_blank"}
* [Kontakte](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"}
* [Konten](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"}
* [Benutzer](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md){target="_blank"}
* [Opportunities](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md){target="_blank"}
* [Salesforce-Kampagnen](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
* [Benutzerdefinierte Objekte](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md){target="_blank"}
* [Aktivität](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md){target="_blank"}

>[!NOTE]
>
>Die [Anmeldeinformationen, die Sie in Marketo für Salesforce eingeben](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} werden verwendet, um Daten zu synchronisieren. Nur Daten, auf die diese Anmeldeinformationen Zugriff haben, werden einbezogen.

Marketos Synchronisation mit [!DNL Salesforce] ist die leistungsstärkste ihrer Art auf der Welt. Es fühlt sich wie Zauberei an; eine Änderung wird vorgenommen und das andere System ist bald auf dem neuesten Stand.
