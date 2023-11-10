---
unique-page-id: 10098625
description: Grundlegendes zur Microsoft Dynamics-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Grundlagen zur Synchronisierung von Microsoft Dynamics
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 8%

---

# Grundlagen zur Synchronisierung von Microsoft Dynamics {#understanding-the-microsoft-dynamics-sync}

Marketo Engage und Microsoft Dynamics gehen Hand in Hand. Wir halten Ihre Verkaufs- und Marketingdaten synchron.

>[!NOTE]
>
>Marketo unterstützt derzeit nur SSL-Zertifikate, die mit Java 7 kompatibel sind.

>[!CAUTION]
>
>Sandbox-Aktualisierung für Marketo Dynamics Sync wird derzeit nicht unterstützt. Wenn Sie Ihre Dynamics CRM-Sandbox aktualisieren müssen, ist eine neue Marketo-Sandbox erforderlich. Weitere Informationen erhalten Sie vom Adobe Account Team (Ihrem Kundenbetreuer).

## Funktionsweise der Synchronisierung {#how-sync-works}

Marketo synchronisiert Daten kontinuierlich und täglich mit Microsoft Dynamics. Dies erfolgt über die Hintergrundsynchronisierung, in Stapeln, nicht in Echtzeit.

>[!NOTE]
>
>Die allererste Synchronisation in Ihrem Abonnement dauert je nach Größe Ihrer Datenbank Minuten bis Stunden. Marketo kopiert die gesamte Datenbank aus Dynamics. Danach dauert eine Synchronisation meist nur Sekunden oder Minuten; neu synchronisiert werden nur die Daten, die sich geändert haben.

Die Synchronisation zwischen Marketo und Dynamics erfolgt bidirektional für Leads und Kontakte. Wenn Sie Änderungen in Marketo oder Dynamics vornehmen, werden Ihre Aktualisierungen in beiden Systemen übernommen. Alle anderen Felder, wie Konten und Chancen, werden nur auf eine Weise synchronisiert, von Dynamics bis Marketo.

## Was wird zwischen Marketo und Microsoft Dynamics synchronisiert? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Leads](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Kontakte](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Konten](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Benutzer](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Teams (Gruppen von System-Benutzern)
* [Opportunitys](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Benutzerdefinierte Entitäten](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

Die [Anmeldedaten, die Sie in Marketo für Dynamics eingeben](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) werden zum Synchronisieren von Daten verwendet.

>[!NOTE]
>
>Die Instanzkopie wird nicht unterstützt, wenn die Quellinstanz in Microsoft Dynamics integriert ist.
