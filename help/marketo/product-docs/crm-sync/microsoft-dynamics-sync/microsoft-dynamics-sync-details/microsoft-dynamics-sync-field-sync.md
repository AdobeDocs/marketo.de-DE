---
unique-page-id: 3571838
description: Microsoft Dynamics-Synchronisierung - Feldsynchronisierung - Marketo-Dokumente - Produktdokumentation
title: Microsoft Dynamics-Synchronisierung - Feldsynchronisierung
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics]: Feldsynchronisierung {#microsoft-dynamics-sync-field-sync}

Die Synchronisierung von Marketo zu [!DNL Dynamics] ist extrem leistungsstark. Im Folgenden finden Sie die Details.

## Wie werden die Felddetails zwischen den beiden Systemen synchron gehalten? {#how-are-field-details-kept-in-sync-between-the-two-systems}

Die Synchronisierung erfolgt bidirektional für Lead- und Kontaktentitäten. Wenn Sie Änderungen an einem Lead oder Kontakt in [!DNL Dynamics] oder an einer Person in Marketo vornehmen, werden Ihre Aktualisierungen in beiden Systemen angezeigt.

Für Konto-, Benutzer-, Opportunity-, Team- und benutzerdefinierte Entitäten erfolgt die Synchronisierung in eine Richtung: [!DNL Dynamics] zu Marketo. Wenn Sie in [!DNL Dynamics] Änderungen an diesen Entitäten vornehmen, werden Ihre Aktualisierungen in Marketo übernommen.

## Was passiert, wenn Änderungen am selben Feld in beiden Systemen gleichzeitig vorgenommen werden? (Datenkollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Obwohl dies selten ist, wird Marketo für Personen (Leads) und [!DNL Dynamics] für Kontakte gewinnen. Der Grund dafür ist, dass wir die Marketing-Abteilung für die Menschen als verbindlich betrachten, während das offizielle System der Aufzeichnung für Kontakte in der Verkaufs- (CRM)-Abteilung ist. Bei unidirektionalen Synchronisierungsentitäten gewinnen [!DNL Dynamics] immer.

## Kann ich mit Marketo ein Feld in [!DNL Dynamics] erstellen? {#can-i-create-a-field-in-dynamics-using-marketo}

Nein, dies wird derzeit nicht unterstützt.

## Ich habe ein Feld in [!DNL Dynamics] erstellt. Kann ich sie mit Marketo synchronisieren? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Ja, Sie können [Feld synchronisieren](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) solange Ihr Synchronisierungsbenutzer in [!DNL Dynamics] Zugriff darauf hat.

## Welche Felder werden mit Marketo synchronisiert? {#what-fields-will-sync-to-marketo}

Sie können [ Setup Felder auswählen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} die synchronisiert werden sollen.

## Was passiert, wenn ich ein benutzerdefiniertes Feld hinzufügen muss, nachdem Marketo und [!DNL Dynamics] synchronisiert wurden? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Sie können jederzeit Felder hinzufügen und erwarten, dass die Daten von [!DNL Dynamics] auf Marketo aktualisiert werden. Siehe [Verwenden der Schnellsynchronisierung mit [!DNL Microsoft Dynamics]  für ein neues benutzerdefiniertes Feld](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) für Details.

## Was passiert, wenn ich ein Feld in [!DNL Dynamics] löschen möchte, nachdem das Feld zur Synchronisierung hinzugefügt wurde? {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

Marketo speichert einen Verweis auf die zu synchronisierenden Felder. Wenn Sie ein Feld in [!DNL Dynamics] löschen, wird empfohlen, dies mit [Synchronisierung deaktiviert](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md) durchzuführen. Aktualisieren Sie dann das Schema in Marketo, indem Sie die Option [Zu synchronisierende Felder auswählen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md) bearbeiten und speichern.
