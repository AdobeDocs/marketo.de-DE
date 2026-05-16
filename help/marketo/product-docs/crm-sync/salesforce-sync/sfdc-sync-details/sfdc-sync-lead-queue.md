---
unique-page-id: 7516241
description: Erfahren Sie mehr über das Zuweisen von Personen zu Salesforce-Lead-Warteschlangen aus Marketo. Verwenden Sie die Flussaktionen „Person mit SFDC synchronisieren“ oder „Besitzer ändern“ für die Lead-Verteilung.
title: SFDC-Synchronisierung - Lead-Warteschlange
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/aUrT7qSMy65t3K07O176nt-Bzjm9urgnXKAkZgs1-cs
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 150
ht-degree: 17%

---

# SFDC-Synchronisation: Lead-Warteschlange {#sfdc-sync-lead-queue}

Mit Marketo können Sie Personen zu [[!DNL Salesforce] Lead-Warteschlangen](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) hinzufügen, um die Lead-Verteilung zu erleichtern. Im Folgenden finden Sie die Details.

## Zuweisen einer Person zu einer Warteschlange in Marketo {#how-to-assign-a-person-to-a-queue-in-marketo}

Sie können eine Person mithilfe einer der folgenden Flussaktionen einer [!DNL Salesforce] Lead-Warteschlange zuweisen:

* [Synchronisieren von Personen mit SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}
* [Ändern von Eigentümerin bzw. Eigentümer](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}

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
