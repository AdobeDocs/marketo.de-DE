---
unique-page-id: 42762794
description: Massenaktionen in Salesforce Classic - Marketing Docs - Produktdokumentation
title: Massenaktionen in Salesforce Classic verwenden
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---


# Verwenden von Massenaktionen in Salesforce Classic {#using-bulk-actions-in-salesforce-classic}

Erfahren Sie, wie Sie Massenaktionen durchführen, z. B. Interessenten zu einer Kampagne hinzufügen, eine Massen-E-Mail versenden oder Interessenten von Salesforce zu Sales Connect verschieben.

>[!PREREQUISITES]
>
>Aktualisieren Sie auf die neueste Version des Sales Connect-Pakets und installieren Sie die Schaltflächen für Massenaktionen in Ihrer Ansicht für Lead/Kontakt. [Klicken Sie hier für Anleitungen](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Bevor Sie die beschriebenen Schritte ausführen, stellen Sie sicher, dass Sie bei Ihrem MarketingTo Sales Connect-Konto angemeldet sind.

## Bulk Email {#bulk-email}

1. Klicken Sie in Salesforce auf die Registerkarte **Interessenten** und dann auf die Schaltfläche **Los**.

   ![](assets/one-5.png)

1. Wählen Sie die gewünschten Interessenten aus und klicken Sie auf die Schaltfläche **E-Mail mit MSC (Classic)**.

   ![](assets/two-5.png)

1. Es erscheint eine MSC-E-Mail. Es umfasst die folgenden Funktionen:

   a. &quot;An&quot;-Feld zeigt &quot;Alle Einnahmen&quot;- dies entspricht der Liste der Interessenten, die Sie in der Ansicht &quot;Interessentenanwerbung&quot;ausgewählt haben\
   b. Diese Liste ist im linken Fensterbereich &quot;Massenzusammenstellung&quot;sichtbar - hier können Sie Empfänger hinzufügen/entfernen\
   c. Sie können eine Vorlage auswählen oder eine eigene E-Mail erstellen\
   d. Sie können dynamische Felder, die in Ihrer E-Mail ausgefüllt werden, Vorschau werden.\
   e. Sie können die E-Mail sofort senden oder planen, sie zu einem späteren Zeitpunkt zu senden

   ![](assets/three-4.png)

## hinzufügen in Kampagne {#add-to-campaign}

1. Klicken Sie in Salesforce auf die Registerkarte **Interessenten** und dann auf die Schaltfläche **Los**.

   ![](assets/four-3.png)

1. Wählen Sie die gewünschten Interessenten aus und klicken Sie auf die Schaltfläche **Hinzufügen zur MSC-Kampagne (Classic)**.

   ![](assets/five-3.png)

1. Es wird ein Popup &quot;Hinzufügen Personen zu Ihrer Kampagne&quot;angezeigt. Klicken Sie auf **Weiter** und gehen Sie durch den typischen Fluss der Kampagne, um eine MSC-Kampagne zu Trigger zu machen.

   ![](assets/six.png)

## Push to Marketing Sales Connect {#push-to-marketo-sales-connect}

1. Klicken Sie in Salesforce auf die Registerkarte **Interessenten** und dann auf die Schaltfläche **Los**.

   ![](assets/seven-1.png)

1. Wählen Sie die gewünschten Interessenten aus und klicken Sie auf die Schaltfläche **In MSC (Classic)** verschieben.

   ![](assets/eight-1.png)

1. Eine neue Registerkarte namens &quot;Salesforce Bridge&quot;wird geöffnet. Klicken Sie auf die Schaltfläche **Fahren Sie mit Gruppe →** fort.

   ![](assets/nine-1.png)

1. Sie werden an Ihr MSC-Konto gesendet, wo eine mit Datum-/Zeitstempel erstellte Gruppe angezeigt wird. Sie erhalten eine Benachrichtigung, sobald die Synchronisierung abgeschlossen ist und die Gruppe die von Salesforce synchronisierten Interessenten enthält.

   ![](assets/ten.png)

>[!NOTE]
>
>Sie können die gleichen Schritte ausführen, um Massenaktionen auch in der Ansicht Liste Kontakt zu verwenden.

>[!MORELIKETHIS]
>
>* [Senden von E-Mails per E-Mail](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Erstellen von Massen-E-Mails mit &quot;Auswählen&quot;und &quot;Senden&quot;](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)

