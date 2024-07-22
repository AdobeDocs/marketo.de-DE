---
unique-page-id: 30082174
description: Interessante Momente in Sales Connect - Marketo Docs - Produktdokumentation
title: Interessante Momente in Sales Connect
exl-id: 210f31d1-606a-479d-8a2b-351b2b1a7678
feature: Marketo Sales Connect
source-git-commit: 3a3287ed20962a052e0015161e34e33a95dd450a
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Interessante Momente in Sales Connect {#interesting-moments-in-sales-connect}

Interessante Momente sind der Schlüssel zur Kommunikation mit Ihrem Verkaufsteam über Marketo Sales Connect.

>[!AVAILABILITY]
>
>Diese sind nur für Kunden von [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/using-interesting-moments.md) und Marketo Sales Connect verfügbar.

>[!PREREQUISITES]
>
>* Sie müssen über eine [Verbindung zum Salesforce CRM](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md){target="_blank"} verfügen.
>* Sie müssen Lead- oder Kontaktinhaber in Salesforce sein.
>* Sie müssen Zugriff auf [Zugriff auf die Marketo Engage-Verbindung gewähren](/help/marketo/product-docs/marketo-sales-connect/marketo/granting-access-to-users.md){target="_blank"} haben

## Was ist ein interessanter Moment? {#what-is-an-interesting-moment}

Das liegt an dir! Sie entscheiden, welche Informationen für Ihr Verkaufsteam relevant sind. Ihr Verkaufsteam möchte möglicherweise wissen, wann ein Lead:

* Besucht die Preisseite auf Ihrer Website
* Klicken Sie auf einen Link in einer neuen Produktankündigungs-E-Mail
* Anfordern einer Produktdemo

## Wie erstelle ich einen interessanten Moment? {#how-do-i-create-an-interesting-moment}

1. Wählen Sie eine [intelligente Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), vorzugsweise eine, die Ihr Verkaufsteam interessant finden würde, wenn sie ausgelöst wird.

   ![](assets/image2015-1-8-18-3a8-3a54.png)

1. Ziehen Sie über den Flussschritt **Interessante Momente**.

   ![](assets/image2015-1-8-18-3a15-3a20.png)

1. Wählen Sie einen **Typ** aus (E-Mail, Meilenstein oder Web).

   ![](assets/image2015-1-8-18-3a17-3a16.png)

1. Schreiben Sie im Feld **Beschreibung** eine Nachricht an Ihr Verkaufsteam, die erklärt, warum diese Aktion wichtig ist.

   ![](assets/image2015-1-8-18-3a18-3a23.png)

   >[!NOTE]
   >
   >Marketo fügt außerdem das Datum, an dem es aufgetreten ist, und die Art hinzu, wie der interessante Moment hinzugefügt wurde (d. h. Lead-Aktion > Flussschritt, SOAP API).

## Wie sieht ein interessanter Moment in Marketo aus?  {#what-does-an-interesting-moment-look-like-in-marketo}

Interessante Momente werden im Aktivitätsprotokoll eines [Leads](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) angezeigt.

![](assets/image2015-1-14-18-3a45-3a58.png)

## Wie sieht ein interessanter Moment in Sales Connect aus? {#what-does-an-interesting-moment-look-like-in-sales-connect}

Interessante Momente werden in Echtzeit im Live Feed eines Benutzers angezeigt. Wir verwenden die Lead-Eigentümer-ID in Salesforce, um die interessanten Momente der Benutzer zu relevanten Leads zu zeigen, deren Inhaber sie sind. Benutzer können schnell über E-Mail-, Telefon- oder Vertriebskampagnen auf Leads reagieren, indem sie auf das Dropdown-Menü neben dem Namen des Leads klicken.

![](assets/engagement.jpg)
