---
unique-page-id: 14352484
description: Fehlerbehebung "Wir konnten Ihre Anforderung nicht authentifizieren" bei der Verbindung mit Salesforce - Marketing Docs - Produktdokumentation
title: Fehlerbehebung "Wir konnten Ihre Anforderung nicht authentifizieren" beim Herstellen einer Verbindung mit Salesforce
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Fehlerbehebung &quot;Wir konnten Ihre Anforderung nicht authentifizieren&quot; beim Herstellen einer Verbindung mit Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Wenn Sie beim Versuch, Sales Connect mit Salesforce zu verbinden, die Fehlermeldung &quot;Wir konnten Ihre Anforderung nicht authentifizieren&quot;erhalten haben, gibt es möglicherweise Einschränkungen beim Zugriff auf die Salesforce-API. Wenden Sie sich an Ihren Salesforce-Administrator, um sicherzustellen, dass folgende Elemente vorhanden sind:

## Aktivieren der API in Benutzerberechtigungen {#enable-api-in-user-permissions}

1. Nehmen Sie einen Salesforce-Admin-Login bei SFDC vor.
1. Wählen Sie **Setup**.
1. Wählen Sie **Benutzer verwalten**.
1. Wählen Sie **Profil**.
1. Suchen Sie das Profil, unter dem sich die ToutApp-Benutzer befinden, und klicken Sie auf **Bearbeiten**.
1. Blättern Sie nach unten zu **Administrative Permissions** und stellen Sie sicher, dass **API Enabled** aktiviert ist.

## Überprüfen Sie, ob Salesforce Sales Connect von der Verbindung {#check-if-salesforce-is-blocking-sales-connect-from-connecting} blockiert.

1. Salesforce-Admin-Anmeldung bei SFDC.
1. Wählen Sie **Setup**.
1. Wählen Sie **Apps verwalten**.
1. Wählen Sie **Connected Apps OAuth Usage**.
1. Stellen Sie sicher, dass Sales Connect &quot;Block&quot;daneben anzeigt. Wenn Sie &quot;Block aufheben&quot;sehen, klicken Sie auf die Schaltfläche, um die Sperrung des Zugriffs von Sales Connect auf Salesforce aufzuheben.

