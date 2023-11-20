---
unique-page-id: 7516241
description: SFDC Sync - Lead Queue - Marketo Docs - Produktdokumentation
title: SFDC Sync - Lead Queue
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 15%

---

# SFDC Sync: Lead Queue {#sfdc-sync-lead-queue}

Mit Marketo Engage können Sie Personen zu [Salesforce-Lead-Warteschlangen](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm){target="_blank"} , um bei der Lead-Verteilung zu helfen. Hier sind die Details.

## Wie wird eine Person in Marketo einer Warteschlange zugewiesen? {#how-to-assign-a-person-to-a-queue-in-marketo}

Sie können eine Person einer Salesforce-Lead-Warteschlange zuweisen, indem Sie eine der folgenden Durchsatzaktionen verwenden:

* [Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}
* [Eigentümer ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}

>[!NOTE]
>
>Sie können keine Warteschlangen in Marketo erstellen oder ändern.

## Wie werden Informationen zum Lead-Eigentümer gespeichert, wenn die Person zu einer Warteschlange gehört? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Wenn ein Lead einer Warteschlange in Salesforce gehört, werden diese Felder des Verkaufsinhabers leer gelassen, bis der Lead einem Eigentümer zugewiesen wird.

* Vorname des Verkaufsinhabers
* Nachname des Verkaufsinhabers
* Name des Vertriebsmitarbeiters
* Telefonnummer des Verkaufsinhabers
* E-Mail-Adresse des Verkaufsinhabers
