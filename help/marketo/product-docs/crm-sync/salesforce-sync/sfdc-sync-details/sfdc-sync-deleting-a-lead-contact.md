---
unique-page-id: 7515131
description: SFDC-Synchronisierung - Löschen eines Leads/Kontakts - Marketo-Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Löschen eines Leads/Kontakts
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---

# SFDC-Synchronisierung: Lead/Kontakt löschen {#sfdc-sync-deleting-a-lead-contact}

Im Folgenden finden Sie einige Details:

* Marketo löscht Personen nicht automatisch, nur weil Leads in [!DNL Salesforce] gelöscht wurden. Stattdessen wird das Feld-Flag &quot;SFDC wird gelöscht“ auf „true“ gesetzt. Sie können bei Bedarf Trigger aus diesem Feld in Marketo löschen.
* [Person löschen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) Flussaktion. Dadurch wird eine Person in MKTO gelöscht, aber Sie haben auch in `Salesforce` die Möglichkeit, sie zu löschen.

* [Aus SFDC löschen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) Flussaktion: Hiermit wird ein Lead in SFDC gelöscht, Sie können jedoch auch eine Person in Marketo löschen.
* Wenn ein Lead in [!DNL Salesforce] gelöscht wird (eine Person jedoch nicht in Marketo gelöscht wird) und anschließend die Flussaktion [Mit synchronisieren [!DNL Salesforce]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) durchläuft, wird in [!DNL Salesforce] ein neuer Lead erstellt.
