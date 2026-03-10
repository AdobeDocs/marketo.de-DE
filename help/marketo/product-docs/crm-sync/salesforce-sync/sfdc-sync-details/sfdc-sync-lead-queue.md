---
unique-page-id: 7516241
description: Erfahren Sie mehr über das Zuweisen von Personen zu Salesforce-Lead-Warteschlangen aus Marketo. Verwenden Sie die Flussaktionen „Person mit SFDC synchronisieren“ oder „Besitzer ändern“ für die Lead-Verteilung.
title: SFDC-Synchronisierung - Lead-Warteschlange
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 13%

---

# SFDC-Synchronisation: Lead-Warteschlange {#sfdc-sync-lead-queue}

Mit Marketo können Sie Personen zu [[!DNL Salesforce] Lead-Warteschlangen](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) hinzufügen, um die Lead-Verteilung zu erleichtern. Im Folgenden finden Sie die Details.

## Zuweisen einer Person zu einer Warteschlange in Marketo {#how-to-assign-a-person-to-a-queue-in-marketo}

Sie können eine Person mithilfe einer der folgenden Flussaktionen einer [!DNL Salesforce] Lead-Warteschlange zuweisen:

* [Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}
* [Besitzer ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}

>[!NOTE]
>
>In Marketo können keine Warteschlangen erstellt oder geändert werden.

## Wie werden Informationen zum Lead-Eigentümer gespeichert, wenn die Person zu einer Warteschlange gehört? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Wenn ein Lead einer Warteschlange in [!DNL Salesforce] gehört, bleiben diese Felder für den Verkaufsverantwortlichen leer, bis der Lead einem Besitzer zugewiesen wird.

* Vorname des Verkaufseigentümers
* Nachname des Verkaufseigentümers
* Titel des Vertriebsinhabers
* Telefonnummer des Verkaufseigentümers
* E-Mail-Adresse des Verkaufseigentümers
