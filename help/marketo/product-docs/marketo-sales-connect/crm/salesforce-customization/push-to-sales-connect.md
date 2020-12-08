---
unique-page-id: 14352477
description: Push to Sales Connect - Marketing Docs - Produktdokumentation
title: An Sales Connect übertragen
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# An Sales Connect übertragen {#push-to-sales-connect}

Über unsere Schaltfläche &quot;Push to Tout&quot;erhalten Sie eine Liste Ihrer Kontakte/Kontakte in Salesforce und können diese in eine Gruppe in Sales Connect verschieben. Anschließend können Sie schnell eine benutzerspezifische Gruppen-E-Mail mit angehängter Tout-Verfolgung senden.

## Anforderungen {#requirements}

* Sales Connect [Salesforce-Paket](http://docs.marketo.com/x/C4PS) installiert von `Salesforce Admin`

* `Push to Sales Connect`Schaltfläche, die in der Ansicht der Liste durch `Salesforce Admin`

* Salesforce-Verbindung mit Sales Connect für Benutzer, die Push erstellen

## Verfahren {#how-to}

1. Klicken Sie in Salesforce auf die Registerkarte **Lead/Kontakt** .
1. Schalten Sie zur Ansicht Liste um, die Sie zu Sales Connect verschieben möchten, neben der Schaltfläche Go.
1. Klicken Sie auf **Los**.
1. Wählen Sie alle Leads/Kontakte aus, die Sie herausziehen möchten.
1. Wählen Sie **In MSE** pushen.
1. Es wird ein neues Fenster angezeigt, in dem die Anzahl der Kontakte/Kontakte überprüft wird, über die Sie weiterleiten möchten. Wählen Sie **Zur Gruppe** fortfahren. Sales Connect `will not push over` alle Kontakte, die als `Email Opt Out` Salesforce oder `Unsubscribed` in Sales Connect markiert sind.

   >[!NOTE]
   >
   >Sales Connect fügt diese Gruppe mit dem Titel &quot;SFDC-...&quot;hinzu. auf der Seite &quot;Beziehungen&quot;der [Webanwendung](http://toutapp.com/login).

1. Wählen Sie **Gesamte Gruppe** per E-Mail senden, um diese Gruppe-E-Mail zu senden.

