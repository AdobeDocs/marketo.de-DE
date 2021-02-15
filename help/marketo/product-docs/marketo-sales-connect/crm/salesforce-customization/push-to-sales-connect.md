---
unique-page-id: 14352477
description: Push to Sales Connect - Marketing Docs - Produktdokumentation
title: An Sales Connect übertragen
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# An Sales Connect {#push-to-sales-connect} weiterleiten

Über unsere Schaltfläche &quot;Push to Tout&quot;erhalten Sie eine Liste Ihrer Kontakte/Kontakte in Salesforce und können diese in eine Gruppe in Sales Connect verschieben. Anschließend können Sie schnell eine benutzerspezifische Gruppen-E-Mail mit angehängter Tout-Verfolgung senden.

## Voraussetzungen {#requirements}

* Sales Connect Salesforce-Paket installiert von Salesforce Admin

* Schaltfläche &quot;An Sales Connect&quot;, die zur Ansicht durch Salesforce-Admin installiert wurde

* Salesforce-Verbindung mit Sales Connect für Benutzer, die Push erstellen

## Verfahren {#how-to}

1. Klicken Sie in Salesforce auf die Registerkarte **Lead/Kontakt**.
1. Schalten Sie zur Ansicht Liste um, die Sie zu Sales Connect verschieben möchten, neben der Schaltfläche Go.
1. Klicken Sie auf **Los**.
1. Wählen Sie alle Leads/Kontakte aus, die Sie herausziehen möchten.
1. Wählen Sie **In MSE** verschieben.
1. Es wird ein neues Fenster angezeigt, in dem die Anzahl der Kontakte/Kontakte überprüft wird, über die Sie weiterleiten möchten. Wählen Sie **Fahren Sie mit der Gruppe** fort. Sales Connect überträgt keine Kontakte, die als E-Mail-Opt-out in Salesforce oder Unsubscribed in Sales Connect gekennzeichnet sind.

   >[!NOTE]
   >
   >Sales Connect fügt diese Gruppe mit dem Titel &quot;SFDC-...&quot;hinzu. auf der Seite &quot;Beziehungen&quot;der [Webanwendung](https://toutapp.com/login).

1. Wählen Sie **E-Mail an die gesamte Gruppe**, um diese Gruppe per E-Mail zu versenden.
