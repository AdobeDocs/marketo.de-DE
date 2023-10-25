---
unique-page-id: 3571838
description: Microsoft Dynamics Sync - Feldsynchronisierung - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - Feldsynchronisierung
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Feldsynchronisierung {#microsoft-dynamics-sync-field-sync}

Marketo Engage to Dynamics Synchronisation ist super leistungsstark. Hier sind die Details.

## Wie werden Felddetails zwischen den beiden Systemen synchronisiert? {#how-are-field-details-kept-in-sync-between-the-two-systems}

Die Synchronisierung erfolgt bidirektional für Lead- und Kontaktentitäten. Wenn Sie Änderungen an einem Lead oder Kontakt in Dynamics oder einer Person in Marketo vornehmen, werden Ihre Aktualisierungen in beiden Systemen angezeigt.

Bei Konto-, Benutzer-, Opportunities-, Team- und benutzerdefinierten Entitäten erfolgt die Synchronisierung unidirektional: Dynamics zu Marketo. Wenn Sie in Dynamics Änderungen an diesen Entitäten vornehmen, werden Ihre Aktualisierungen in Marketo übernommen.

## Was passiert, wenn in beiden Systemen gleichzeitig Änderungen an demselben Feld vorgenommen werden? (Datenkollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Obwohl dies selten vorkommt, gewinnt Marketo für Personen (Leads) und Dynamics gewinnt für Kontakte. Dies liegt daran, dass wir die Marketing-Abteilung für Menschen als maßgeblich betrachten, während das offizielle System der Kontaktaufnahme in der Vertriebs- (CRM-) Abteilung ist. Bei unidirektionalen Synchronisierungsentitäten gewinnt Dynamics immer.

## Kann ich mit Marketo ein Feld in Dynamics erstellen? {#can-i-create-a-field-in-dynamics-using-marketo}

Nein, dies wird derzeit nicht unterstützt.

## Ich habe ein Feld in Dynamics erstellt. Kann ich es mit Marketo synchronisieren? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Ja, Sie können [Feld synchronisieren](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} solange Ihr Synchronisierungsbenutzer Zugriff darauf in Dynamics hat.

## Welche Felder werden mit Marketo synchronisiert? {#what-fields-will-sync-to-marketo}

Sie können [Auswahl der zu synchronisierenden Felder](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} während der Einrichtung.

## Was passiert, wenn ich nach der Synchronisierung von Marketo und Dynamics ein benutzerdefiniertes Feld hinzufügen muss? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Sie können jederzeit Felder hinzufügen und erwarten, dass die Daten von Dynamics in Marketo aktualisiert werden. Siehe [Verwenden der Schnellsynchronisierung mit Microsoft Dynamics für ein neues benutzerdefiniertes Feld](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md){target="_blank"} für Details.

## Was passiert, wenn ich ein Feld in Dynamics löschen möchte, nachdem das Feld zur Synchronisierung hinzugefügt wurde? {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo speichert einen Verweis auf die zu synchronisierenden Felder. Wenn Sie ein Feld in Dynamics löschen, wird empfohlen, dies mit der [Synchronisieren deaktiviert](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}. Then refresh the schema in Marketo by editing and saving the [Select Fields to Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}.
