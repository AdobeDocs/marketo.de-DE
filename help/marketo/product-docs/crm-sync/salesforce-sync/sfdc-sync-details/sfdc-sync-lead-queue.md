---
unique-page-id: 7516241
description: SFDC-Synchronisierung - Lead-Warteschlange - Marketing Docs - Produktdokumentation
title: SFDC-Synchronisierung - Interessentenwarteschlange
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# SFDC-Synchronisierung: Interessentenwarteschlange {#sfdc-sync-lead-queue}

Mit Marketo können Sie Personen zu [Salesforce-Interessentenwarteschlangen](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) hinzufügen, um die Interessentenverteilung zu unterstützen. Hier sind die Details.

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

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

