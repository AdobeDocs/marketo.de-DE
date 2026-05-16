---
unique-page-id: 14352477
description: Erfahren Sie, wie Sie die Schaltfläche Push-Benachrichtigung für Vertriebsverbindung in Salesforce verwenden. Leads oder Kontakte aus Salesforce zu Sales Connect mit einem Klick hinzufügen.
title: Push an [!DNL Sales Connect]
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/piy3bPtiO48FQhWEmpu5qo4denlJ8v1ZU-VXBlWh0Mg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 190
ht-degree: 0%

---

# Push an [!DNL Sales Connect] {#push-to-sales-connect}

Unser [!UICONTROL Push to Tout] Button wird eine Liste Ihrer Leads/Kontakte in [!DNL Salesforce] nehmen und sie in eine Gruppe in [!DNL Sales Connect] schieben. Sie können dann schnell eine anpassbare Gruppen-E-Mail mit angehängtem Tout-Tracking senden.

## Anforderungen {#requirements}

* Von [!DNL Salesforce] Admin installiertes [!DNL Sales Connect Salesforce]

* Schaltfläche [!UICONTROL Push to Sales Connect] von [!DNL Salesforce] Administrator zur Listenansicht installiert

* [!DNL Salesforce] Verbindung mit [!DNL Sales Connect] für Benutzer, die die Push-Benachrichtigung durchführen

## Anleitung {#how-to}

1. Klicken Sie in [!DNL Salesforce] auf **[!UICONTROL Lead/Kontakt]**.
1. Schalten Sie zur Listenansicht um, die Sie auf [!DNL Sales Connect] neben der Schaltfläche [!UICONTROL Los“ &#x200B;] möchten.
1. Klicken Sie **[!UICONTROL Los]**.
1. Wählen Sie alle Leads/Kontakte aus, an die Sie gepusht werden möchten.
1. Wählen Sie **[!UICONTROL Push an MSE]** aus.
1. Es wird ein neues Fenster angezeigt, in dem die Anzahl der Leads/Kontakte überprüft wird, die übertragen werden sollen. Wählen Sie **[!UICONTROL Mit Gruppe fortfahren]**.[!DNL Sales Connect] überträgt keine Kontakte, die als [!UICONTROL E-Mail-Opt-out] in [!DNL Salesforce] oder „Abgemeldet[!UICONTROL &#x200B; in [!DNL Sales Connect] &#x200B;] sind.

   >[!NOTE]
   >
   >[!DNL Sales Connect] fügen diese Gruppe mit dem Titel &quot;SFDC-…“ hinzu zur Seite „Beziehungen“ in der [Web-Anwendung](https://toutapp.com/login).

1. Wählen Sie **[!UICONTROL E-Mail an gesamte]** senden, um diese Gruppen-E-Mail zu senden.
