---
unique-page-id: 7515131
description: SFDC-Synchronisierung - Löschen eines Interessenten/Kontakts - Marketing Docs - Produktdokumentation
title: SFDC-Synchronisierung - Löschen eines Interessenten/Kontakts
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---


# SFDC-Synchronisierung: Löschen eines Interessenten/Kontakts {#sfdc-sync-deleting-a-lead-contact}

Im Folgenden finden Sie einige Details:

* Marketo löscht nicht automatisch Personen, nur weil Leads in Salesforce gelöscht wurden. Stattdessen ist das Flag &quot;SFDC ist gelöscht&quot;auf &quot;true&quot;gesetzt. Sie können dieses Feld auslösen, um es bei Bedarf in Marketo zu löschen.
* [Aktion ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) &quot;Personflow löschen&quot; Dadurch wird eine Person in MKTO gelöscht, Sie haben aber auch die Möglichkeit, sie in `Salesforce` zu löschen.

* [Aus ](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) SFDCflow-Aktion löschen: Dadurch wird ein Lead im SFDC gelöscht, aber Sie haben auch die Wahl, eine Person in Marketo zu löschen.
* Wenn ein Interessent in Salesforce gelöscht wird (aber eine Person nicht in Marketo gelöscht wird) und anschließend die [Synchronisierung mit Salesforce](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)-Fließaktion durchläuft, würde es einen neuen Lead in Salesforce erstellen.

Mit anderen Worten, es funktioniert wie Zauberei!

![—](assets/image2015-5-20-15-3a3-3a27.png)

