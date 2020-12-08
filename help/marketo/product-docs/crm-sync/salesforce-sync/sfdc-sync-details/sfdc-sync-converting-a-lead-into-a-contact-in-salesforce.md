---
unique-page-id: 2953465
description: SFDC-Synchronisierung - Umwandlung eines Interessenten in einen Kontakt in Salesforce - Marketo Docs - Produktdokumentation
title: SFDC-Synchronisierung - Umwandlung eines Interessenten in einen Kontakt in Salesforce
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---


# SFDC-Synchronisierung: Umwandlung eines Interessenten in einen Kontakt in Salesforce {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Stellen Sie sich drei verschiedene Szenarien in Salesforce vor: (nicht mit dem Schritt [&quot;Person](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) konvertieren&quot;in Marketing)

1. Einen Interessenten in einen **neuen Kontakt und ein neues Konto umwandeln**
1. Konvertieren eines Interessenten in einen **neuen Kontakt** in einem **vorhandenen Konto**

1. Konvertieren eines Interessenten in einen **vorhandenen Kontakt** in einem **vorhandenen Konto** (funktioniert genauso wie das [Zusammenführen](sfdc-sync-merging-a-lead-contact-person.md))

In allen drei Fällen haben Sie **1 Kontakt und keine Leads in Salesforce und 1 Kontakt und keine Leute in Marketo.**

In Marketo wird der Datensatz jetzt einen SFDC-Typ = Kontakt haben.

>[!TIP]
>
>Stellen Sie bei der Konvertierung in Salesforce sicher, dass Ihre [Interessentenbenutzerfelder gut](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm)zugeordnet sind. Sie wollen keine Daten verlieren.

Sie können Folgendes auslösen und filtern: &quot;Blei wird konvertiert&quot;und &quot;Blei wurde konvertiert&quot;.