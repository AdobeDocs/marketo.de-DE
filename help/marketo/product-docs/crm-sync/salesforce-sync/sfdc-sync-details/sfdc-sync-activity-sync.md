---
unique-page-id: 2953473
description: SFDC Sync - Activity Sync - Marketo-Dokumente - Produktdokumentation
title: SFDC Sync - Aktivitäts-Sync
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 4%

---

# SFDC-Synchronisierung: Aktivitätensynchronisierung {#sfdc-sync-activity-sync}

Marketo synchronisiert auch die Salesforce-Aktivitätsdaten. Hier sind einige Fragen und Antworten.

## Über welche Aktivitätsdaten synchronisiert Marketo? {#what-types-of-activity-data-does-marketo-sync-over}

Marketo synchronisiert Ereignisse und Aufgaben, die mit einem Lead oder Kontakt verknüpft sind.

## Wie werden Aktivitätsdetails zwischen den beiden Systemen synchronisiert? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

Die Synchronisation ist eine Möglichkeit, von Salesforce bis Marketo. Sie können eine Aufgabe in Salesforce jedoch mit der [Aufgabe erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) Flussschritt oder [Aktivitätensynchronisierung anpassen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) nach Salesforce.

## Kann ich eine Aufgabe mit Marketo erstellen? {#can-i-create-a-task-using-marketo}

Ja, Sie können die [Aktion zum Erstellen eines Aufgabenflusses](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md).

## Welche Trigger/Filter beziehen sich auf die Aktivität? {#what-are-the-triggers-filters-related-to-activity}

Trigger

* Aktivität wird protokolliert
* Aktivität wird aktualisiert

Filter

* Aktivität wurde protokolliert/Aktivität wurde nicht protokolliert
* Aktivität wurde aktualisiert/Aktivität wurde nicht aktualisiert

>[!TIP]
>
>Sie sind sich nicht sicher, was die Formulierung &quot;Not Activity&quot;betrifft? &quot;nicht&quot;bezieht sich auf einen Inaktivitätsfilter. Weitere Informationen dazu finden Sie hier: [Verwenden von Inaktivitätsfiltern in einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)
