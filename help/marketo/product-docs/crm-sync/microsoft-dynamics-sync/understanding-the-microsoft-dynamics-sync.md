---
unique-page-id: 10098625
description: Die Microsoft Dynamics Sync - Marketo Docs - Produktdokumentation
title: Die Microsoft Dynamics Sync
translation-type: tm+mt
source-git-commit: 20d4c8a079916f47267df3dab5a8e663f6eb019b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Die Microsoft Dynamics Sync {#understanding-the-microsoft-dynamics-sync}

Marketo und Microsoft Dynamics gehen Hand in Hand. Wir halten Ihre Verkaufs- und Marketingdaten synchron.

>[!NOTE]
>
>Marketo unterstützt derzeit nur SSL-Zertifikate, die mit Java 7 kompatibel sind.

## Funktionsweise der Synchronisierung {#how-sync-works}

Marketo synchronisiert die Daten laufend mit Microsoft Dynamics. Es wird mithilfe der Hintergrundsynchronisierung, in Stapeln, nicht in Echtzeit durchgeführt.

>[!NOTE]
>
>Die erste Synchronisierung in Ihrem Abonnement dauert Minuten bis Stunden, je nach Datenbankgröße. Marketo kopiert die gesamte Datenbank von Dynamics. Danach dauert die Synchronisierung in der Regel Sekunden oder Minuten und es werden nur die geänderten Daten synchronisiert.

Die Synchronisierung zwischen Marketo und Dynamics erfolgt bidirektional für Kontakte und Kontakte. Wenn Sie Änderungen an Marketo oder Dynamics vornehmen, werden Ihre Updates in beiden Systemen übernommen. Alle anderen Bereiche, wie z.B. Konten und Chancen, werden nur auf eine Weise synchronisiert, von Dynamics bis Marketo.

## Was wird zwischen Marketo und Microsoft Dynamics synchronisiert? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Interessenten](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Kontakte](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Konten](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Benutzer](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Teams (Gruppen von SystemUsers)
* [Chancen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Benutzerdefinierte Entitäten](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-custom-entity-sync.md)

>[!NOTE]
>
>Die [Anmeldeinformationen, die Sie in Marketing for Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md) eingeben, werden zum Synchronisieren der Daten verwendet.

>[!CAUTION]
>
>Wir unterstützen derzeit keine Sandbox-Aktualisierung für Marketo Dynamics Sync. Wenn Sie Ihre Dynamics CRM-Sandbox aktualisieren müssen, benötigen Sie eine neue Marketo-Sandbox. Weitere Informationen erhalten Sie von Ihrem Kundenbetreuer.
