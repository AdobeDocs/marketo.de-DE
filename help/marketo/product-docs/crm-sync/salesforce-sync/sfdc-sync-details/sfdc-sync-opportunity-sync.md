---
unique-page-id: 2953467
description: SFDC Sync - Opportunity Sync - Marketo Docs - Produktdokumentation
title: SFDC Sync - Opportunity Sync
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 6%

---

# SFDC Sync: Opportunity Sync {#sfdc-sync-opportunity-sync}

## Wie werden Opportunitätsdetails zwischen den beiden Systemen synchronisiert? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

Die Synchronisation ist eine Möglichkeit: von Salesforce zu Marketo Engage. Aktualisierungen der Möglichkeiten in Salesforce werden mit Marketo synchronisiert.

>[!NOTE]
>
>Die [Anmeldedaten, die Sie in Marketo für Salesforce eingeben](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} werden zum Synchronisieren von Daten verwendet. Es werden nur Daten einbezogen, auf die diese Anmeldeinformationen Zugriff haben.

## Kann ich eine Opportunity Sync starten? {#can-i-initiate-an-opportunity-sync}

Nein, das kannst du nicht. Die Änderungen an allen Möglichkeiten in Salesforce werden automatisch mit Marketo synchronisiert.

## Unterstützt Marketo mehr als eine Währung im Opportunity Amount? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

Nein, Marketo unterstützt nur eine Währung. Der Opportunitätsbetrag wird von Salesforce synchronisiert, die Währung ist jedoch der [Standardwährung](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription){target="_blank"} in Ihrem Marketo-Abonnement.

## Wie verknüpft Marketo Chancen und Kontakte? {#how-does-marketo-associate-opportunities-and-contacts}

Marketo verknüpft Chancen und Kontakte mithilfe von [Kontaktrollen für Opportunity](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm){target="_blank"}. Chancen ohne zugewiesene Kontaktrollen werden mit Marketo synchronisiert, gehören jedoch niemandem. Beispielsweise qualifiziert die Person den Filter Hat Chancen nicht.

## Wie kann ich alle Möglichkeiten eines Menschen sehen? {#how-can-i-see-all-the-opportunities-of-a-person}

Eine Liste der Möglichkeiten finden Sie im Abschnitt **Opportunity Info** im [Personendetails](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} Seite.

## Welche Trigger/Filter beziehen sich auf Chancen? {#what-are-the-triggers-filters-related-to-opportunity}

Auslöser:

* Einer Gelegenheit hinzugefügt
* Aus Opportunity entfernt
* Opportunity wird aktualisiert

Filter:

* Hat Opportunity
* Die Chancen wurden aktualisiert/die Chancen wurden nicht aktualisiert.
* wurde zu Opportunity hinzugefügt/wurde nicht zu Opportunity hinzugefügt
* Aus Opportunity entfernt/Nicht aus Opportunity entfernt
* Opty-Gesamtbetrag
* Anzahl Opportunities
* Erwarteter Opty-Gesamtumsatz

>[!TIP]
>
>Sehen Sie sich die Einschränkungen für Filter und Trigger an. Viele coole Details sind da drin.
>
>Machen Sie einfach ein neues Feld im Opportunitätsobjekt in Salesforce und es wird automatisch zu einer Einschränkung!
