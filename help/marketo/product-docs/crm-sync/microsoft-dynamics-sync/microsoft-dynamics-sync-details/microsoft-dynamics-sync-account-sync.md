---
unique-page-id: 3571836
description: Synchronisation von Microsoft Dynamics - Kontosynchronisierung - Marketo-Dokumente - Produktdokumentation
title: Synchronisation von Microsoft Dynamics - Kontosynchronisierung
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Kontosynchronisierung {#microsoft-dynamics-sync-account-sync}

Wussten Sie, dass Marketo Engage Ihre gesamte Datenbank mit Dynamics synchronisiert? Es wird synchronisiert, dann 5 Minuten wartet und dann wieder synchronisiert, den ganzen Tag, jeden Tag. Im Folgenden finden Sie einige Details dazu, wie Marketo Dynamics-Konten spezifisch behandelt.

## Wie werden die Informationen synchronisiert? {#which-way-does-the-information-sync}

Nur eine Möglichkeit: von Dynamics bis Marketo.

## Wie funktionieren die Aktualisierungen? {#how-do-the-updates-work}

Wenn Sie ein Feld &quot;Konto&quot;für einen Kontakt in Marketo aktualisieren, werden die Werte aller Kontakte geändert, die zu diesem Konto in Marketo gehören. Es wird nicht mit Dynamics synchronisiert. Wenn dieses Konto jedoch das nächste Mal in Dynamics aktualisiert wird, werden alle Kontoinformationen in Marketo durch die Änderungen überschrieben.

## Kann ich mit Marketo ein Konto erstellen? {#can-i-create-an-account-using-marketo}

Anz. Marketo kann keine Konten in Dynamics erstellen.

## Welche Felder werden mit Marketo synchronisiert? {#which-fields-will-sync-to-marketo}

Sie können [ Felder auswählen, die während der Einrichtung synchronisiert werden sollen. ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} Marketo synchronisiert jedoch nur die Felder, auf die der Benutzer für die Synchronisierung mit Dynamics Zugriff hat.

## Führt eine Änderung in einem Kontofeld in Dynamics zu einem Aktivitätsprotokoll zum Datenwert ändern für jeden Kontakt?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

Meistens ja. Wenn jedoch ein Konto über mehr als 5.000 Kontakte verfügt und sich ein Feld in diesem Konto in Dynamics ändert, wird die Änderung synchronisiert, aber die Aktivität für mehr als 5.000 Kontakte wird nicht protokolliert.
