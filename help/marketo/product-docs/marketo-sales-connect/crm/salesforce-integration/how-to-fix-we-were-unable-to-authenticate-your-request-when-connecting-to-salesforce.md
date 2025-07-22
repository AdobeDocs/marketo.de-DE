---
unique-page-id: 14352484
description: Fehlerbehebung „Wir konnten Ihre Anfrage nicht authentifizieren“ beim Herstellen einer Verbindung zu Salesforce - Marketo-Dokumente - Produktdokumentation
title: Wie zu beheben ist „Wir konnten Ihre Anfrage nicht authentifizieren“, wenn eine Verbindung zu Salesforce hergestellt wurde
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Wie zu beheben „Wir konnten Ihre Anfrage nicht authentifizieren“, wenn eine Verbindung zu [!DNL Salesforce] hergestellt wurde {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Wenn Sie beim Versuch, eine Verbindung zwischen [!DNL Sales Connect] und [!DNL Salesforce] herzustellen, die Fehlermeldung „Wir konnten Ihre Anfrage nicht authentifizieren“ erhalten, kann Ihr Zugriff auf die API von [!DNL Salesforce] eingeschränkt sein. Wenden Sie sich an Ihren [!DNL Salesforce], um sicherzustellen, dass die folgenden Voraussetzungen erfüllt sind.

## Aktivieren der API in Benutzerberechtigungen {#enable-api-in-user-permissions}

1. Bitten Sie einen [!DNL Salesforce] Administrator, sich bei SFDC anzumelden.
1. Wählen Sie **[!UICONTROL Setup]** aus.
1. Wählen Sie **[!UICONTROL Benutzer verwalten]** aus.
1. Wählen Sie **[!UICONTROL Profile]** aus.
1. Suchen Sie das Profil, unter dem sich die ToutApp-Benutzer befinden, und klicken Sie auf **[!UICONTROL Bearbeiten]**.
1. Scrollen Sie nach unten **[!UICONTROL Administratorberechtigungen]** und stellen Sie sicher, dass **[!UICONTROL API aktiviert]** aktiviert ist.

## Überprüfen, ob [!DNL Salesforce] [!DNL Sales Connect] am Herstellen einer Verbindung hindert {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Bitten Sie einen [!DNL Salesforce] Administrator, sich bei SFDC anzumelden.
1. Wählen Sie **[!UICONTROL Setup]** aus.
1. Wählen Sie **[!UICONTROL Apps verwalten]** aus.
1. Wählen Sie **[!UICONTROL Connected Apps OAuth Usage]** aus.
1. Stellen Sie sicher, dass [!DNL Sales Connect] &quot;[!UICONTROL Block]&quot; daneben anzeigt. Wenn Sie &quot;[!UICONTROL Unblock]&quot; sehen, klicken Sie auf die Schaltfläche, um [!DNL Sales Connect] Zugriff auf [!DNL Salesforce] zu entsperren.
