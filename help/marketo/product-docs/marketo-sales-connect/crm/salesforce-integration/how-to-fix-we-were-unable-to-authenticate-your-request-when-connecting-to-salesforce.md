---
unique-page-id: 14352484
description: Hier erhalten Sie Hilfe zur Behebung des Fehlers „Wir konnten Ihre Anfrage nicht authentifizieren“ beim Verbinden von Sales Connect mit Salesforce. Fehlerbehebung bei Authentifizierungsproblemen.
title: Wie sich der Fehler „Wir konnten Ihre Anfrage nicht authentifizieren“ beheben lässt, wenn eine Verbindung zu Salesforce hergestellt werden soll
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/51pd-hGwspmp6ZuOShb3z3wRdQ0PZ-pCIY-BeV4Q5ho
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 175
ht-degree: 8%

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
