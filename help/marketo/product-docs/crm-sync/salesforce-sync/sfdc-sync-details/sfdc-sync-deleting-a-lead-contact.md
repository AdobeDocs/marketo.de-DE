---
unique-page-id: 7515131
description: SFDC-Synchronisierung - Löschen eines Interessenten/Kontakts - Marketing Docs - Produktdokumentation
title: SFDC-Synchronisierung - Löschen eines Interessenten/Kontakts
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---


# SFDC-Synchronisierung: Löschen eines Interessenten/Kontakts {#sfdc-sync-deleting-a-lead-contact}

Im Folgenden finden Sie einige Details:

* Marketo löscht nicht automatisch Personen, nur weil Leads in Salesforce gelöscht wurden. Stattdessen ist das Flag &quot;SFDC ist gelöscht&quot;auf &quot;true&quot;gesetzt. Sie können dieses Feld bei Bedarf in Marketo löschen, um es zu löschen.
* [Aktion ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) &quot;Personflow löschen&quot; Dadurch wird eine Person in MKTO gelöscht, Sie haben aber auch die Möglichkeit, sie in `Salesforce` zu löschen.

* [Aus ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) SFDCflow-Aktion löschen: Dadurch wird ein Lead im SFDC gelöscht, aber Sie haben auch die Wahl, eine Person in Marketo zu löschen.
* Wenn ein Interessent in Salesforce gelöscht wird (aber eine Person nicht in Marketo gelöscht wird) und anschließend die [Synchronisierung mit Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)-Fließaktion durchläuft, würde es einen neuen Lead in Salesforce erstellen.
