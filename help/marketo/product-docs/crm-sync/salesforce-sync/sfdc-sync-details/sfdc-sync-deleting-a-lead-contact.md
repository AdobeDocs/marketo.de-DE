---
unique-page-id: 7515131
description: SFDC Sync - Löschen eines Leads/Kontakts - Marketo Docs - Produktdokumentation
title: SFDC Sync - Löschen eines Leads/Kontakts
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# SFDC-Synchronisation: Löschen eines Leads/Kontakts {#sfdc-sync-deleting-a-lead-contact}

Im Folgenden finden Sie einige Details:

* Marketo Engage löscht Personen nicht automatisch, nur weil Leads in Salesforce gelöscht wurden. Stattdessen wird die Markierung &quot;SFDC ist gelöscht&quot;auf &quot;true&quot;gesetzt. Sie können dieses Feld bei Bedarf löschen und in Marketo löschen.
* [Person löschen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md){target="_blank"} Flussaktion. Dadurch wird eine Person in MKTO gelöscht, Sie können jedoch löschen in `Salesforce` auch.

* [Aus SFDC löschen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md){target="_blank"} Flow-Aktion: Löscht einen Lead in SFDC, Sie können jedoch auch eine Person in Marketo löschen.
* Wenn ein Lead in Salesforce gelöscht wird (aber eine Person nicht in Marketo gelöscht wird), durchläuft er anschließend die [Mit Salesforce synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} Fluss-Aktion, dann würde es einen neuen Lead in Salesforce erstellen.
