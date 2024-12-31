---
unique-page-id: 2953473
description: SFDC-Synchronisierung - Aktivitätssynchronisierung - Marketo-Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Aktivitätssynchronisierung
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 4%

---

# SFDC-Synchronisierung: Aktivitätssynchronisierung {#sfdc-sync-activity-sync}

Marketo Engage synchronisiert auch die Daten der Salesforce-Aktivitäten. Im Folgenden finden Sie einige Fragen und Antworten.

## Welche Aktivitätstypen werden von Marketo synchronisiert? {#what-types-of-activity-data-does-marketo-sync-over}

Marketo synchronisiert sowohl Ereignisse als auch Aufgaben, die mit einem Lead oder Kontakt verknüpft sind.

## Wie werden Aktivitätsdetails zwischen den beiden Systemen synchron gehalten? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

Die Synchronisierung erfolgt in eine Richtung, von Salesforce zu Marketo. Sie können eine Aufgabe jedoch in Salesforce mit dem Flussschritt [Aufgabe erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} oder [Aktivitätssynchronisierung anpassen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md){target="_blank"} mit Salesforce erstellen.

## Kann ich eine Aufgabe mit Marketo erstellen? {#can-i-create-a-task-using-marketo}

Ja, Sie können die Aktion [Aufgabenfluss erstellen“ ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}.

## Welche Trigger/Filter beziehen sich auf eine Aktivität? {#what-are-the-triggers-filters-related-to-activity}

Trigger

* Aktivität wird protokolliert
* Aktivität wird aktualisiert

Filter

* Aktivität wurde protokolliert/Aktivität wurde nicht protokolliert
* Aktivität wurde aktualisiert/Aktivität wurde nicht aktualisiert

>[!TIP]
>
>Sie sind sich nicht sicher, was die Formulierung „Keine Aktivität“ angeht? Das „not“ bezieht sich auf einen Inaktivitätsfilter. Weitere Informationen dazu finden Sie hier: [Verwenden von Inaktivitätsfiltern in einer Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md){target="_blank"}
