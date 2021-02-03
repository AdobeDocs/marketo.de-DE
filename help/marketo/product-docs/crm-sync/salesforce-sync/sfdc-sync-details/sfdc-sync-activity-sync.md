---
unique-page-id: 2953473
description: SFDC-Synchronisierung - Synchronisierung von Aktivitäten - Marketing Docs - Produktdokumentation
title: SFDC-Synchronisierung - Aktivität synchronisieren
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# SFDC-Synchronisierung: Aktivität Sync {#sfdc-sync-activity-sync}

Marketo synchronisiert auch die Salesforce-Aktivitäten-Daten. Hier sind einige Fragen und Antworten.

## Über welche Aktivitäten synchronisiert Marketo? {#what-types-of-activity-data-does-marketo-sync-over}

Marketo synchronisiert sowohl Ereignisse als auch Aufgaben, die mit einem Interessenten oder Kontakt verbunden sind.

## Wie werden die Aktivitäten zwischen den beiden Systemen synchronisiert? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

Die Synchronisierung ist eine Möglichkeit, von Salesforce bis Marketo. Sie können jedoch eine Aufgabe in Salesforce mit dem Flussschritt [Aufgabe erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) oder [Aktivitäten anpassen Synchronisieren](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) zu Salesforce erstellen.

## Kann ich mit Marketo eine Aufgabe erstellen? {#can-i-create-a-task-using-marketo}

Ja, Sie können die Flussaktion [Aufgabe erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) verwenden.

## Welche Trigger/Filter sind mit der Aktivität verbunden? {#what-are-the-triggers-filters-related-to-activity}

Trigger

* Aktivität wird protokolliert
* Aktivität wurde aktualisiert

Filter

* Aktivität wurde protokolliert/Nicht Aktivität wurde protokolliert
* Aktivität wurde aktualisiert/Aktivität wurde nicht aktualisiert

>[!TIP]
>
>Nicht sicher, ob es sich um die Formulierung &quot;Nicht Aktivität&quot; handelt? &quot;nicht&quot;bezieht sich auf einen Inaktivitätsfilter. Weitere Informationen finden Sie hier: [Inaktive Filter in einer intelligenten Liste verwenden](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)
