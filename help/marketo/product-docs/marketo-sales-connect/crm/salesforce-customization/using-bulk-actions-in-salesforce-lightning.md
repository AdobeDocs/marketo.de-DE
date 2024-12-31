---
unique-page-id: 42762825
description: Verwenden von Massenaktionen in Salesforce Lightning - Marketo-Dokumente - Produktdokumentation
title: Verwenden von Massenaktionen in Salesforce Lightning
exl-id: 72022507-6568-4cc2-b3b5-c1703a1493ad
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 1%

---

# Verwenden von Massenaktionen in Salesforce Lightning {#using-bulk-actions-in-salesforce-lightning}

Erfahren Sie, wie Sie Massenaktionen durchführen, z. B. Leads zu einer Kampagne hinzufügen, eine Massen-E-Mail senden oder Leads von Salesforce an Sales Connect pushen.

>[!PREREQUISITES]
>
>Aktualisieren Sie auf die neueste Version des Sales Connect-Pakets und installieren Sie die Massenaktionsschaltflächen in Ihrer Lead-/Kontaktansicht. [Klicken Sie hier für Anweisungen](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf).

>[!NOTE]
>
>Bevor Sie die folgenden Schritte ausführen, stellen Sie sicher, dass Sie bei Ihrem Marketo Sales Connect-Konto angemeldet sind.

## Bulk Email {#bulk-email}

1. Klicken Sie in Salesforce auf **Leads** und wählen Sie dann die Liste der gewünschten Leads aus.

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >Wenn Sie sich bereits in der Liste befinden, die Sie verwenden werden, müssen Sie sie erneut ausführen, indem Sie sie aus der Dropdown-Liste auswählen, um sicherzustellen, dass die MSC-Massenaktionsschaltflächen angezeigt werden. Dies ist das Verhalten von Salesforce, das nicht geändert werden kann.

1. Klicken Sie auf den Pfeil der Dropdown-Liste (ganz rechts auf dem Bildschirm) und wählen Sie **E-Mail mit MSC**.

   ![](assets/two-6.png)

1. Eine MSC-E-Mail wird angezeigt. Es umfasst die folgenden Funktionen:

   a. Das Feld „An“ zeigt „Alle Wareneingänge“ an. Dies entspricht der Liste der Leads, die Sie in der Lead-Listenansicht ausgewählt haben\
   b. Diese Liste ist im linken Bereich namens „Massenverarbeitung“ sichtbar - Sie können hier Empfänger hinzufügen/entfernen\
   c. Sie können eine Vorlage auswählen oder Ihre eigene E-Mail erstellen\
   d. Sie können die E-Mail sofort senden oder einen Zeitplan festlegen, um sie zu einem späteren Zeitpunkt zu senden

   ![](assets/three-5.png)

## Zur Kampagne hinzufügen {#add-to-campaign}

1. Klicken Sie in Salesforce auf **Leads** und wählen Sie dann die Liste der gewünschten Leads aus.

   ![](assets/four-4.png)

1. Klicken Sie auf den Pfeil der Dropdown-Liste (ganz rechts im Bildschirm) und wählen Sie **Zu MSC-Kampagne hinzufügen**.

   ![](assets/five-4.png)

1. Ein Popup-Fenster „Personen zu Ihrer Kampagne hinzufügen“ wird angezeigt. Klicken Sie **Weiter** und gehen Sie durch den typischen Kampagnenfluss, um eine MSC-Kampagne Trigger.

   ![](assets/six-1.png)

## In Marketo Sales Connect pushen {#push-to-marketo-sales-connect}

1. Klicken Sie in Salesforce auf **Leads** und wählen Sie dann die Liste der gewünschten Leads aus.

   ![](assets/seven-2.png)

1. Klicken Sie auf den Pfeil der Dropdown-Liste (ganz rechts auf dem Bildschirm) und wählen Sie **Push to MSC**.

   ![](assets/eight-2.png)

1. Eine neue Registerkarte mit dem Namen &quot;Salesforce Bridge&quot; wird geöffnet. Klicken Sie auf **Schaltfläche „Mit → fortfahren**.

   ![](assets/nine-2.png)

1. Sie werden an Ihr MSC-Konto gesendet, wo eine Gruppe mit Datum/Zeitstempel erstellt wird. Sie erhalten eine Benachrichtigung, sobald die Synchronisierung abgeschlossen ist und die Gruppe die aus Salesforce synchronisierten Leads enthält.

   ![](assets/ten-1.png)

>[!NOTE]
>
>Sie können dieselben Schritte ausführen, um Massenaktionen auch in der Kontaktlistenansicht zu verwenden.

>[!MORELIKETHIS]
>
>* [Senden von E-Mails über Gruppen-E-Mails](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Erstellen von Massen-E-Mails mit Auswählen und Senden](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)
