---
unique-page-id: 14352477
description: Push to Sales Connect - Marketo Docs - Produktdokumentation
title: In Sales Connect pushen
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 4%

---

# In Sales Connect pushen {#push-to-sales-connect}

Über die Schaltfläche Push to Tout erhalten Sie eine Liste Ihrer Kontakte/Leads in Salesforce und können diese in eine Gruppe in Sales Connect übertragen. Sie können dann schnell eine anpassbare Gruppen-E-Mail mit angehängtem Tout-Tracking senden.

## Anforderungen {#requirements}

* Sales Connect Salesforce-Paket, das von Salesforce Admin installiert wird

* Schaltfläche &quot;Push to Sales Connect&quot;installiert, um die Listenansicht von Salesforce Admin aufzurufen

* Salesforce-Verbindung mit Sales Connect für Benutzer, die Push durchführen

## Verfahren {#how-to}

1. Klicken Sie auf **Lead/Kontakt** in Salesforce.
1. Schalten Sie zur Listenansicht um, die Sie zur Verkaufsverbindung pushen möchten, und klicken Sie neben der Schaltfläche Los .
1. Klicks **Los**.
1. Wählen Sie alle Leads/Kontakte aus, an die Sie gepusht werden möchten.
1. Auswählen **Push to MSE**.
1. Es wird ein neues Fenster angezeigt, in dem die Anzahl der Leads/Kontakte überprüft wird, über die Sie pushen möchten. Auswählen **Zu Gruppe wechseln**. Sales Connect überträgt keine Kontakte, die als E-Mail-Abmeldung in Salesforce oder Abmeldung in Sales Connect gekennzeichnet sind.

   >[!NOTE]
   >
   >Sales Connect fügt diese Gruppe mit dem Titel &quot;SFDC-..&quot;zur Seite Beziehungen auf der Seite hinzu. [Webanwendung](https://toutapp.com/login).

1. Auswählen **Gesamte E-Mail-Gruppe** um diese Gruppen-E-Mail zu versenden.
