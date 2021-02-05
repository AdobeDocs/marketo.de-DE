---
unique-page-id: 42762825
description: Verwendung von Massenaktionen in Salesforce Lightning - Marketing Docs - Produktdokumentation
title: Verwenden von Massenaktionen im Salesforce-Blitz
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---


# Verwenden von Massenaktionen in Salesforce-Blitzen {#using-bulk-actions-in-salesforce-lightning}

Erfahren Sie, wie Sie Massenaktionen durchführen, z. B. Interessenten zu einer Kampagne hinzufügen, eine Massen-E-Mail versenden oder Interessenten von Salesforce zu Sales Connect verschieben.

>[!PREREQUISITES]
>
>Aktualisieren Sie auf die neueste Version des Sales Connect-Pakets und installieren Sie die Schaltflächen für Massenaktionen in Ihrer Ansicht für Lead/Kontakt. [Klicken Sie hier für Anleitungen](http://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf).

>[!NOTE]
>
>Bevor Sie die unten stehenden Schritte ausführen, stellen Sie sicher, dass Sie bei Ihrem Marketingto Sales Connect-Konto angemeldet sind.

## Bulk Email {#bulk-email}

1. Klicken Sie in Salesforce auf die Registerkarte **Interessenten** und wählen Sie dann die Liste der gewünschten Interessenten aus.

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >Wenn Sie bereits auf der Liste sind, die Sie verwenden werden, müssen Sie sie erneut ausführen, indem Sie sie aus der Dropdownliste auswählen, um sicherzustellen, dass die MSC-MSC-MSC-Massen-Aktionsschaltflächen angezeigt werden. Das ist Salesforce-Verhalten, das nicht geändert werden kann.

1. Klicken Sie auf die Dropdownliste mit dem Pfeil (ganz rechts auf dem Bildschirm) und wählen Sie **E-Mail mit MSC**.

   ![](assets/two-6.png)

1. Es erscheint eine MSC-E-Mail. Es umfasst die folgenden Funktionen:

   a. &quot;An&quot;-Feld zeigt &quot;Alle Einnahmen&quot;- dies entspricht der Liste der Interessenten, die Sie in der Ansicht &quot;Interessentenanwerbung&quot;ausgewählt haben\
   b. Diese Liste ist im linken Fensterbereich &quot;Massenzusammenstellung&quot;sichtbar - hier können Sie Empfänger hinzufügen/entfernen\
   c. Sie können eine Vorlage auswählen oder eine eigene E-Mail erstellen\
   d. Sie können die E-Mail sofort senden oder planen, sie zu einem späteren Zeitpunkt zu senden

   ![](assets/three-5.png)

## hinzufügen in Kampagne {#add-to-campaign}

1. Klicken Sie in Salesforce auf die Registerkarte **Interessenten** und wählen Sie dann die Liste der gewünschten Interessenten aus.

   ![](assets/four-4.png)

1. Klicken Sie auf das Dropdownmenü mit dem Pfeil (ganz rechts auf dem Bildschirm) und wählen Sie **Hinzufügen auf MSC-Kampagne**.

   ![](assets/five-4.png)

1. Es wird ein Popup &quot;Hinzufügen Personen zu Ihrer Kampagne&quot;angezeigt. Klicken Sie auf **Weiter** und gehen Sie durch den typischen Fluss der Kampagne, um eine MSC-Kampagne zu Trigger zu machen.

   ![](assets/six-1.png)

## Push to Marketing Sales Connect {#push-to-marketo-sales-connect}

1. Klicken Sie in Salesforce auf die Registerkarte **Interessenten** und wählen Sie dann die Liste der gewünschten Interessenten aus.

   ![](assets/seven-2.png)

1. Klicken Sie auf die Dropdownliste mit dem Pfeil (ganz rechts auf dem Bildschirm) und wählen Sie **Nach MSC** verschieben.

   ![](assets/eight-2.png)

1. Eine neue Registerkarte namens &quot;Salesforce Bridge&quot;wird geöffnet. Klicken Sie auf die Schaltfläche **Fahren Sie mit Gruppe →** fort.

   ![](assets/nine-2.png)

1. Sie werden an Ihr MSC-Konto gesendet, wo eine mit Datum-/Zeitstempel erstellte Gruppe angezeigt wird. Sie erhalten eine Benachrichtigung, sobald die Synchronisierung abgeschlossen ist und die Gruppe die von Salesforce synchronisierten Interessenten enthält.

   ![](assets/ten-1.png)

>[!NOTE]
>
>Sie können die gleichen Schritte ausführen, um Massenaktionen auch in der Ansicht Liste Kontakt zu verwenden.

>[!MORELIKETHIS]
>
>* [Senden von E-Mails per E-Mail](http://docs.marketo.com/x/KAQ6Ag)
>* [Erstellen von Massen-E-Mails mit &quot;Auswählen&quot;und &quot;Senden&quot;](http://docs.marketo.com/display/public/DOCS/Composing+Bulk+Emails+with+Select+and+Send#ComposingBulkEmailswithSelectandSend-SendingEmails)

>



