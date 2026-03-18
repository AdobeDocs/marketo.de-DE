---
unique-page-id: 14746177
description: Erfahren Sie, wie Sie einen Kontakt, der sich in Sales Connect abgemeldet hat, erneut abonnieren können. Stellen Sie bei Bedarf die Möglichkeit zum Empfang von Verkaufs-E-Mails wieder her.
title: Erneutes Abonnieren nach einer Abmeldung
exl-id: 1c451ff7-c56f-477e-b287-898c359aedcf
feature: Marketo Sales Connect
source-git-commit: 15427eacd2fc42a02f6a4c59d9102bacba02e57b
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 2%

---

# Erneutes Abonnieren eines [!UICONTROL Abmelden] {#resubscribing-an-unsubscribe}

Manchmal möchten Personen den Erhalt von E-Mails rückgängig machen. Hier ist, wie man Abmeldungen wieder als E-Mail nutzbar macht.

>[!NOTE]
>
>**Admin-Berechtigungen erforderlich**

>[!CAUTION]
>
>Bevor Sie eine Person erneut anmelden, sollten Sie nachweisen können, dass die Autorisierung zum erneuten Abonnieren dokumentiert ist und alle geltenden Gesetze einhält.

>[!NOTE]
>
>Wenn Sie die Abmeldesynchronisierung aktiviert haben, müssen Sie die Abmeldung von ToutApp entfernen und die Option Abmelden in deaktivieren, [!DNL Salesforce] der Personendatensatz nicht erneut synchronisiert werden kann.

1. Wechseln Sie zur [Web-Anwendung](https://toutapp.com/login) und klicken Sie auf **[!UICONTROL Personen]**.

1. Wählen Sie die Person aus, um die Ansicht „Personendetails“ zu öffnen.

   ![](assets/two.png)

1. Klicken Sie auf die drei Punkte in der Ansicht „Personendetails“ und wählen Sie **[!UICONTROL Abmelden entfernen]**.

   ![](assets/three.png)

1. Wählen Sie den Grund aus, aus dem die Person für den Empfang von E-Mails wieder angemeldet wird, und klicken Sie dann auf **[!UICONTROL Abmelden entfernen]**.

   ![](assets/four.png)

>[!NOTE]
>
>Wenn Sie die Abmeldesynchronisierung aktiviert haben, müssen Sie auch das Kontrollkästchen zum Abmelden für den Datensatz in Salesforce deaktivieren. Andernfalls wird die Person in [!DNL Sales Connect] durch die nächtliche Synchronisierung erneut abgemeldet, da so erkannt wird, dass die Person in [!DNL Salesforce] abgemeldet wurde. Wenn einer der Datensätze abgemeldet/abgemeldet wird, markiert die Synchronisierung den verknüpften Datensatz als solchen.
