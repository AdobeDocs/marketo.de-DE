---
unique-page-id: 2953467
description: SFDC-Synchronisierung - Opportunity-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: SFDC Sync - Opportunity Sync
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 7%

---

# SFDC Sync: Opportunity Sync {#sfdc-sync-opportunity-sync}

## Wie werden Opportunity-Details zwischen den beiden Systemen synchron gehalten? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

Die Synchronisierung erfolgt in eine Richtung: von [!DNL Salesforce] zu Marketo. Aktualisierungen der Opportunities in [!DNL Salesforce] werden mit Marketo synchronisiert.

>[!NOTE]
>
>Die [Anmeldeinformationen, die Sie in Marketo für eingeben [!DNL Salesforce]](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) werden verwendet, um Daten zu synchronisieren. Nur Daten, auf die diese Anmeldeinformationen Zugriff haben, werden einbezogen.

## Kann ich eine Opportunity-Synchronisation starten? {#can-i-initiate-an-opportunity-sync}

Nein, das kannst du nicht. Die Änderungen an einer Opportunity in [!DNL Salesforce] werden automatisch mit Marketo synchronisiert.

## Unterstützt Marketo mehr als eine Währung im Opportunity-Betrag? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

Nein, Marketo unterstützt nur eine Währung. Der Opportunity-Betrag wird von [!DNL Salesforce] synchronisiert, aber die Währung ist die [Standardwährung](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription) in Ihrem Marketo-Abonnement.

## Wie verknüpft Marketo Opportunities und Kontakte? {#how-does-marketo-associate-opportunities-and-contacts}

Marketo verknüpft Opportunities und Kontakte mithilfe von [Opportunity-Kontaktrollen](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm){target="_blank"}. Opportunities ohne zugewiesene Kontaktrollen werden mit Marketo synchronisiert, gehören aber niemandem. Beispielsweise qualifiziert die Person den Filter „Hat Opportunity“ nicht.

## Wie kann ich alle Chancen einer Person sehen? {#how-can-i-see-all-the-opportunities-of-a-person}

Sie können eine Liste von Opportunitys auf der Registerkarte **[!UICONTROL Opportunity-Info]** auf der Seite [Personendetails](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) anzeigen.

## Welche Trigger/Filter beziehen sich auf Opportunities? {#what-are-the-triggers-filters-related-to-opportunity}

Auslöser:

* Zu Opportunity hinzugefügt
* Aus Opportunity entfernt
* Opportunity wird aktualisiert

Filter:

* Hat Opportunity
* Opportunity wurde aktualisiert/Opportunity wurde nicht aktualisiert
* wurde zu Opportunity hinzugefügt/wurde nicht zu Opportunity hinzugefügt
* wurde aus Opportunity entfernt/wurde nicht aus Opportunity entfernt
* Opty-Gesamtbetrag
* Anzahl Möglichkeiten
* Erwarteter Opty-Gesamtumsatz

>[!TIP]
>
>Sehen Sie sich die Einschränkungen für Filter und Trigger an. Viele coole Details da drin.
>
>Erstellen Sie einfach ein neues Feld im Opportunity-Objekt in [!DNL Salesforce] und es wird automatisch zu einer Einschränkung!
