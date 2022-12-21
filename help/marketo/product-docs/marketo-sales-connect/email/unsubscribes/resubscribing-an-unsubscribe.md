---
unique-page-id: 14746177
description: Zurücksetzen und Abmelden - Marketo Docs - Produktdokumentation
title: Abmeldung
exl-id: 1c451ff7-c56f-477e-b287-898c359aedcf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Abmeldung {#resubscribing-an-unsubscribe}

Manchmal möchten Benutzer sich wieder für den Erhalt von E-Mails entscheiden. Hier ist, wie man Abmeldungen wieder versendefähig macht.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!CAUTION]
>
>Bevor Sie eine Person erneut abonnieren, sollten Sie nachweisen können, dass die Genehmigung zur erneuten Anmeldung dokumentiert ist und allen geltenden Gesetzen entspricht.

>[!NOTE]
>
>Wenn Sie die Abmelde-Synchronisation aktiviert haben, müssen Sie die Abmeldung von ToutApp entfernen und die Abmeldung in Salesforce deaktivieren, damit der Personendatensatz nicht erneut synchronisiert wird.

1. Navigieren Sie zu [Webanwendung](https://toutapp.com/login) und klicken Sie auf **Personen**.

1. Wählen Sie die Person aus, um die Personendetailansicht zu öffnen.

   ![](assets/two.png)

1. Klicken Sie auf die drei Punkte in der Personendetailansicht und wählen Sie **Abmeldung entfernen**.

   ![](assets/three.png)

1. Wählen Sie den Grund aus, aus dem die Person sich für den Empfang von E-Mails entschieden hat, und klicken Sie auf **Abmeldung entfernen**.

   ![](assets/four.png)

>[!NOTE]
>
>Wenn Sie die Synchronisierung zum Abmelden aktiviert haben, müssen Sie auch das Opt-out-Feld im Datensatz in Salesforce deaktivieren. Andernfalls wird die Person in Sales Connect durch die nächtliche Synchronisierung erneut abgemeldet, da die Person in Salesforce abgewählt wird. Wenn einer der Datensätze abgemeldet/abgemeldet wird, markiert die Synchronisierung den verknüpften Datensatz als solchen.
