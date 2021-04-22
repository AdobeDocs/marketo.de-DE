---
unique-page-id: 2953465
description: SFDC-Synchronisierung - Umwandlung eines Interessenten in einen Kontakt in Salesforce - Marketo Docs - Produktdokumentation
title: SFDC-Synchronisierung - Umwandlung eines Interessenten in einen Kontakt in Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# SFDC-Synchronisierung: Konvertieren eines Interessenten in einen Kontakt in Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Stellen Sie sich drei verschiedene Szenarien in Salesforce vor: (nicht mit dem Schritt [Benutzerfluss konvertieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) in Marketo)

1. Umrechnung eines Interessenten in einen **neuen Kontakt und ein neues Konto**
1. Konvertieren eines Interessenten in einen **neuen Kontakt** in ein **vorhandenes Konto**

1. Konvertieren eines Interessenten in einen **vorhandenen Kontakt** in einem **vorhandenen Konto** (dies funktioniert genauso wie [Zusammenführen](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md))

In allen drei Fällen haben Sie den Kontakt **1 und keine Kontakte in Salesforce und 1 Kontakt und keine Personen in Marketo.**

In Marketo wird der Datensatz jetzt einen SFDC-Typ = Kontakt haben.

>[!TIP]
>
>Stellen Sie bei der Konvertierung in Salesforce sicher, dass Ihre benutzerdefinierten Interessentenfelder gut](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm) zugeordnet sind. [ Sie wollen keine Daten verlieren.

Sie können Trigger und Filter mit folgenden Methoden durchführen: &quot;Blei wird konvertiert&quot;und &quot;Blei wurde konvertiert&quot;.
