---
unique-page-id: 14352484
description: Fehlerbehebung „Wir konnten Ihre Anfrage nicht authentifizieren“ beim Herstellen einer Verbindung zu Salesforce - Marketo-Dokumente - Produktdokumentation
title: Wie zu beheben ist „Wir konnten Ihre Anfrage nicht authentifizieren“, wenn eine Verbindung zu Salesforce hergestellt wurde
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# Wie zu beheben ist „Wir konnten Ihre Anfrage nicht authentifizieren“, wenn eine Verbindung zu Salesforce hergestellt wurde {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Wenn Sie beim Versuch, eine Verbindung zwischen Sales Connect und Salesforce herzustellen, die Fehlermeldung „Wir konnten Ihre Anfrage nicht authentifizieren“ erhalten, kann dies zu einer Einschränkung Ihres Zugriffs auf die Salesforce-API führen. Wenden Sie sich an Ihren Salesforce-Administrator, um sicherzustellen, dass die folgenden Voraussetzungen erfüllt sind.

## Aktivieren der API in Benutzerberechtigungen {#enable-api-in-user-permissions}

1. Bitten Sie einen Salesforce-Administrator, sich bei SFDC anzumelden.
1. Wählen Sie **Setup** aus.
1. Wählen Sie **Benutzer verwalten** aus.
1. Wählen Sie **Profile** aus.
1. Suchen Sie das Profil, unter dem sich die ToutApp-Benutzer befinden, und klicken Sie auf **Bearbeiten**.
1. Scrollen Sie nach unten **Administratorberechtigungen** und stellen Sie sicher, dass **API aktiviert** aktiviert ist.

## Überprüfen, ob Salesforce Sales Connect daran hindert, eine Verbindung herzustellen {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Bitten Sie einen Salesforce-Administrator, sich bei SFDC anzumelden.
1. Wählen Sie **Setup** aus.
1. Wählen Sie **Apps verwalten** aus.
1. Wählen Sie **Connected Apps OAuth Usage** aus.
1. Stellen Sie sicher, dass Sales Connect „Block“ daneben anzeigt. Wenn Sie „Blockierung aufheben“ sehen, klicken Sie auf die Schaltfläche, um den Zugriff von Sales Connect auf Salesforce aufzuheben.
