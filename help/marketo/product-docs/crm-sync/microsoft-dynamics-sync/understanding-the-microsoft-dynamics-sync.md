---
unique-page-id: 10098625
description: Die Microsoft Dynamics Sync - Marketo Docs - Produktdokumentation
title: Die Microsoft Dynamics Sync
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '276'
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

* [Interessenten](microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Kontakte](microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Konten](microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Benutzer](microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Teams (Gruppen von SystemUsers)
* [Chancen](microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Benutzerdefinierte Entitäten](microsoft-dynamics-sync-details/microsoft-dynamics-sync-custom-entity-sync.md)

>[!NOTE]
>
>Die [Anmeldeinformationen, die Sie in Marketo für Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md) eingeben, werden zum Synchronisieren der Daten verwendet.

Es gibt viele Nuancen und Features über Dynamics sync. Sehen Sie sich die Details im Bereich [Microsoft Dynamics Sync Details an](http://docs.marketo.com/display/docs/microsoft+dynamics+sync+details).

>[!CAUTION]
>
>Wir unterstützen derzeit keine Sandbox-Aktualisierung für Marketo Dynamics Sync. Wenn Sie Ihre Dynamics CRM-Sandbox aktualisieren müssen, benötigen Sie eine neue Marketo-Sandbox. Weitere Informationen erhalten Sie von Ihrem Kundenbetreuer.

>[!MORELIKETHIS]
>
>* [Synchronisierungseinstellungen](http://docs.marketo.com/display/docs/sync+setup)
   >
   >
* [Microsoft Dynamics-Synchronisierungsdetails](http://docs.marketo.com/display/docs/microsoft+dynamics+sync+details)

