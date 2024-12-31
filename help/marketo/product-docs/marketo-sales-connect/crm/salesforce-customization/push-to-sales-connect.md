---
unique-page-id: 14352477
description: Push an Sales Connect - Marketo-Dokumente - Produktdokumentation
title: Push an Sales Connect
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---

# Push an Sales Connect {#push-to-sales-connect}

Über die Schaltfläche „Push to Tout“ wird eine Liste Ihrer Leads/Kontakte in Salesforce erstellt und in eine Gruppe in Sales Connect verschoben. Sie können dann schnell eine anpassbare Gruppen-E-Mail mit angehängtem Tout-Tracking senden.

## Anforderungen {#requirements}

* Vom Salesforce-Administrator installiertes Sales Connect Salesforce-Paket

* Schaltfläche „Push an Sales Connect“ von Salesforce-Administrator in Listenansicht installiert

* Salesforce-Verbindung mit Sales Connect für Anwender, die Push-Benachrichtigungen senden

## Anleitung {#how-to}

1. Salesforce Klicken Sie in **auf die Registerkarte** Lead/Kontakt“.
1. Schalten Sie neben der Schaltfläche Los in die Listenansicht um, die Sie an Sales Connect pushen möchten.
1. Klicken Sie **Los**.
1. Wählen Sie alle Leads/Kontakte aus, an die Sie gepusht werden möchten.
1. Wählen Sie **Push an MSE** aus.
1. Es wird ein neues Fenster angezeigt, in dem die Anzahl der Leads/Kontakte überprüft wird, die übertragen werden sollen. Wählen Sie **Mit Gruppe fortfahren** aus. Sales Connect überträgt keine Kontakte, die in Salesforce als E-Mail-Opt-out markiert oder in Sales Connect abgemeldet wurden.

   >[!NOTE]
   >
   >Sales Connect fügt diese Gruppe mit dem Titel &quot;SFDC-…“ zur Seite „Beziehungen“ in der [Web-Anwendung“ ](https://toutapp.com/login).

1. Wählen Sie **E-Mail an gesamte** senden, um diese Gruppen-E-Mail zu senden.
