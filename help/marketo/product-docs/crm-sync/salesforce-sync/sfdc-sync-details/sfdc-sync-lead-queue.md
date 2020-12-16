---
unique-page-id: 7516241
description: SFDC-Synchronisierung - Lead-Warteschlange - Marketing Docs - Produktdokumentation
title: SFDC-Synchronisierung - Interessentenwarteschlange
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---


# SFDC-Synchronisierung: Interessentenwarteschlange {#sfdc-sync-lead-queue}

Mit Marketo können Sie Personen zu [Salesforce-Interessentenwarteschlangen](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) hinzufügen, um die Interessentenverteilung zu unterstützen. Hier sind die Details.

## Wie kann man eine Person einer Warteschlange in Marketo zuweisen? {#how-to-assign-a-person-to-a-queue-in-marketo}

Sie können eine Person einer Salesforce-Interessentenwarteschlange mithilfe einer der folgenden Flussaktionen zuweisen:

* [Person mit dem SFDC synchronisieren](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [Inhaber ändern](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>Sie können Warteschlangen in Marketing weder erstellen noch ändern.

## Wie werden Informationen zum Interessenteninhaber gespeichert, wenn die Person zu einer Warteschlange gehört? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Wenn ein Interessent einer Warteschlange in Salesforce gehört, bleiben diese Felder des Vertriebseigentümers leer, bis der Interessent einem Eigentümer zugewiesen wird.

* Vorname des Verkäufers
* Nachname des Verkäufers
* Name des Verkäufers
* Telefonnummer des Verkäufers
* E-Mail-Adresse des Verkäufers

