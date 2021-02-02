---
unique-page-id: 3571838
description: Microsoft Dynamics Sync -Field Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - Feldsynchronisierung
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Feldsynchronisierung {#microsoft-dynamics-sync-field-sync}

Marketo to to Dynamics sync ist super leistungsfähig. Hier sind die Details.

## Wie werden die Felddetails zwischen den beiden Systemen synchronisiert? {#how-are-field-details-kept-in-sync-between-the-two-systems}

Die Synchronisierung erfolgt bidirektional für Interessenten- und Kontaktstellen. Wenn Sie Änderungen an einem Lead oder Kontakt in Dynamics oder einer Person in Marketo vornehmen, werden Ihre Updates in beiden Systemen übernommen.

Für Konto-, Benutzer-, Gelegenheit-, Team- und benutzerdefinierte Entitäten erfolgt die Synchronisierung nur in einer Richtung: Dynamik zu Marketo. Wenn Sie Änderungen an diesen Entitäten in Dynamics vornehmen, werden Ihre Updates in Marketo übernommen.

## Was ist, wenn in beiden Systemen gleichzeitig Änderungen am gleichen Feld vorgenommen werden? (Datenkollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Obwohl dies selten ist, wird Marketo gewinnen für Menschen (Interessenten) und Dynamics für Kontakte gewinnen. Das liegt daran, dass wir die Marketingabteilung für Menschen als maßgeblich betrachten, während das offizielle System der Kontaktaufnahme in der Verkaufsabteilung (CRM) besteht. Bei einseitigen Synchronisierungsentitäten gewinnt Dynamics immer.

## Kann ich mit Marketo ein Feld in Dynamics erstellen? {#can-i-create-a-field-in-dynamics-using-marketo}

Nein, dies wird derzeit nicht unterstützt.

## Ich schuf ein Feld in Dynamics. Kann ich es mit Marketo synchronisieren? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Ja, Sie können [das Feld](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) synchronisieren, solange Ihr Synchronisierungsbenutzer Zugriff darauf in Dynamics hat.

Welche Felder werden mit Marketo synchronisiert?

Sie können die zu synchronisierenden Felder [während des Setups auswählen.](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)

## Was ist, wenn ich nach der Synchronisierung von Marketo und Dynamics ein benutzerdefiniertes Feld hinzufügen muss? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Sie können jederzeit Felder hinzufügen und erwarten, dass die Daten von Dynamics zu Marketo aktualisiert werden. Weitere Informationen finden Sie unter [Schnellsynchronisierung mit Microsoft Dynamics verwenden für ein neues benutzerdefiniertes Feld](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md).
