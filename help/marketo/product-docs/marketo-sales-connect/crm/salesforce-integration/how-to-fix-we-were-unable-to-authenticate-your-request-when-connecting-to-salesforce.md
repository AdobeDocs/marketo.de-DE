---
unique-page-id: 14352484
description: Fehlerbehebung "Wir konnten Ihre Anfrage nicht authentifizieren"bei der Verbindung mit Salesforce - Marketo Docs - Produktdokumentation
title: Fehlerbehebung "Wir konnten Ihre Anfrage nicht authentifizieren"bei der Verbindung mit Salesforce
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# Fehlerbehebung &quot;Wir konnten Ihre Anfrage nicht authentifizieren&quot;bei der Verbindung mit Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Wenn Sie beim Versuch, Sales Connect mit Salesforce zu verbinden, die Fehlermeldung &quot;Wir konnten Ihre Anfrage nicht authentifizieren&quot;erhalten, kann es eine Einschränkung Ihres Zugriffs auf die Salesforce-API geben. Wenden Sie sich an Ihren Salesforce-Administrator, um sicherzustellen, dass die folgenden Elemente vorhanden sind.

## Aktivieren der API in Benutzerberechtigungen {#enable-api-in-user-permissions}

1. Bitten Sie einen Salesforce-Administrator, sich bei SFDC anzumelden.
1. Auswählen **Einrichtung**.
1. Auswählen **Benutzer verwalten**.
1. Auswählen **Profile**.
1. Suchen Sie das Profil, unter dem sich die ToutApp-Benutzer befinden, und klicken Sie auf **Bearbeiten**.
1. Nach unten scrollen zu **Administratorberechtigungen** und stellen Sie sicher, **API aktiviert** aktiviert ist.

## Überprüfen Sie, ob Salesforce die Verbindung von Sales Connect blockiert. {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Bitten Sie einen Salesforce-Administrator, sich bei SFDC anzumelden.
1. Auswählen **Einrichtung**.
1. Auswählen **Apps verwalten**.
1. Auswählen **Connected Apps OAuth-Nutzung**.
1. Stellen Sie sicher, dass neben Sales Connect &quot;Block&quot;angezeigt wird. Wenn &quot;Block aufheben&quot;angezeigt wird, klicken Sie auf die Schaltfläche , um den Zugriff von Sales Connect auf Salesforce zu entsperren.
