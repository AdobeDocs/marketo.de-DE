---
unique-page-id: 2953465
description: SFDC Sync - Konvertieren eines Leads in einen Kontakt in Salesforce - Marketo Docs - Produktdokumentation
title: SFDC Sync - Konvertieren eines Leads in einen Kontakt in Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# SFDC Sync: Konvertieren eines Leads in einen Kontakt in Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Stellen Sie sich drei verschiedene Szenarien in Salesforce vor: (Nicht verwenden von [Schritt zum Konvertieren des Personen-Flusses](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) in Marketo)

1. Konvertieren eines Leads in eine **neuer Kontakt und neues Konto**
1. Konvertieren eines Leads in eine **neuer Kontakt** in einer **bestehendes Konto**

1. Konvertieren eines Leads in eine **vorhandener Kontakt** in einer **bestehendes Konto** (diese Funktion entspricht [Zusammenführen](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md))

In allen drei Fällen **1 Kontakt und keine Leads in Salesforce und 1 Kontakt und keine Personen in Marketo.**

In Marketo weist der Datensatz jetzt einen SFDC-Typ = Kontakt auf.

>[!TIP]
>
>Stellen Sie beim Konvertieren in Salesforce sicher, dass Ihre [Lead-benutzerdefinierte Felder sind gut zugeordnet](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). Sie wollen keine Daten verlieren.

Sie können Trigger und Filter wie folgt durchführen: &quot;Blei ist konvertiert&quot;und &quot;Blei wurde konvertiert&quot;.
