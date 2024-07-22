---
unique-page-id: 2953465
description: SFDC Sync - Konvertieren eines Leads in einen Kontakt in Salesforce - Marketo Docs - Produktdokumentation
title: SFDC Sync - Konvertieren eines Leads in einen Kontakt in Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%

---

# SFDC Sync: Konvertieren eines Leads in einen Kontakt in Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Stellen Sie sich drei verschiedene Szenarien in Salesforce vor: (nicht mit dem Schritt [Personenstrom konvertieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"} in Marketo Engage)

1. Konvertieren eines Leads in einen **neuen Kontakt und ein neues Konto**
1. Konvertieren eines Leads in einen **neuen Kontakt** in einem **vorhandenen Konto**

1. Konvertieren eines Leads in einen **vorhandenen Kontakt** in einem **vorhandenen Konto** (funktioniert genauso wie beim Zusammenführen](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"})[

In allen drei Fällen erhalten Sie **1 Kontakt und keine Leads in Salesforce und 1 Kontakt und keine Personen in Marketo.**

In Marketo weist der Datensatz jetzt einen SFDC-Typ = Kontakt auf.

>[!TIP]
>
>Stellen Sie beim Konvertieren in Salesforce sicher, dass Ihre benutzerdefinierten Felder für [Lead korrekt zugeordnet sind](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm){target="_blank"}. Sie wollen keine Daten verlieren.

Sie können den Trigger und die Filterung wie folgt durchführen: &quot;Lead ist konvertiert&quot;und &quot;Lead wurde konvertiert&quot;.
