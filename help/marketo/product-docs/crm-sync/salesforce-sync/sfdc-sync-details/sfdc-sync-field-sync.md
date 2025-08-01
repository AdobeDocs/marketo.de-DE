---
unique-page-id: 2953461
description: SFDC-Synchronisierung - Feldsynchronisierung - Marketo-Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Feldsynchronisierung
exl-id: fbd66829-53cb-47fd-a530-149d12baee0e
feature: Salesforce Integration
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# SFDC-Synchronisierung: Feldsynchronisierung {#sfdc-sync-field-sync}

Marketo synchronisiert Feldinformationen aus [!DNL Salesforce]. Im Folgenden finden Sie die Details.

## Welche Felder werden synchronisiert? {#which-fields-are-synced}

Wir synchronisieren die meisten Standardfelder in SFDC und alle benutzerdefinierten Felder, für die der Synchronisierungsbenutzer über die Berechtigung zum Anzeigen verfügt.

## Wie kann man feststellen, ob ein Datensatz in Marketo ein Lead oder ein Kontakt in [!DNL Salesforce] ist? {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

Wir haben in Marketo ein Feld namens SFDC Type. Es gibt drei mögliche Werte: Lead, Kontakt oder es ist leer. Wenn er leer ist, bedeutet dies, dass dieser Marketo-Lead nicht in SFDC vorhanden ist.

## Wie kann festgestellt werden, ob ein Lead oder Kontakt in SFDC gelöscht wird? {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

Wir haben ein Feld in Marketo namens SFDC isDeleted. Wenn der Wert „true“ ist, wurde der Lead in SFDC gelöscht.

## Wie stelle ich sicher, dass ein neues Feld, das ich in SFDC hinzufüge, auch zu Marketo hinzugefügt wird? {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>Wenn Sie ein Feld in beiden Systemen möchten, erstellen Sie es zuerst in SFDC und es wird automatisch mit Marketo synchronisiert.

Wenn Sie ein neues Feld in SFDC hinzufügen und der Synchronisierungsbenutzer berechtigt ist, es anzuzeigen, wird es automatisch zu Marketo hinzugefügt.

## Was passiert, wenn ich eine Feldbezeichnung in SFDC ändere? {#what-if-i-change-a-field-label-in-sfdc}

Das Ändern der Feldbezeichnung in SFDC wirkt sich nicht auf die Feldbezeichnung in Marketo aus.

## Was passiert, wenn ich einen Feldtyp in SFDC ändere? {#what-if-i-change-a-field-type-in-sfdc}

Wenn Sie einen Feldtyp ändern, löscht Marketo die Daten in den Feldern, wenn sie nicht übereinstimmen (zeigt jedoch zuerst eine Warnung an). Um die Daten beizubehalten, exportieren Sie sie unbedingt und importieren Sie sie erneut, nachdem Sie den Feldtyp geändert haben.

## Was passiert, wenn ich einen API-Namen in SFDC ändere? {#what-if-i-change-an-api-name-in-sfdc}

Wenn Sie den API-Namen eines Felds in SFDC ändern, wird in Marketo ein neues Feld erstellt.

## Was passiert, wenn ich in SFDC einen neuen Wert für die Auswahlliste hinzufüge? {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

Wenn einem Feld in SFDC ein neuer Auswahllistenwert hinzugefügt wird, sendet Marketo eine Benachrichtigung.

## Was ist mit benutzerdefinierten SFDC-Suchfeldern? {#what-about-custom-sfdc-lookup-fields}

Suchfelder in SFDC synchronisieren die ID, aber nicht den referenzierten Namen.

## Was ist mit SFDC-Formelfeldern? {#what-about-sfdc-formula-fields}

Formelfelder werden synchronisiert. Aktualisierungen an den Verweisen in der Formel werden jedoch erst synchronisiert, wenn eine Aktualisierung für einen [Systemmodusstempel“ ](https://help.salesforce.com/apex/HTViewSolution?id=000193203&language=en_US){target="_blank"}.

## Was passiert, wenn ich ein Feld aus [!DNL Salesforce] lösche, das zuvor mit Marketo synchronisiert wurde? {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

Wenn Sie ein Feld in SFDC löschen, wird es nicht automatisch in Marketo gelöscht, sondern die Synchronisierung wird beendet.
