---
unique-page-id: 3571838
description: Microsoft Dynamics Sync -Field Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - Feldsynchronisierung
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Feldsynchronisierung {#microsoft-dynamics-sync-field-sync}

Marketo to Dynamics sync ist super leistungsfähig. Hier sind die Details.

## Wie werden die Felddetails zwischen den beiden Systemen synchronisiert? {#how-are-field-details-kept-in-sync-between-the-two-systems}

Die Synchronisierung erfolgt bidirektional für Interessenten- und Kontaktstellen. Wenn Sie Änderungen an einem Lead oder Kontakt in Dynamics oder einer Person in Marketo vornehmen, werden Ihre Updates in beiden Systemen übernommen.

Für Konto-, Benutzer-, Gelegenheit-, Team- und benutzerdefinierte Entitäten erfolgt die Synchronisierung nur in einer Richtung: Dynamik nach Marketo. Wenn Sie Änderungen an diesen Entitäten in Dynamics vornehmen, werden Ihre Updates in Marketo angezeigt.

## Was ist, wenn in beiden Systemen gleichzeitig Änderungen am gleichen Feld vorgenommen werden? (Datenkollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Obwohl dies selten geschieht, wird Marketo für Menschen (Interessenten) gewinnen und Dynamics für Kontakte gewinnen. Das liegt daran, dass wir die Marketingabteilung für Menschen als maßgeblich betrachten, während das offizielle System der Kontaktaufnahme in der Verkaufsabteilung (CRM) besteht. Bei einseitigen Synchronisierungsentitäten gewinnt Dynamics immer.

## Kann ich mit Marketo ein Feld in Dynamics erstellen? {#can-i-create-a-field-in-dynamics-using-marketo}

Nein, dies wird derzeit nicht unterstützt.

## Ich schuf ein Feld in Dynamics. Kann ich es mit Marketo synchronisieren? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Ja, Sie können [das Feld](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) synchronisieren, solange Ihr Synchronisierungsbenutzer Zugriff darauf in Dynamics hat.

## Welche Felder werden mit Marketo synchronisiert? {#what-fields-will-sync-to-marketo}

Sie können die zu synchronisierenden Felder [während des Setups auswählen.](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)

## Was ist, wenn ich nach der Synchronisierung von Marketo und Dynamics ein benutzerdefiniertes Feld hinzufügen muss? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Sie können jederzeit Felder hinzufügen und erwarten, dass die Daten von Dynamics bis Marketo aktualisiert werden. Weitere Informationen finden Sie unter [Schnellsynchronisierung mit Microsoft Dynamics verwenden für ein neues benutzerdefiniertes Feld](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md).

## Was ist, wenn ich ein Feld in Dynamics löschen möchte, nachdem das Feld zur Synchronisierung hinzugefügt wurde? {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo speichert einen Verweis auf die zu synchronisierenden Felder. Wenn Sie ein Feld in Dynamics löschen, wird empfohlen, dies mit [sync deaktiviert](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md) zu tun. Aktualisieren Sie dann das Schema in Marketo, indem Sie die Felder [Zu synchronisierende Felder auswählen bearbeiten und speichern.](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md)
