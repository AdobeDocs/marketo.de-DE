---
unique-page-id: 42762794
description: Verwenden von Massenaktionen in  [!DNL Salesforce]  Classic - Marketo-Dokumente - Produktdokumentation
title: Verwenden von Massenaktionen in  [!DNL Salesforce]  Classic
exl-id: f676ba65-6bc9-41e5-aa70-0f10bceedab7
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 2%

---

# Verwenden von Massenaktionen in [!DNL Salesforce] Classic {#using-bulk-actions-in-salesforce-classic}

Erfahren Sie, wie Sie Massenaktionen durchführen, z. B. Leads zu einer Kampagne hinzufügen, eine Massen-E-Mail senden oder Leads von [!DNL Salesforce] zu [!DNL Sales Connect] pushen.

>[!PREREQUISITES]
>
>Aktualisieren Sie auf die neueste Version des [!DNL Sales Connect]-Pakets und installieren Sie die Massenaktionsschaltflächen in Ihrer Lead-/Kontaktansicht. [Klicken Sie hier für Anweisungen](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Bevor Sie die beschriebenen Schritte ausführen, stellen Sie sicher, dass Sie bei Ihrem Marketo Sales Connect-Konto angemeldet sind.

## Bulk Email {#bulk-email}

1. Klicken Sie [!DNL Salesforce] auf die **[!UICONTROL Leads]** und dann auf die Schaltfläche **[!UICONTROL Los]**.

   ![](assets/one-5.png)

1. Wählen Sie die gewünschten Leads aus und klicken Sie auf die Schaltfläche **[!UICONTROL E-Mail mit MSC (Classic]**.

   ![](assets/two-5.png)

1. Eine MSC-E-Mail wird angezeigt. Es umfasst die folgenden Funktionen:

   a. Das Feld [!UICONTROL An] zeigt &quot;[!UICONTROL Alle Empfänger]&quot; an. Dies entspricht der Liste der Leads, die Sie in der Lead-Listenansicht ausgewählt haben
b. Diese Liste ist im linken Bereich namens &quot;[!UICONTROL Bulk Compose] sichtbar - Sie können hier Empfänger hinzufügen/entfernen
c. Sie können eine Vorlage auswählen oder Ihre eigene E-Mail erstellen
d. Sie können eine Vorschau der dynamischen Felder anzeigen, die in Ihrer E-Mail ausgefüllt werden
e. Sie können die E-Mail sofort senden oder einen Zeitplan für den Versand zu einem späteren Zeitpunkt festlegen

   ![](assets/three-4.png)

## Zur Kampagne hinzufügen {#add-to-campaign}

1. Klicken Sie [!DNL Salesforce] auf die **[!UICONTROL Leads]** und dann auf die Schaltfläche **[!UICONTROL Los]**.

   ![](assets/four-3.png)

1. Wählen Sie die gewünschten Leads aus und klicken Sie auf die Schaltfläche **[!UICONTROL Zu MSC-Kampagne hinzufügen (Classic]**.

   ![](assets/five-3.png)

1. Ein Popup [!UICONTROL Personen zu Ihrer Kampagne hinzufügen] wird angezeigt. Klicken Sie **[!UICONTROL Weiter]** und gehen Sie durch den typischen Kampagnenfluss, um eine MSC-Kampagne Trigger.

   ![](assets/six.png)

## In Marketo Sales Connect pushen {#push-to-marketo-sales-connect}

1. Klicken Sie [!DNL Salesforce] auf die **[!UICONTROL Leads]** und dann auf die Schaltfläche **[!UICONTROL Los]**.

   ![](assets/seven-1.png)

1. Wählen Sie die gewünschten Leads aus und klicken Sie auf die Schaltfläche **[!UICONTROL Push to MSC (Classic]**.

   ![](assets/eight-1.png)

1. Eine neue Registerkarte mit dem Namen &quot;[!UICONTROL Salesforce Bridge]&quot; wird geöffnet. Klicken Sie auf **[!UICONTROL Schaltfläche „Mit → fortfahren]**.

   ![](assets/nine-1.png)

1. Sie werden an Ihr MSC-Konto gesendet, wo eine Gruppe mit Datum/Zeitstempel erstellt wird. Sie erhalten eine Benachrichtigung, sobald die Synchronisierung abgeschlossen ist und die Gruppe die aus [!DNL Salesforce] synchronisierten Leads enthält.

   ![](assets/ten.png)

>[!NOTE]
>
>Sie können dieselben Schritte ausführen, um Massenaktionen auch in der Kontaktlistenansicht zu verwenden.

>[!MORELIKETHIS]
>
>* [Senden von E-Mails über Gruppen-E-Mails](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Erstellen von Massen-E-Mails mit Auswählen und Senden](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
