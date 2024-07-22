---
unique-page-id: 2951640
description: Verwenden interessanter Momente - Marketo Docs - Produktdokumentation
title: Verwenden interessanter Momente
exl-id: ccf7664b-08e1-490a-a3f9-5fa3bd8fb05f
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# Verwenden interessanter Momente {#using-interesting-moments}

Interessante Momente sind der Schlüssel zur Kommunikation mit Ihrem Verkaufsteam über die Marketo Sales Insight-App.

>[!AVAILABILITY]
>
>Diese sind nur für Kunden von Marketo Sales Insight und [Marketo Sales Connect](/help/marketo/product-docs/marketo-sales-connect/marketo/interesting-moments-in-sales-connect.md) verfügbar.

## Was ist ein interessanter Moment? {#what-is-an-interesting-moment}

Das liegt an dir! Sie entscheiden, welche Informationen für Ihr Verkaufsteam relevant sind. Ihr Verkaufsteam möchte möglicherweise wissen, wann ein Lead:

* Besucht die Preisseite auf Ihrer Website
* Klicken Sie auf einen Link in einer neuen Produktankündigungs-E-Mail
* Anfordern einer Produktdemo

## Wie erstelle ich einen interessanten Moment?  {#how-do-i-create-an-interesting-moment}

1. Wählen Sie eine [intelligente Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), vorzugsweise eine, die Ihr Verkaufsteam interessant finden würde, wenn sie ausgelöst wird.

   ![](assets/using-interesting-moments-1.png)

1. Ziehen Sie über den Flussschritt **Interessante Momente**.

   ![](assets/using-interesting-moments-2.png)

1. Wählen Sie einen **Typ** aus (E-Mail, Meilenstein oder Web).

   ![](assets/using-interesting-moments-3.png)

1. Schreiben Sie im Feld **Beschreibung** eine Nachricht an Ihr Verkaufsteam, die erklärt, warum diese Aktion wichtig ist.

   ![](assets/using-interesting-moments-4.png)

   >[!NOTE]
   >
   >Marketo fügt außerdem das Datum, an dem es aufgetreten ist, und die Art hinzu, wie der interessante Moment hinzugefügt wurde (d. h. Lead-Aktion > Flussschritt, SOAP API).

## Wie kann das noch interessanter werden?  {#how-can-this-get-even-more-interesting}

Token! Fügen Sie sie im Beschreibungsfeld hinzu, um Ihrem Verkaufsteam spezifischere Informationen wie die Betreffzeile der E-Mail, die der Lead geöffnet hat, oder wer sie gesendet hat, bereitzustellen. Überprüfen Sie, welche Token im Glossar [Token für interessante Momente](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) verfügbar sind.

>[!TIP]
>
>Beginnen Sie mit fünf interessanten Momenten und arbeiten Sie dann mit Ihrem Verkaufsteam zusammen, um zu bestimmen, welche Informationen sie sehen möchten.

## Wie sieht ein interessanter Moment in Marketo aus?  {#what-does-an-interesting-moment-look-like-in-marketo}

Interessante Momente werden im Aktivitätsprotokoll eines [Leads](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) angezeigt.

![](assets/using-interesting-moments-5.png)

## Wie sieht ein interessanter Moment in Salesforce aus?  {#what-does-an-interesting-moment-look-like-in-salesforce}

Sobald Sie [ die Marketo Sales Insight App installiert haben, werden interessante Momente auf den Interessenten-, Kontakt-, Konto- oder Opportunity-Seiten angezeigt. ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) Sie werden auch im Sales Insight-Dashboard im Lead-Feed, Best Bets und Watch-Liste angezeigt.

![](assets/using-interesting-moments-6.png)

## Wie sieht ein interessanter Moment in Salesforce1 aus? {#what-does-an-interesting-moment-look-like-in-salesforce-1}

Nachdem Sie Marketo Sales Insight für Salesforce1 installiert oder aktualisiert haben, werden unter den entsprechenden Links des Leads interessante Momente angezeigt.

![](assets/using-interesting-moments-7.png)

## Abonnieren von interessanten Momenten {#subscribe-to-interesting-moments}

Sie können einen interessanten Moment abonnieren, indem Sie entweder auf der Registerkarte Interessanter Moment oder im Lead-Feed auf die Schaltfläche Abonnieren klicken. Die folgenden Schritte sind für beide identisch.

1. Klicken Sie auf das Symbol Abonnieren . Navigieren Sie dann zum Tab E-Mail-Anmeldung .

1. Sie können den Typ des E-Mail-Warnhinweises auswählen, den Sie erhalten möchten, basierend auf Name, Konto, Typ oder Beschreibung.

1. Wählen Sie die E-Mail-Adresse(n) aus, an die Sie die Warnungen senden möchten (Sie/die Teammitglieder)

1. Klicken Sie auf **Abonnieren**.

>[!NOTE]
>
>Beim Abonnieren von interessanten Ereignistypen oder -beschreibungen erhält der Benutzer E-Mail-Benachrichtigungen für Personen (Leads/Kontakte), die ihm gehören, wenn er einen interessanten Moment Trigger, der mit diesem Typ oder dieser Beschreibung übereinstimmt.

![](assets/using-interesting-moments-8.png)
