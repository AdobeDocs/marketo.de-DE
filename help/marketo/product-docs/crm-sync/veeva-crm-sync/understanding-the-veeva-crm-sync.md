---
description: Verstehen der VEC CRM-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Grundlagen zur VEC CRM-Synchronisierung
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 1%

---

# Grundlagen zur VEC CRM-Synchronisierung {#understanding-the-veeva-crm-sync}

In wenigen Schritten ist es einfach, eine Synchronisation zwischen Adobe Marketo Engage und dem Veeva CRM durchzuführen.

## Funktionsweise der Synchronisierung {#how-the-sync-works}

Marketo Engage synchronisiert täglich mit Veeva CRM. Jede Synchronisation dauert einige Zeit, hält 5 Minuten an und beginnt dann erneut.

>[!NOTE]
>
>Die erste Synchronisation kann Stunden oder sogar Tage dauern, da Marketo Engage die gesamte Datenbank aus Veeva kopiert. Danach dauert jede Synchronisation in der Regel Minuten (manchmal Sekunden) und synchronisiert nur Daten, die sich geändert haben.

![](assets/understanding-the-veeva-sync-1.png)

Die Synchronisation zwischen VEE und Marketo Engage erfolgt nur für Kontaktfelder im Benutzerkontoobjekt. In diesen Fällen spiegeln sich Ihre Aktualisierungen in beiden Systemen wider, sobald Sie Änderungen in Veeva oder Marketo Engage vornehmen. Alle anderen Synchronisationen sind nur von Veeva nach Marketo Engage. Klicken Sie auf die folgenden Links, um Details zu den einzelnen Links zu erhalten.

## Was wird zwischen Marketo Engage und Veeva synchronisiert? {#what-is-synced-between-marketo-engage-and-veeva}

* [Personenkonten](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target="_blank"}
* Benutzer
* [Schlüsselobjekte aufrufen und aufrufen](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
* [Benutzerdefinierte Objekte](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

## Was zu wissen ist {#things-to-know}

* Die [Anmeldedaten, die Sie im Marketo Engage für Veeva eingeben](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} werden zum Synchronisieren von Daten verwendet. Es werden nur Daten einbezogen, auf die diese Anmeldeinformationen Zugriff haben.

* Veeva CRM basiert auf force.com und das Rich-Experience-Marketo Engage mit der Plattform wird in diese Synchronisation übernommen.

* Das VEE-CRM zeigt Lead, Kontakt, Konten (Geschäftskonten, Chancen, Kampagne und Aktivität. Sie werden jedoch nicht in der Synchronisierung mit Marketo Engage unterstützt.
