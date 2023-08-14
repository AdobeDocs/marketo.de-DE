---
unique-page-id: 9438139
description: Person zu Blockierungsliste hinzufügen - Marketo Docs - Produktdokumentation
title: Person zu Blockierungsliste hinzufügen
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: cc87ecb8d3245734ec0ce984eeccf742833a85d2
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 3%

---

# Person zu Blockierungsliste hinzufügen {#add-person-to-blocklist}

Wenn Sie Personen zu Ihrer Blockierungsliste hinzufügen, wird verhindert, dass sie Ihre Korrespondenz erhalten.

1. [Neues Standardprogramm erstellen](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) und benennen Sie sie **Zu Blockierungsliste hinzufügen**.

1. Klicks **Neu** und wählen **Neues lokales Asset**.

   ![](assets/add-person-to-blocklist-1.png)

1. Auswählen **Smart List**.

   ![](assets/add-person-to-blocklist-2.png)

1. Benennen Sie Ihre Liste und klicken Sie auf **Erstellen**.

   ![](assets/add-person-to-blocklist-3.png)

1. Fügen Sie alle Personen zu Ihren **Smart List** Sie möchten zu Ihrer Blockierungsliste hinzugefügt werden.

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >Personen auf Ihrer Blockierungsliste erhalten keine operativen E-Mails.

1. Gehen Sie zurück zu Ihrem Programm.

   ![](assets/add-person-to-blocklist-5.png)

1. Klicks **Neu** und wählen **Neue intelligente Kampagne**.

   ![](assets/add-person-to-blocklist-6.png)

1. Benennen Sie die **Neue intelligente Kampagne**. Klicken Sie auf **Erstellen**.

   ![](assets/add-person-to-blocklist-7.png)

1. Drag &amp; Drop **Mitglied der Smart List**.

   ![](assets/add-person-to-blocklist-8.png)

1. Wählen Sie die soeben erstellte Smart-Liste aus.

   ![](assets/add-person-to-blocklist-9.png)

1. Klicken Sie auf die Registerkarte **“Flow“**. Ziehen Sie die **Datenwert ändern** Flussaktion.

   ![](assets/add-person-to-blocklist-10.png)

1. Im **Attribut** Dropdown-Auswahl **Block Listed** und **Neuer Wert** nach **true**.

   ![](assets/add-person-to-blocklist-11.png)

1. Klicken Sie auf **Zeitplan** Registerkarte und wählen Sie **Einmal ausführen**.

   ![](assets/add-person-to-blocklist-12.png)

1. Auswählen **Jetzt ausführen** und klicken **Ausführen**.

   ![](assets/add-person-to-blocklist-13.png)

1. Klicks **Ausführen** erneut.

   ![](assets/add-person-to-blocklist-14.png)

Diese Personen erhalten keine E-Mails mehr.

>[!TIP]
>
>Erstellen Sie eine [Smart-Kampagne für Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) using **Datenwert ändern** mit **Block Listed is true** für alle zukünftigen Personen mit Attributen, die über Blockierungsliste verfügen.
