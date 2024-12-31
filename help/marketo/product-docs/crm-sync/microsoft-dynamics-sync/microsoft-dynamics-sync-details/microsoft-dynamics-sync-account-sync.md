---
unique-page-id: 3571836
description: Microsoft Dynamics-Synchronisierung - Kontosynchronisierung - Marketo-Dokumente - Produktdokumentation
title: Microsoft Dynamics-Synchronisierung - Kontosynchronisierung
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Microsoft Dynamics-Synchronisierung: Kontosynchronisierung {#microsoft-dynamics-sync-account-sync}

Wussten Sie, dass Marketo Engage Ihre gesamte Datenbank mit Dynamics synchronisiert? Er synchronisiert, wartet dann 5 Minuten und synchronisiert dann erneut, den ganzen Tag, jeden Tag. Im Folgenden finden Sie einige Details dazu, wie Marketo Dynamics-Konten spezifisch behandelt.

## Auf welche Weise werden die Informationen synchronisiert? {#which-way-does-the-information-sync}

Nur eine Möglichkeit: von Dynamics zu Marketo.

## Wie funktionieren die Aktualisierungen? {#how-do-the-updates-work}

Wenn Sie ein Kontofeld für einen Kontakt in Marketo aktualisieren, werden die Werte aller Kontakte geändert, die zu diesem Konto in Marketo gehören. Es wird nicht mit Dynamics synchronisiert. Wenn dieses Konto jedoch das nächste Mal in Dynamics aktualisiert wird, überschreiben die Änderungen alle Kontoinformationen in Marketo.

## Kann ich mit Marketo ein Konto erstellen? {#can-i-create-an-account-using-marketo}

Nein. Marketo kann keine Konten in Dynamics erstellen.

## Welche Felder werden mit Marketo synchronisiert? {#which-fields-will-sync-to-marketo}

Sie können [ Setup Felder auswählen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} die synchronisiert werden sollen. Marketo synchronisiert jedoch nur die Felder, auf die der Dynamics-Synchronisierungsbenutzer Zugriff hat.

## Führt eine Änderung an einem Kontofeld in Dynamics zu einem Aktivitätsprotokoll „Datenwert ändern“ für jeden Kontakt?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

Meistens ja. Wenn ein Konto jedoch mehr als 5.000 Kontakte hat und sich ein Feld in Dynamics ändert, synchronisieren wir die Änderung, protokollieren jedoch nicht die Aktivität für die über 5.000 Kontakte.
