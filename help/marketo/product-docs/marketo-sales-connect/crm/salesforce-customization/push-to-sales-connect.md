---
unique-page-id: 14352477
description: 'Push- [!DNL Sales Connect] : Marketo-Dokumente - Produktdokumentation'
title: Push an [!DNL Sales Connect]
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Push an [!DNL Sales Connect] {#push-to-sales-connect}

Unser [!UICONTROL Push to Tout] Button wird eine Liste Ihrer Leads/Kontakte in [!DNL Salesforce] nehmen und sie in eine Gruppe in [!DNL Sales Connect] schieben. Sie können dann schnell eine anpassbare Gruppen-E-Mail mit angehängtem Tout-Tracking senden.

## Anforderungen {#requirements}

* Von [!DNL Sales Connect Salesforce] Admin installiertes [!DNL Salesforce]

* Schaltfläche [!UICONTROL Push to Sales Connect] von [!DNL Salesforce] Administrator zur Listenansicht installiert

* [!DNL Salesforce] Verbindung mit [!DNL Sales Connect] für Benutzer, die die Push-Benachrichtigung durchführen

## Anleitung {#how-to}

1. Klicken Sie in **[!UICONTROL auf]** Lead/Kontakt[!DNL Salesforce].
1. Schalten Sie zur Listenansicht um, die Sie auf [!DNL Sales Connect] neben der Schaltfläche [!UICONTROL Los“ &#x200B;] möchten.
1. Klicken Sie **[!UICONTROL Los]**.
1. Wählen Sie alle Leads/Kontakte aus, an die Sie gepusht werden möchten.
1. Wählen Sie **[!UICONTROL Push an MSE]** aus.
1. Es wird ein neues Fenster angezeigt, in dem die Anzahl der Leads/Kontakte überprüft wird, die übertragen werden sollen. Wählen Sie **[!UICONTROL Mit Gruppe fortfahren]** aus.[!DNL Sales Connect] überträgt keine Kontakte, die als [!UICONTROL E-Mail-Opt-out] in [!DNL Salesforce] oder [!UICONTROL Abgemeldet] in [!DNL Sales Connect] gekennzeichnet sind.

   >[!NOTE]
   >
   >[!DNL Sales Connect] fügt diese Gruppe mit dem Titel &quot;SFDC-…“ zur Seite „Beziehungen“ in der [Web-Anwendung“ &#x200B;](https://toutapp.com/login).

1. Wählen Sie **[!UICONTROL E-Mail an gesamte]** senden, um diese Gruppen-E-Mail zu senden.
