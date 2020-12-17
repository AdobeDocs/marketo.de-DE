---
unique-page-id: 2953465
description: SFDC-Synchronisierung - Umwandlung eines Interessenten in einen Kontakt in Salesforce - Marketo Docs - Produktdokumentation
title: SFDC-Synchronisierung - Umwandlung eines Interessenten in einen Kontakt in Salesforce
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# SFDC-Synchronisierung: Konvertieren eines Interessenten in einen Kontakt in Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Stellen Sie sich drei verschiedene Szenarien in Salesforce vor: (nicht mit dem [Schritt \&quot;Person konvertieren\&quot; unter ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) in Markieren)

1. Umrechnung eines Interessenten in einen **neuen Kontakt und ein neues Konto**
1. Konvertieren eines Interessenten in einen **neuen Kontakt** in ein **vorhandenes Konto**

1. Konvertieren eines Interessenten in einen **vorhandenen Kontakt** in einem **vorhandenen Konto** (dies funktioniert genauso wie [Zusammenführen](sfdc-sync-merging-a-lead-contact-person.md))

In allen drei Fällen haben Sie den Kontakt **1 und keine Kontakte in Salesforce und 1 Kontakt und keine Personen in Marketo.**

In Marketo wird der Datensatz jetzt einen SFDC-Typ = Kontakt haben.

>[!TIP]
>
>Stellen Sie bei der Konvertierung in Salesforce sicher, dass Ihre benutzerdefinierten Interessentenfelder gut[ zugeordnet sind. ](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm) Sie wollen keine Daten verlieren.

Sie können Folgendes auslösen und filtern: &quot;Blei wird konvertiert&quot;und &quot;Blei wurde konvertiert&quot;.