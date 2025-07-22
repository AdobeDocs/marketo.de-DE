---
unique-page-id: 2953469
description: SFDC-Synchronisierung - Kampagnensynchronisierung - Marketo-Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Kampagnensynchronisierung
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 5%

---

# SFDC-Synchronisation: Kampagnensynchronisation {#sfdc-sync-campaign-sync}

Marketo-Programme können mit [!DNL Salesforce]-Kampagnen synchronisiert werden. Im Folgenden finden Sie einen Überblick darüber, wie dies funktioniert.

## Warum sollte ich Marketo-Programme mit [!DNL Salesforce] Kampagnen synchronisieren? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Nutzen Sie die leistungsstarken Funktionen eines Marketo-Programms.
* Halten Sie Mitglieder und ihren Status zwischen einem Marketo-Programm und einer [!DNL Salesforce] Campaign synchron.
* Nutzen Sie die Reporting-Funktionen in Marketo und [!DNL Salesforce].

## Wie werden ein Marketo-Programm und eine [!DNL Salesforce]-Kampagne synchronisiert? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

In Marketo haben Sie die Möglichkeit, eine Eins-zu-eins-Zuordnung zwischen einem Programm und einer [!DNL Salesforce] Kampagne zu erstellen.

![](assets/image2015-7-8-9-3a43-3a8.png)

Die **[Kanal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)** und **[Periodenkosten](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** in Marketo synchronisieren sich mit [!DNL Salesforce] als **Kampagnentyp** und **Istkosten**. Diese Synchronisierung erfolgt **unidirektional** von Marketo nach [!DNL Salesforce].

Marketo **Programmmitglieder** und ihre **[Fortschrittsstatus](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** werden mit den **[!DNL Salesforce]** Kampagnenmitgliedern und **Kampagnenmitgliederstatus**. Dies ist eine **bidirektionale Synchronisierung** sodass alle Änderungen, die an Marketo oder [!DNL Salesforce] vorgenommen wurden, auf beiden Systemen widergespiegelt werden.

>[!NOTE]
>
>Wenn im Marketo-Programm Mitglieder vorhanden sind, die nicht in [!DNL Salesforce] vorhanden sind, erstellt Marketo diese Personen als Leads in [!DNL Salesforce].

## Welche Trigger/Filter beziehen sich auf Kampagnen? {#what-are-the-triggers-filters-related-to-campaigns}

Auslöser:

* Zu SFDC-Kampagne hinzugefügt
* Aus SFDC-Kampagne entfernt
* Status wird in SFDC-Kampagne geändert

Filter:

* Mitglied der SFDC-Kampagne

## Kann ich Marketo People zu meiner SFDC-Kampagne hinzufügen? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Ja, die [Kampagnenflussaktion Zu SFDC hinzufügen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md) verwenden. Wenn diese Person nicht in [!DNL Salesforce] vorhanden ist, erstellt Marketo sie in [!DNL Salesforce] und fügt sie dann der Kampagne hinzu.

## Kann ich Mitglieder mithilfe von Marketo aus meiner SFDC-Kampagne entfernen? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Ja, die Flussaktion [Aus SFDC Campaign entfernen“ ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md){target="_blank"}.

## Kann ich den Status des Kampagnenmitglieds mit Marketo ändern? {#can-i-change-campaign-member-status-using-marketo}

Ja, verwenden Sie die [Statusänderung in SFDC Campaign-Flussaktion](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}.

## Warum sehe ich keine meiner [!DNL Salesforce] Kampagnen? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Hier sind die Dinge, die Sie überprüfen können:

1. Stellen Sie sicher[ dass die Kampagnensynchronisierung aktiviert ](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. Vergewissern Sie sich, dass Ihr [Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)Synchronisierungsbenutzer[ ein „Marketing-](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)&quot; in [!DNL Salesforce] ist.

>[!NOTE]
>
>Wenn Ihre [!DNL Salesforce]-Kampagne und das zugeordnete Marketo-Programm inkompatible Programmstatus haben, erhalten Sie möglicherweise eine Fehlermeldung. Es wird empfohlen[ die Programmstatus vor der Synchronisierung abzugleichen](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

>[!MORELIKETHIS]
>
>* [Synchronisieren einer SFDC-Kampagne mit einem Programm](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}
>* [Grundlegendes zur Programmmitgliedschaft](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}
>* [Kampagnensynchronisierung aktivieren/deaktivieren](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}
>* [Marketo-Synchronisierungsbenutzer als Marketing-Benutzer festlegen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}
