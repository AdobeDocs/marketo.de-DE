---
unique-page-id: 2953461
description: SFDC Sync - Feldsynchronisierung - Marketo-Dokumente - Produktdokumentation
title: SFDC Sync - Feldsynchronisierung
exl-id: fbd66829-53cb-47fd-a530-149d12baee0e
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# SFDC Sync: Feldsynchronisierung {#sfdc-sync-field-sync}

Marketo synchronisiert Feldinformationen aus Salesforce. Hier sind die Details.

## Welche Felder werden synchronisiert? {#which-fields-are-synced}

Wir synchronisieren die meisten Standardfelder in SFDC und jedes benutzerdefinierte Feld, das der Synchronisierungsbenutzer sehen darf.

## Wie können Sie feststellen, ob ein Datensatz in Marketo ein Lead oder ein Kontakt in Salesforce ist? {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

Wir haben ein Feld in Marketo namens SFDC Type. Es hat drei mögliche Werte: Lead, Kontakt oder es ist leer. Wenn es leer ist, bedeutet dies, dass dieser Marketo-Lead nicht in SFDC vorhanden ist.

## Wie können Sie feststellen, ob ein Lead oder Kontakt im SFDC gelöscht wird? {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

In Marketo gibt es ein Feld namens SFDC isDeleted. Wenn der Wert wahr ist, wurde der Lead in SFDC gelöscht.

## Wie stelle ich sicher, dass ein neues Feld, das ich in SFDC hinzufüge, auch in Marketo hinzugefügt wird? {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>Wenn Sie ein Feld in beiden Systemen erstellen möchten, erstellen Sie es zuerst in SFDC und es wird automatisch mit Marketo synchronisiert.

Wenn Sie ein neues Feld in SFDC hinzufügen und der Synchronisierungsbenutzer über die Berechtigung zum Anzeigen verfügt, wird es automatisch zu Marketo hinzugefügt.

## Was passiert, wenn ich eine Feldbezeichnung in SFDC ändere? {#what-if-i-change-a-field-label-in-sfdc}

Eine Änderung der Feldbezeichnung in SFDC hat keine Auswirkungen auf die Feldbezeichnung in Marketo.

## Was passiert, wenn ich einen Feldtyp in SFDC ändere? {#what-if-i-change-a-field-type-in-sfdc}

Wenn Sie einen Feldtyp ändern, löscht Marketo die Daten in den Feldern, wenn sie nicht übereinstimmen (es wird jedoch zuerst eine Warnung angezeigt). Um die Daten beizubehalten, müssen Sie sie exportieren und erneut importieren, nachdem Sie den Feldtyp geändert haben.

## Was passiert, wenn ich einen API-Namen in SFDC ändere? {#what-if-i-change-an-api-name-in-sfdc}

Wenn Sie den API-Namen eines Felds in SFDC ändern, wird in Marketo ein neues Feld erstellt.

## Was passiert, wenn ich einen neuen Picklist-Wert in SFDC hinzufüge? {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

Wenn ein neuer Picklist-Wert in SFDC zu einem Feld hinzugefügt wird, sendet Ihnen Marketo eine Benachrichtigung.

## Was ist mit benutzerdefinierten SFDC-Suchfeldern? {#what-about-custom-sfdc-lookup-fields}

Suchfelder in SFDC synchronisieren die ID, aber nicht den referenzierten Namen.

## Wie sieht es mit SFDC-Formelfeldern aus? {#what-about-sfdc-formula-fields}

Formelfelder werden zwar synchronisiert, Aktualisierungen der Verweise in der Formel werden jedoch erst synchronisiert, wenn eine Aktualisierung der [System Mod Stempel](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=en_US).

## Was passiert, wenn ich ein Feld aus Salesforce lösche, das zuvor mit Marketo synchronisiert wurde? {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

Wenn Sie ein Feld in SFDC löschen, wird das Feld in Marketo nicht automatisch gelöscht, sondern die Synchronisierung wird beendet.
