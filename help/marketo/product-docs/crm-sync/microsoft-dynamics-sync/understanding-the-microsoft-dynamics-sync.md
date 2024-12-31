---
unique-page-id: 10098625
description: Informationen zur Synchronisierung mit Microsoft Dynamics - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zur Synchronisierung mit Microsoft Dynamics
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 8%

---

# Grundlegendes zur Synchronisierung mit Microsoft Dynamics {#understanding-the-microsoft-dynamics-sync}

Marketo Engage und Microsoft Dynamics passen zusammen. Wir halten Ihre Verkaufs- und Marketingdaten synchron.

>[!NOTE]
>
>Marketo unterstützt derzeit nur SSL-Zertifikate, die mit Java 7 kompatibel sind.

>[!CAUTION]
>
>Wir unterstützen derzeit keine Sandbox-Aktualisierung für Marketo Dynamics Sync. Wenn Sie Ihre Dynamics CRM-Sandbox aktualisieren müssen, ist eine neue Marketo-Sandbox erforderlich. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).

## Funktionsweise der Synchronisierung {#how-sync-works}

Marketo synchronisiert Daten kontinuierlich den ganzen Tag, jeden Tag mit Microsoft Dynamics. Dies geschieht mithilfe der Hintergrundsynchronisierung, in Stapeln, nicht in Echtzeit.

>[!NOTE]
>
>Die erste Synchronisation in Ihrem Abonnement dauert je nach Größe Ihrer Datenbank Minuten bis Stunden. Marketo kopiert die gesamte Datenbank aus Dynamics. Danach dauert eine Synchronisation meist nur Sekunden oder Minuten; neu synchronisiert werden nur die Daten, die sich geändert haben.

Die Synchronisation zwischen Marketo und Dynamics erfolgt bidirektional für Leads und Kontakte. Wenn Sie Änderungen in Marketo oder Dynamics vornehmen, werden Ihre Aktualisierungen auf beiden Systemen angezeigt. Alle anderen Felder, z. B. Konten und Opportunities, werden nur in eine Richtung synchronisiert, von Dynamics bis Marketo.

## Was wird zwischen Marketo und Microsoft Dynamics synchronisiert? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Leads](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Kontakte](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Konten](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Benutzer](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Teams (Gruppen von Systembenutzern)
* [Opportunitys](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Benutzerdefinierte Entitäten](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

Die [Anmeldeinformationen, die Sie in Marketo für Dynamics eingeben](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) werden verwendet, um Daten zu synchronisieren.

>[!NOTE]
>
>Das Kopieren von Instanzen wird nicht unterstützt, wenn die Quellinstanz in Microsoft Dynamics integriert ist.
