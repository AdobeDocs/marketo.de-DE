---
unique-page-id: 7515131
description: Erfahren Sie, wie das Löschen von Leads und Kontakten zwischen Salesforce und Marketo funktioniert. Erfahren Sie mehr über die Flussaktionen „Person löschen“ und „Aus SFDC löschen“.
title: SFDC-Synchronisierung - Löschen eines Leads/Kontakts
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/v0nRloqmlp-iedcmE4DdATxpYXnvB13cxkEn7809Hy4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 149
ht-degree: 4%

---

# SFDC-Synchronisierung: Löschen eines Leads/Kontakts {#sfdc-sync-deleting-a-lead-contact}

Im Folgenden finden Sie einige Details:

* Marketo löscht Personen nicht automatisch, nur weil Leads in [!DNL Salesforce] gelöscht wurden. Stattdessen wird das Feld-Flag &quot;SFDC wird gelöscht“ auf „true“ gesetzt. Sie können bei Bedarf Trigger aus diesem Feld in Marketo löschen.
* [Person löschen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) Flussaktion. Dadurch wird eine Person in MKTO gelöscht, aber Sie haben auch in `Salesforce` die Möglichkeit, sie zu löschen.

* [Aus SFDC löschen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) Flussaktion: Hiermit wird ein Lead in SFDC gelöscht, Sie können jedoch auch eine Person in Marketo löschen.
* Wenn ein Lead in [!DNL Salesforce] gelöscht wird (eine Person jedoch nicht in Marketo gelöscht wird) und anschließend die Flussaktion [Mit synchronisieren [!DNL Salesforce]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) durchläuft, wird in [!DNL Salesforce] ein neuer Lead erstellt.
