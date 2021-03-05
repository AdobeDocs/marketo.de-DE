---
unique-page-id: 14746177
description: Neuabonnieren und Abmelden - Marketing Docs - Produktdokumentation
title: Abonnement neu abonnieren
translation-type: tm+mt
source-git-commit: 1649aae540204bb5de205e3f5b75ec7e968a7da4
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---


# Neuabonnieren eines Abonnenten {#resubscribing-an-unsubscribe}

Manchmal wollen die Leute sich wieder für den Empfang von E-Mails entscheiden. Hier ist, wie man Abbestellungen wieder mailbar macht.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!CAUTION]
>
>Bevor Sie eine Person erneut abonnieren, sollten Sie nachweisen können, dass die Autorisierung, sie erneut zu abonnieren, dokumentiert ist und in Übereinstimmung mit allen anwendbaren Gesetzen steht.

>[!NOTE]
>
>Wenn Sie die Synchronisierung zum Abbestellen aktiviert haben, müssen Sie das Abbestellen von ToutApp entfernen und die Opt-out in Salesforce deaktivieren, damit der persönliche Datensatz nicht wieder synchronisiert wird.

1. Wechseln Sie zur Webanwendung [und klicken Sie auf **Personen**.](https://toutapp.com/login)

1. Wählen Sie die Person aus, um die Ansicht mit den Personendetails zu öffnen.

   ![](assets/two.png)

1. Klicken Sie auf die drei Punkte in der Ansicht mit den Personendetails und wählen Sie **Abmelden entfernen**.

   ![](assets/three.png)

1. Wählen Sie den Grund aus, warum die Person wieder für den Empfang von E-Mails ausgewählt wurde, und klicken Sie dann auf **Abmelden entfernen**.

   ![](assets/four.png)

>[!NOTE]
>
>Wenn Sie die Synchronisierung zum Abbestellen aktiviert haben, müssen Sie auch das Opt-out Feld im Datensatz in Salesforce deaktivieren, oder die nächtliche Synchronisierung wird die Person in Sales Connect erneut abmelden, da sie erkennt, dass die Person in Salesforce abgemeldet wurde. Wenn einer der Datensätze Opt-out/nicht abonniert wird, markiert die Synchronisierung den verknüpften Datensatz als solchen.
