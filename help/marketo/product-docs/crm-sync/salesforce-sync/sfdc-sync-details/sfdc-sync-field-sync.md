---
unique-page-id: 2953461
description: SFDC-Synchronisierung - Feldsynchronisierung - Marketing-Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Feldsynchronisierung
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---


# SFDC-Synchronisierung: Feldsynchronisierung {#sfdc-sync-field-sync}

Marketo synchronisiert Feldinformationen aus Salesforce. Hier sind die Details.

## Welche Felder werden synchronisiert? {#which-fields-are-synced}

Wir synchronisieren die meisten Standardfelder im SFDC und alle benutzerdefinierten Felder, die der Synchronisierungsbenutzer sehen darf.

## Wie bestimmen Sie, ob ein Datensatz in Marketo ein Lead oder ein Kontakt in Salesforce ist? {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

Wir haben ein Feld in Marketo namens SFDC Type. Es verfügt über drei mögliche Werte: Lead, Kontakt oder leer. Wenn es leer ist, bedeutet das, dass dieser Marketo-Lead nicht im SFDC vorhanden ist.

## Wie stellen Sie fest, ob ein Interessent oder Kontakt im SFDC gelöscht wird? {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

Wir haben ein Feld in Marketo namens SFDC isDeleted. Wenn der Wert true ist, wurde der Interessent im SFDC gelöscht.

## Wie stelle ich sicher, dass ein neues Feld, das ich in SFDC hinzufüge, auch in Marketo hinzugefügt wird? {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>Wenn Sie ein Feld in beiden Systemen wünschen, erstellen Sie es zuerst im SFDC und es wird automatisch nach Marketo synchronisiert.

Wenn Sie ein neues Feld in SFDC hinzufügen und der Synchronisierungsbenutzer berechtigt ist, es anzuzeigen, wird es automatisch zu Marketo hinzugefügt.

## Was ist, wenn ich eine Feldbeschriftung im SFDC ändere? {#what-if-i-change-a-field-label-in-sfdc}

Eine Änderung der Feldbeschriftung im SFDC hat keine Auswirkungen auf die Feldbeschriftung in Marketo.

## Was ist, wenn ich einen Feldtyp im SFDC ändere? {#what-if-i-change-a-field-type-in-sfdc}

Wenn Sie einen Feldtyp ändern, werden die Daten in den Feldern gelöscht, wenn sie nicht übereinstimmen (zunächst wird jedoch eine Warnung angezeigt). Um die Daten zu erhalten, müssen Sie sie exportieren und erneut importieren, nachdem Sie den Feldtyp geändert haben.

## Was ist, wenn ich einen API-Namen in SFDC ändere? {#what-if-i-change-an-api-name-in-sfdc}

Wenn Sie den API-Namen eines Felds in SFDC ändern, wird ein neues Feld in Marketo erstellt.

## Was passiert, wenn ich einen neuen Picklist-Wert in das SFDC einfüge? {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

Wenn ein neuer picklist-Wert in SFDC zu einem Feld hinzugefügt wird, sendet Ihnen Marketo eine Benachrichtigung.

## Wie sieht es mit benutzerdefinierten SFDC-Suchfeldern aus? {#what-about-custom-sfdc-lookup-fields}

Suchfelder in SFDC synchronisieren die ID, nicht jedoch den referenzierten Namen.

## Wie sieht es mit den SFDC-Formularfeldern aus? {#what-about-sfdc-formula-fields}

Formularfelder werden synchronisiert, allerdings werden Aktualisierungen der Verweise in der Formel erst synchronisiert, wenn ein [System Mod Stamp](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=en_US)aktualisiert wurde.

## Was passiert, wenn ich ein Feld aus Salesforce lösche, das zuvor mit Marketo synchronisiert wurde? {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

Wenn Sie ein Feld in SFDC löschen, wird das Feld in Marketo nicht automatisch gelöscht, es stoppt die Synchronisierung.
