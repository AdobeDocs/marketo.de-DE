---
unique-page-id: 2953469
description: SFDC Sync - Kampagnensynchronisierung - Marketo-Dokumente - Produktdokumentation
title: SFDC Sync - Kampagnensynchronisierung
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 5%

---

# SFDC-Synchronisation: Kampagnensynchronisierung {#sfdc-sync-campaign-sync}

Marketo-Programme können mit Salesforce-Kampagnen synchronisiert werden. Hier finden Sie einen Überblick darüber, wie dies funktioniert.

## Warum sollte ich Marketo-Programme mit Salesforce-Kampagnen synchronisieren? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Verwenden Sie die leistungsstarken Funktionen eines Marketo-Programms.
* Die Mitglieder und ihr Status bleiben zwischen einem Marketo-Programm und einer Salesforce-Kampagne synchron.
* Tippen Sie auf die Berichterstellungsfunktionen in Marketo und Salesforce.

## Wie werden ein Marketo-Programm und eine Salesforce-Kampagne synchronisiert? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

In Marketo haben Sie die Möglichkeit, ein Eins-zu-Eins-Mapping zwischen einem Programm und einer Salesforce-Kampagne zu erstellen.

![](assets/image2015-7-8-9-3a43-3a8.png)

Die **[channel](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)** und **[Zeitraumkosten](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** Synchronisieren Sie in Marketo mit Salesforce als **Kampagnentyp** und **tatsächliche Kosten**. Diese Synchronisierung **Einweg**, von Marketo nach Salesforce.

Marketo **Programmmitglieder** und **[Progressionsstatus](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** werden mit dem **Salesforce-Kampagnenmitglieder** und **Status der Kampagnenmitglieder**. Dies ist ein **bidirektionale Synchronisation**, sodass alle Änderungen, die in Marketo oder Salesforce vorgenommen werden, in beiden Systemen übernommen werden.

>[!NOTE]
>
>Wenn es Mitglieder im Marketo-Programm gibt, die nicht in Salesforce vorhanden sind, erstellt Marketo diese Personen als Leads in Salesforce.

## Welche Trigger/Filter beziehen sich auf Kampagnen? {#what-are-the-triggers-filters-related-to-campaigns}

Auslöser:

* Zu SFDC-Kampagne hinzugefügt
* Aus SFDC-Kampagne entfernt
* Status wird in SFDC-Kampagne geändert

Filter:

* Mitglied einer SFDC-Kampagne

## Kann ich meiner SFDC-Kampagne Marketo People hinzufügen? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Ja, verwenden Sie die [Zu SFDC-Kampagnenflussaktion hinzufügen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md). Wenn diese Person nicht in Salesforce vorhanden ist, erstellt Marketo sie in Salesforce und fügt sie dann der Kampagne hinzu.

## Kann ich mit Marketo Mitglieder aus meiner SFDC-Kampagne entfernen? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Ja, verwenden Sie die [Aus der SFDC-Campaign-Flussaktion entfernen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md).

## Kann ich den Status von Kampagnenmitgliedern mit Marketo ändern? {#can-i-change-campaign-member-status-using-marketo}

Ja, verwenden Sie die [Status in der Flow-Aktion für SFDC-Kampagnen ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md).

## Warum kann ich keine meiner Salesforce-Kampagnen sehen? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Sie können Folgendes überprüfen:

1. Stellen Sie sicher, dass [Kampagnensynchronisation ist aktiviert](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. Vergewissern Sie sich, dass [Marketo Sync User](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) ist [Marketing-Benutzer](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) in Salesforce.

>[!NOTE]
>
>Wenn Ihre Salesforce-Kampagne und das zugeordnete Marketo-Programm inkompatible Programmstatus aufweisen, erhalten Sie möglicherweise eine Fehlermeldung. Wir empfehlen Ihnen, [Übereinstimmung mit dem Programmstatus vor der Synchronisierung](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

>[!MORELIKETHIS]
>
>* [Synchronisieren einer SFDC-Kampagne mit einem Programm](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [Grundlegendes zur Programmmitgliedschaft](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [Aktivieren/Deaktivieren der Kampagnensynchronisierung](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [Einrichten eines Marketo Sync-Benutzers als Marketing-Benutzer](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)
