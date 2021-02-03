---
unique-page-id: 2953467
description: SFDC-Synchronisierung - Opportunity Sync - Marketing Docs - Produktdokumentation
title: SFDC-Synchronisierung - Opportunity Sync
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---


# SFDC-Synchronisierung: Opportunity Sync {#sfdc-sync-opportunity-sync}

## Wie werden Opportunitätsdetails zwischen den beiden Systemen synchronisiert? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

Die Synchronisierung erfolgt auf eine Weise: von Salesforce bis Marketo. Aktualisierungen der Möglichkeiten in Salesforce werden mit Marketo synchronisiert.

>[!NOTE]
>
>Die [Anmeldedaten, die Sie in Marketo für Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) eingeben, werden zum Synchronisieren der Daten verwendet. Es werden nur Daten einbezogen, auf die diese Anmeldeinformationen Zugriff haben.

## Kann ich eine Opportunity Sync starten? {#can-i-initiate-an-opportunity-sync}

Nein, das kannst du nicht. Die Änderungen an allen Möglichkeiten in Salesforce werden automatisch mit Marketo synchronisiert.

## Unterstützt Marketo mehr als eine Währung im Opportunity Amount? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

Nein, Marketo unterstützt nur eine Währung. Der Opportunitätsbetrag wird von Salesforce synchronisiert, die Währung ist jedoch die [Standardwährung](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription) in Ihrem Marketing-Abonnement.

## Wie verbindet Marketo Chancen und Kontakte? {#how-does-marketo-associate-opportunities-and-contacts}

Marketo verknüpft Chancen und Kontakte mit [Gelegenheitskontaktrollen](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm). Gelegenheiten ohne zugewiesene Kontaktrollen werden mit Marketo synchronisiert, gehören aber niemandem. Beispielsweise wird der Filter &quot;Hat Gelegenheit&quot;nicht für die Person qualifiziert.

## Wie kann ich alle Möglichkeiten einer Person sehen? {#how-can-i-see-all-the-opportunities-of-a-person}

Sie können eine Liste von Möglichkeiten auf der Registerkarte **Opportunity Info** auf der Seite [Personendetail](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) Ansicht.

## Welche Trigger/Filter stehen im Zusammenhang mit Chancen? {#what-are-the-triggers-filters-related-to-opportunity}

Trigger:

* Der Gelegenheit hinzugefügt
* Aus Gelegenheit entfernt
* Chancen werden aktualisiert

Filter:

* Hat Chancen
* Gelegenheit wurde aktualisiert/Keine Gelegenheit wurde aktualisiert
* Der Möglichkeit hinzugefügt/Nicht der Möglichkeit hinzugefügt
* Aus der Gelegenheit entfernt/Nicht aus der Gelegenheit entfernt
* Optimalbetrag gesamt
* Anzahl der Optionen
* Erwarteter Gesamtumsatz der Option

>[!TIP]
>
>Sehen Sie sich die Einschränkungen für Filter und Trigger an. Viele coole Details.
>
>Machen Sie einfach ein neues Feld im Opportunitätsobjekt in Salesforce und es wird automatisch eine Einschränkung!
