---
unique-page-id: 2953469
description: SFDC-Synchronisierung - Synchronisierung von Kampagnen - Marketo Docs - Produktdokumentation
title: SFDC-Synchronisierung - Kampagne synchronisieren
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 5%

---

# SFDC-Synchronisierung: Kampagne Sync {#sfdc-sync-campaign-sync}

Marketo-Programm können mit Salesforce-Kampagnen synchronisiert werden. Hier finden Sie einen Überblick darüber, wie das funktioniert.

## Warum sollte ich Marketo-Programme mit Salesforce-Kampagnen synchronisieren? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Nutzen Sie die leistungsstarken Funktionen eines Marketo-Programms.
* Synchronisieren Sie Mitglieder und deren Status zwischen einem Marketo-Programm und einer Salesforce-Kampagne.
* Tippen Sie auf die Berichte-Funktionen in Marketo und Salesforce.

## Wie werden ein Marketo-Programm und eine Salesforce-Kampagne synchronisiert? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

In Marketo haben Sie die Möglichkeit, eine Eins-zu-Eins-Zuordnung zwischen einem Programm und einer Salesforce-Kampagne zu erstellen.

![](assets/image2015-7-8-9-3a43-3a8.png)

Die Kosten für **[Kanal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)** und **[Punkt](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** in Marketo werden mit Salesforce als **Kampagne Typ** und **tatsächliche Kosten** synchronisiert. Diese Synchronisierung erfolgt von Marketo nach Salesforce auf eine Weise.****

Marketo **Programm-Mitglieder** und ihre **[Progressionsstatus](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** werden mit den **Salesforce-Kampagne-Mitgliedern** und **Kampagne-Mitgliedsstatus** synchronisiert. Hierbei handelt es sich um eine **bidirektionale Synchronisierung**, sodass alle in Marketo oder Salesforce vorgenommenen Änderungen auf beiden Systemen übernommen werden.

>[!NOTE]
>
>Wenn es Mitglieder im Marketo-Programm gibt, die nicht in Salesforce existieren, dann schafft Marketo diese Menschen als Interessenten in Salesforce.

## Welche Trigger/Filter sind mit Kampagnen verbunden? {#what-are-the-triggers-filters-related-to-campaigns}

Auslöser:

* Zu SFDC-Kampagne hinzugefügt
* Aus SFDC-Kampagne entfernt
* Status wird in SFDC-Kampagne geändert

Filter:

* Mitglied der SFDC-Kampagne

## Kann ich Marketo People zu meiner SFDC-Kampagne hinzufügen? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Ja, verwenden Sie die Hinzufügen [zu SFDC Kampagne Flow Aktion](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md). Wenn diese Person nicht in Salesforce vorhanden ist, erstellt Marketo sie in Salesforce und fügt sie dann der Kampagne hinzu.

## Kann ich mit Marketo Mitglieder aus meiner SFDC-Kampagne entfernen? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Ja, verwenden Sie die Fließaktion [Aus SFDC-Kampagne entfernen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md).

## Kann ich den Mitgliedsstatus der Kampagne mit Marketo ändern? {#can-i-change-campaign-member-status-using-marketo}

Ja, verwenden Sie die Aktion [Status in SFDC-Kampagne ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md).

## Warum kann ich keine meiner Salesforce-Kampagnen sehen? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Sie können folgende Punkte prüfen:

1. Vergewissern Sie sich, dass [Kampagne-Synchronisierung aktiviert ist](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. Vergewissern Sie sich, dass der [Marketo Sync User](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) ein [Marketing-Benutzer](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) in Salesforce ist.

>[!NOTE]
>
>Wenn Ihre Salesforce-Kampagne und das zugeordnete Marketo-Programm inkompatible Programm-Status haben, erhalten Sie möglicherweise eine Fehlermeldung. Es wird empfohlen, [vor der Synchronisierung mit dem Programm-Status abzugleichen.](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)

>[!MORELIKETHIS]
>
>* [Synchronisieren einer SFDC-Kampagne mit einem Programm](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [Informationen zur Programm-Mitgliedschaft](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [Synchronisierung der Kampagne aktivieren/deaktivieren](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [Marketo Sync-Benutzer zu einem Marketing-Benutzer machen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)

