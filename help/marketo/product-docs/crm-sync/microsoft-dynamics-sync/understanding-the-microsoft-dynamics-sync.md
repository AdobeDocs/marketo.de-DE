---
unique-page-id: 10098625
description: Grundlegendes zur  [!DNL Microsoft Dynamics] -Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zur Synchronisierung mit Microsoft Dynamics
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 9%

---

# Grundlegendes zur [!DNL Microsoft Dynamics] {#understanding-the-microsoft-dynamics-sync}

Marketo und [!DNL Microsoft Dynamics] gehen zusammen. Wir halten Ihre Verkaufs- und Marketingdaten synchron.

>[!NOTE]
>
>Marketo unterstützt derzeit nur SSL-Zertifikate, die mit Java 7 kompatibel sind.

>[!CAUTION]
>
>Wir unterstützen derzeit keine Sandbox-Aktualisierung für die [!DNL Marketo Dynamics]. Wenn Sie Ihre [!DNL Dynamics] CRM-Sandbox aktualisieren müssen, ist eine neue Marketo-Sandbox erforderlich. Weitere Informationen erhalten Sie von Ihrem Customer Success Manager.

## Funktionsweise der Synchronisierung {#how-sync-works}

Marketo synchronisiert Daten kontinuierlich jeden Tag mit [!DNL Microsoft Dynamics]. Dies geschieht mithilfe der Hintergrundsynchronisierung, in Stapeln, nicht in Echtzeit.

>[!NOTE]
>
>Die erste Synchronisation in Ihrem Abonnement dauert je nach Größe Ihrer Datenbank Minuten bis Stunden. Marketo kopiert die gesamte Datenbank aus [!DNL Dynamics]. Danach dauert eine Synchronisation meist nur Sekunden oder Minuten; neu synchronisiert werden nur die Daten, die sich geändert haben.

Die Synchronisation zwischen Marketo und [!DNL Dynamics] erfolgt bidirektional für Leads und Kontakte. Wenn Sie Änderungen in Marketo oder [!DNL Dynamics] vornehmen, werden die Aktualisierungen auf beiden Systemen angezeigt. Alle anderen Felder, z. B. Konten und Opportunities, werden nur in eine Richtung synchronisiert, von [!DNL Dynamics] bis Marketo.

## Was wird zwischen Marketo und [!DNL Microsoft Dynamics] synchronisiert? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Leads](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Kontakte](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Konten](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Benutzer](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Teams (Gruppen von Systembenutzern)
* [Opportunitys](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Benutzerdefinierte Entitäten](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

Die [Anmeldeinformationen, die Sie in Marketo für eingeben [!DNL Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) werden verwendet, um Daten zu synchronisieren.

>[!NOTE]
>
>Eine Instanzkopie wird nicht unterstützt, wenn die Quellinstanz in [!DNL Microsoft Dynamics] integriert ist.
