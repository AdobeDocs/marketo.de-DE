---
unique-page-id: 7516241
description: SFDC-Synchronisierung - Lead-Warteschlange - Marketo Docs - Produktdokumentation
title: SFDC-Synchronisierung - Interessentenwarteschlange
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 15%

---

# SFDC-Synchronisierung: Interessentenwarteschlange {#sfdc-sync-lead-queue}

Mit Marketo können Sie Personen zu [Salesforce-Interessentenwarteschlangen](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) hinzufügen, um die Interessentenverteilung zu unterstützen. Hier sind die Details.

## Wie kann man eine Person einer Warteschlange in Marketo zuweisen? {#how-to-assign-a-person-to-a-queue-in-marketo}

Sie können eine Person einer Salesforce-Interessentenwarteschlange mithilfe einer der folgenden Flussaktionen zuweisen:

* [Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [Eigentümer ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>Sie können Warteschlangen in Marketo weder erstellen noch ändern.

## Wie werden Informationen zum Interessenteninhaber gespeichert, wenn die Person zu einer Warteschlange gehört? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Wenn ein Interessent einer Warteschlange in Salesforce gehört, bleiben diese Felder des Vertriebseigentümers leer, bis der Interessent einem Eigentümer zugewiesen wird.

* Vorname des Vertriebseigentümers
* Nachname des Vertriebseigentümers
* Name des Verkäufers
* Telefonnummer des Vertriebseigentümers
* E-Mail-Adresse des Vertriebseigentümers
