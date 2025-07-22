---
unique-page-id: 3571844
description: Microsoft Dynamics-Synchronisierung - Opportunity-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Microsoft Dynamics-Synchronisierung - Opportunity-Synchronisierung
exl-id: dcb72f28-c980-4183-8473-a1e5ad0c8d3c
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics]: Opportunity-Synchronisation {#microsoft-dynamics-sync-opportunity-sync}

Die Synchronisierung von Marketo zu [!DNL Dynamics] ist extrem leistungsstark. Im Folgenden finden Sie alle Details zur Opportunity-Synchronisierung:

## Wie werden Opportunity-Details zwischen den beiden Systemen synchron gehalten? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

Die Opportunity-Synchronisation ist eine Möglichkeit - [!DNL Dynamics] zu Marketo. Wenn Sie in [!DNL Dynamics] Änderungen an einer Opportunity vornehmen, wird Ihre Aktualisierung in Marketo übernommen.

## Kann ich mit Marketo in [!DNL Dynamics] eine Opportunity erstellen? {#can-i-create-an-opportunity-in-dynamics-using-marketo}

Nein, Sie müssen die Opportunity in [!DNL Dynamics] erstellen. Sie wird automatisch mit Marketo synchronisiert.

## Welche Felder werden mit Marketo synchronisiert? {#what-fields-will-sync-to-marketo}

Sie können [ Setup Felder auswählen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} die synchronisiert werden sollen.

## Wie ist ein Konto/Kontakt mit einer Opportunity verbunden? {#how-is-an-account-contact-associated-with-an-opportunity}

Der Kontakt/das Konto kann auf zwei Arten mit Opportunity verknüpft werden:

* Beim Erstellen einer Opportunity können der Kontakt (Suchfeld im zu kontaktierenden Formular) und/oder das Konto (Suchfeld im zu kontaktierenden Formular) festgelegt werden. In beiden Fällen werden diese Werte im Feld Potenzieller Kunde (customerID) in Dynamics gespeichert. Dieses Feld wird nicht im Opportunity-Formular angezeigt, kann jedoch aus den Einstellungen hinzugefügt werden. Dieses Feld kann nur einen Wert enthalten, entweder Kontakt oder Konto. Marketo führt folgende Schritte durch:

   * Wenn der Kontaktwert festgelegt ist und das Konto leer bleibt, erstellt Marketo eine `opportunitycontactrole` und legt das Konto für die Opportunity auf das Konto des Kontakts fest. Wenn der Kontakt kein Konto hat, bleibt dieses Feld leer.
   * Wenn der Kontowert festgelegt ist und der Kontakt leer gelassen wird, legt Marketo das Konto nur für die Opportunity auf dieses Konto fest.
   * Wenn beide Werte festgelegt sind, wählt Dynamics das Konto als Wert für die Kunden-ID aus, sodass das Verhalten dasselbe wie oben wäre.


* Über Stakeholder: Dynamics verwendet Verbindungen, um über Stakeholder von der Seite „Opportunity erstellen“ aus eine Opportunity zu kontaktieren. Dazu erstellen wir für jeden neuen Stakeholder einen `opportunitycontactrole`.
