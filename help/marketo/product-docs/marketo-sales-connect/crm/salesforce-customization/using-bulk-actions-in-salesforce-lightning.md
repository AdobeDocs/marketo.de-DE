---
unique-page-id: 42762825
description: Verwenden von Massenaktionen in Salesforce-Blitzen - Marketo-Dokumente - Produktdokumentation
title: Verwenden von Massenaktionen in Salesforce-Blitzen
exl-id: 72022507-6568-4cc2-b3b5-c1703a1493ad
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 1%

---

# Verwenden von Massenaktionen in Salesforce-Blitzen {#using-bulk-actions-in-salesforce-lightning}

Erfahren Sie, wie Sie Massenaktionen durchführen, z. B. Leads zu einer Kampagne hinzufügen, eine Massen-E-Mail senden oder Leads von Salesforce an Sales Connect senden.

>[!PREREQUISITES]
>
>Aktualisieren Sie auf die neueste Version des Sales Connect-Packages und installieren Sie die Massen-Aktionsschaltflächen in Ihrer Lead-/Kontaktansicht. [Klicken Sie hier, um Anweisungen zu erhalten.](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)

>[!NOTE]
>
>Bevor Sie die folgenden Schritte ausführen, stellen Sie sicher, dass Sie bei Ihrem Marketo Sales Connect-Konto angemeldet sind.

## Bulk Email {#bulk-email}

1. Klicken Sie in Salesforce auf die Registerkarte **Leads** und wählen Sie dann die Liste der gewünschten Leads aus.

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >Wenn Sie sich bereits auf der Liste befinden, die Sie verwenden werden, müssen Sie sie erneut ausführen, indem Sie sie aus der Dropdown-Liste auswählen, um sicherzustellen, dass die MSC-Aktionsschaltflächen angezeigt werden. Dies ist das Salesforce-Verhalten, das nicht geändert werden kann.

1. Klicken Sie auf das Dropdown-Menü mit dem Pfeil (ganz rechts im Bildschirm) und wählen Sie **E-Mail mit MSC** aus.

   ![](assets/two-6.png)

1. Daraufhin wird eine MSC-E-Mail angezeigt. Es umfasst die folgenden Funktionen:

   a. Das Feld &quot;An&quot;zeigt &quot;Alle Quittungen&quot;- dies entspricht der Liste der Leads, die Sie in der Lead-Listenansicht ausgewählt haben\
   b. Diese Liste ist im linken Bedienfeld &quot;Bulk Composer&quot;sichtbar - Sie können hier Empfänger hinzufügen/entfernen\
   c. Sie können eine Vorlage auswählen oder eine eigene E-Mail erstellen.\
   d. Sie können die E-Mail sofort versenden oder einen späteren Versand planen

   ![](assets/three-5.png)

## Zur Kampagne hinzufügen {#add-to-campaign}

1. Klicken Sie in Salesforce auf die Registerkarte **Leads** und wählen Sie dann die Liste der gewünschten Leads aus.

   ![](assets/four-4.png)

1. Klicken Sie auf das Dropdown-Menü mit dem Pfeil (ganz rechts im Bildschirm) und wählen Sie **Zu MSC-Kampagne hinzufügen** aus.

   ![](assets/five-4.png)

1. Daraufhin wird das Popup &quot;Personen zu Ihrer Kampagne hinzufügen&quot;angezeigt. Klicken Sie auf **Weiter** und gehen Sie durch den typischen Kampagnenfluss, um eine MSC-Kampagne Trigger.

   ![](assets/six-1.png)

## In Marketo Sales Connect pushen {#push-to-marketo-sales-connect}

1. Klicken Sie in Salesforce auf die Registerkarte **Leads** und wählen Sie dann die Liste der gewünschten Leads aus.

   ![](assets/seven-2.png)

1. Klicken Sie auf das Dropdown-Menü mit dem Pfeil (ganz rechts auf dem Bildschirm) und wählen Sie **Push to MSC** aus.

   ![](assets/eight-2.png)

1. Eine neue Registerkarte mit dem Namen &quot;Salesforce Bridge&quot;wird geöffnet. Klicken Sie auf die Schaltfläche **Weiter zu Gruppe →** .

   ![](assets/nine-2.png)

1. Sie werden an Ihr MSC-Konto gesendet, wo eine mit Datums-/Uhrzeitstempel erstellte Gruppe angezeigt wird. Sie erhalten eine Benachrichtigung, sobald die Synchronisation abgeschlossen ist und die Gruppe die von Salesforce synchronisierten Leads enthält.

   ![](assets/ten-1.png)

>[!NOTE]
>
>Sie können dieselben Schritte ausführen, um auch Massenaktionen in der Kontaktlisten-Ansicht zu verwenden.

>[!MORELIKETHIS]
>
>* [Senden von E-Mails über Gruppen-E-Mails](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Erstellen von Massen-E-Mails mit Auswählen und Senden](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
