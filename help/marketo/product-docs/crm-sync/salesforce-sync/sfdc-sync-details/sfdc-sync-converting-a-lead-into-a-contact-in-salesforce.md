---
unique-page-id: 2953465
description: SFDC-Synchronisierung - Konvertieren eines Leads in einen Kontakt in Salesforce - Marketo-Dokumente - Produktdokumentation
title: SFDC-Synchronisation - Konvertieren eines Leads in einen Kontakt in Salesforce
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# SFDC-Synchronisation: Konvertieren eines Leads in einen Kontakt in [!DNL Salesforce] {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Stellen Sie sich drei verschiedene Szenarien in [!DNL Salesforce] vor: (ohne Verwendung des Schritts [Personenfluss konvertieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) in Marketo)

1. Lead in einen **Kontakt und ein neues Konto**
1. Lead in einen **neuen Kontakt** in einem (**Konto umwandeln**

1. Leads in einen **vorhandenen Kontakt** in einem **vorhandenen Konto** konvertieren (funktioniert genauso wie [Zusammenführen](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"})

In allen drei Fällen haben Sie am Ende **1 Kontakt und keine Leads in [!DNL Salesforce] und 1 Kontakt und keine Personen in Marketo.**

In Marketo hat der Datensatz jetzt den SFDC-Typ = Kontakt.

>[!TIP]
>
>Stellen Sie beim Konvertieren in [!DNL Salesforce] sicher, [ Ihre benutzerdefinierten Lead-Felder gut zugeordnet ](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm). Sie möchten keine Daten verlieren.

Sie können Trigger erstellen und filtern mit: &quot;[!UICONTROL Lead ist konvertiert]&quot; und &quot;[!UICONTROL Lead wurde konvertiert]&quot;.
