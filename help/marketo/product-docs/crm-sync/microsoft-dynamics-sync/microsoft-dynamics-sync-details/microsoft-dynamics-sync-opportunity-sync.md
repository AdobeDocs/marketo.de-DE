---
unique-page-id: 3571844
description: Microsoft Dynamics Sync - Opportunity Sync - Marketo Docs - Produktdokumentation
title: Synchronisation von Microsoft Dynamics - Opportunity Sync
exl-id: dcb72f28-c980-4183-8473-a1e5ad0c8d3c
feature: Microsoft Dynamics
source-git-commit: 9a130e0b2ec84b638adf37188b65b565b090fe1b
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Opportunity Sync {#microsoft-dynamics-sync-opportunity-sync}

Marketo Engage to Dynamics Synchronisation ist super leistungsstark. Hier finden Sie alle Details zur Opportunity-Synchronisation.

## Wie werden Opportunitätsdetails zwischen den beiden Systemen synchronisiert? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

Die Opportunitäts-Synchronisation ist eine Möglichkeit - Dynamics zu Marketo. Wenn Sie Änderungen an einer Gelegenheit in Dynamics vornehmen, wird Ihre Aktualisierung in Marketo übernommen.

## Kann ich mit Marketo eine Chance in Dynamics schaffen? {#can-i-create-an-opportunity-in-dynamics-using-marketo}

Nein, Sie müssen die Möglichkeit in Dynamics erstellen und sie wird automatisch mit Marketo synchronisiert.

## Welche Felder werden mit Marketo synchronisiert? {#what-fields-will-sync-to-marketo}

Sie können [Auswahl der zu synchronisierenden Felder](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} während der Einrichtung.

## Wie ist ein Konto/Kontakt mit einer Chance verbunden? {#how-is-an-account-contact-associated-with-an-opportunity}

Der Kontakt/das Konto kann auf zwei Arten mit Opportunity verknüpft werden:

* Beim Erstellen einer Gelegenheit können Sie den Kontakt (Suchfeld im Formular, das kontaktiert werden soll) und/oder das Konto (Suchfeld im Formular, das dem Konto zugeordnet werden soll) festlegen. In beiden Fällen werden diese Werte im Feld Potenzieller Kunde (customerid) in Dynamics gespeichert. Dieses Feld wird nicht im Opportunity-Formular angezeigt, kann aber über die Einstellungen hinzugefügt werden. Dieses Feld kann nur einen Wert enthalten, entweder Kontakt oder Konto. Marketo führt Folgendes aus:

   * Wenn der Kontaktwert festgelegt und das Konto leer gelassen wird, erstellt Marketo eine `opportunitycontactrole` und legt das Konto für die Möglichkeit auf das Konto des Kontakts fest. Wenn der Kontakt kein Konto hat, bleibt dieses Feld leer.
   * Wenn der Kontowert festgelegt ist und der Kontakt leer gelassen wird, legt Marketo das Konto nur bei der Möglichkeit dieses Kontos fest.
   * Wenn beide Werte festgelegt sind, wählt Dynamics das Konto als Wert für customerid aus, sodass das Verhalten mit dem oben genannten übereinstimmt.


* Über Stakeholder: Dynamics nutzt Verbindungen, um über Interessengruppen aus der Seite zum Erstellen von Opportunities zu verbinden. Dazu erstellen wir eine `opportunitycontactrole` für jeden neuen Verantwortlichen.
