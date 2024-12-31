---
unique-page-id: 30082174
description: Interessante Momente in Sales Connect - Marketo-Dokumentation - Produktdokumentation
title: Interessante Momente in Sales Connect
exl-id: 210f31d1-606a-479d-8a2b-351b2b1a7678
feature: Marketo Sales Connect
source-git-commit: 3a3287ed20962a052e0015161e34e33a95dd450a
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Interessante Momente in Sales Connect {#interesting-moments-in-sales-connect}

Interessante Momente sind der Schlüssel zur Kommunikation mit Ihrem Vertriebsteam über Marketo Sales Connect.

>[!AVAILABILITY]
>
>Diese sind nur für Kunden von [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/using-interesting-moments.md) und Marketo Sales Connect verfügbar.

>[!PREREQUISITES]
>
>* Sie müssen über eine [Verbindung mit dem Salesforce CRM“ ](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md){target="_blank"}
>* Sie müssen der Lead- oder Kontaktinhaber in Salesforce sein
>* Sie müssen Zugriff auf haben [Zugriff auf die Marketo Engage-Verbindung gewähren](/help/marketo/product-docs/marketo-sales-connect/marketo/granting-access-to-users.md){target="_blank"}

## Was ist ein interessanter Moment? {#what-is-an-interesting-moment}

Das liegt an dir! Sie entscheiden, welche Informationen für Ihr Vertriebsteam relevant sind. Ihr Vertriebsteam möchte möglicherweise wissen, wann ein Lead:

* Besucht die Preisseite auf Ihrer Website
* Klickt auf einen Link in einer E-Mail zur Produktankündigung
* Fordert eine Produktdemo an

## Wie erschaffe ich einen interessanten Moment? {#how-do-i-create-an-interesting-moment}

1. Wählen Sie eine [intelligente Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md) vorzugsweise eine, die Ihr Vertriebsteam bei Auslösung interessant finden würde.

   ![](assets/image2015-1-8-18-3a8-3a54.png)

1. Ziehen Sie über den **Interessante Momente** Flussschritt.

   ![](assets/image2015-1-8-18-3a15-3a20.png)

1. Wählen Sie einen **Typ** aus (E-Mail, Meilenstein oder Web).

   ![](assets/image2015-1-8-18-3a17-3a16.png)

1. Schreiben Sie eine Nachricht an Ihr Vertriebsteam im Feld **Beschreibung**, in der erläutert wird, warum diese Aktion wichtig ist.

   ![](assets/image2015-1-8-18-3a18-3a23.png)

   >[!NOTE]
   >
   >Marketo fügt auch das Datum hinzu, an dem es aufgetreten ist, und wie der interessante Moment hinzugefügt wurde (d. h. Lead-Aktion > Flussschritt, SOAP-API).

## Wie sieht ein interessanter Moment in Marketo aus?  {#what-does-an-interesting-moment-look-like-in-marketo}

Interessante Momente werden im Aktivitätsprotokoll eines [Leads) ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/image2015-1-14-18-3a45-3a58.png)

## Wie sieht ein interessanter Moment in Sales Connect aus? {#what-does-an-interesting-moment-look-like-in-sales-connect}

Interessante Momente werden in Echtzeit im Live-Feed eines Benutzers angezeigt. Wir verwenden die Lead-Eigentümer-ID in Salesforce, um den Nutzern die interessanten Momente relevanter Leads zu zeigen, deren Besitzer sie sind. Benutzer können Leads schnell über E-Mail/Telefon/Verkaufskampagne verfolgen, indem sie auf die Dropdown-Liste neben dem Namen des Leads klicken.

![](assets/engagement.jpg)
