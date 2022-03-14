---
description: Wie behebe ich die Fehlermeldung "Wir konnten Ihre Anfrage nicht authentifizieren"bei der Verbindung mit Salesforce - Marketo Docs - Produktdokumentation
title: Wie behebe ich bei der Verbindung mit Salesforce die Fehlermeldung "Wir konnten Ihre Anfrage nicht authentifizieren"?
hide: true
hidefromtoc: true
source-git-commit: c398aff77e09f4a63db5d51af55178aa663ec98e
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# Wie behebe ich bei der Verbindung mit Salesforce die Fehlermeldung &quot;Wir konnten Ihre Anfrage nicht authentifizieren&quot;? {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Wenn Sie beim Versuch, Sales Insight-Aktionen mit Salesforce zu verbinden, die Fehlermeldung &quot;Wir konnten Ihre Anfrage nicht authentifizieren&quot;erhalten, kann es eine Einschränkung Ihres Zugriffs auf die Salesforce-API geben. Wenden Sie sich an Ihren Salesforce-Administrator, um sicherzustellen, dass die folgenden Elemente vorhanden sind.

## Aktivieren der API in Benutzerberechtigungen {#enable-api-in-user-permissions}

1. Bitten Sie einen Salesforce-Administrator, sich bei SFDC anzumelden.
1. Auswählen **Einrichtung**.
1. Auswählen **Benutzer verwalten**.
1. Auswählen **Profile**.
1. Suchen Sie das Profil, unter dem sich die ToutApp-Benutzer befinden, und klicken Sie auf **Bearbeiten**.
1. Scrollen Sie nach unten zu **Administratorberechtigungen** und stellen Sie sicher, dass **API aktiviert** aktiviert ist.

## Überprüfen Sie, ob Salesforce Sales Insight-Aktionen von der Verbindung blockiert {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Bitten Sie einen Salesforce-Administrator, sich bei SFDC anzumelden.
1. Auswählen **Einrichtung**.
1. Auswählen **Apps verwalten**.
1. Auswählen **Connected Apps OAuth-Nutzung**.
1. Stellen Sie sicher, dass Sales Insight-Aktionen daneben &quot;Block&quot;anzeigen. Wenn Sie &quot;Block aufheben&quot;sehen, klicken Sie auf die Schaltfläche, um den Zugriff von Sales Insight-Aktionen auf Salesforce zu entsperren.
