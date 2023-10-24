---
unique-page-id: 9438139
description: Person zu Blockierungsliste hinzufügen - Marketo Docs - Produktdokumentation
title: Person zu Blockierungsliste hinzufügen
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: de8eb7dd1b7f1da5d219ec8c182a02eb998a2a22
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 3%

---

# Person zu Blockierungsliste hinzufügen {#add-person-to-blocklist}

Wenn Sie Personen zu Ihrer Blockierungsliste hinzufügen, wird verhindert, dass sie Ihre Korrespondenz erhalten.

1. Erstellen Sie eine neue [Standardprogramm](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"} und benennen Sie sie &quot;Zu Blockierungsliste hinzufügen&quot;.

1. Klicks **[!UICONTROL Neu]** und wählen **[!UICONTROL Neues lokales Asset]**.

   ![](assets/add-person-to-blocklist-1.png)

1. Auswählen **[!UICONTROL Smart List]**.

   ![](assets/add-person-to-blocklist-2.png)

1. Benennen Sie Ihre Liste und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/add-person-to-blocklist-3.png)

1. Fügen Sie alle Personen zu Ihrer Smart-Liste hinzu, die Sie Ihrer Blockierungsliste hinzufügen möchten.

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >Personen auf Ihrer Blockierungsliste erhalten keine operativen E-Mails.

1. Gehen Sie zurück zu Ihrem Programm.

   ![](assets/add-person-to-blocklist-5.png)

1. Klicks **[!UICONTROL Neu]** und wählen **[!UICONTROL Neue intelligente Kampagne]**.

   ![](assets/add-person-to-blocklist-6.png)

1. Benennen Sie die neue Smart-Kampagne. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/add-person-to-blocklist-7.png)

1. Drag &amp; Drop **[!UICONTROL Mitglied der Smart List]**.

   ![](assets/add-person-to-blocklist-8.png)

1. Wählen Sie die soeben erstellte Smart-Liste aus.

   ![](assets/add-person-to-blocklist-9.png)

1. Klicken Sie auf die Registerkarte **[!UICONTROL “Flow“]**. Ziehen Sie die **[!UICONTROL Datenwert ändern]** Flussaktion.

   ![](assets/add-person-to-blocklist-10.png)

1. Im **[!UICONTROL Attribut]** Dropdown-Auswahl **[!UICONTROL Block Listed]** und **[!UICONTROL Neuer Wert]** nach **[!UICONTROL true]**.

   ![](assets/add-person-to-blocklist-11.png)

1. Klicken Sie auf **[!UICONTROL Zeitplan]** Registerkarte und wählen Sie **[!UICONTROL Einmal ausführen]**.

   ![](assets/add-person-to-blocklist-12.png)

1. Auswählen **[!UICONTROL Jetzt ausführen]** und klicken **[!UICONTROL Ausführen]**.

   ![](assets/add-person-to-blocklist-13.png)

1. Klicks **[!UICONTROL Ausführen]** erneut.

   ![](assets/add-person-to-blocklist-14.png)

Diese Personen erhalten keine E-Mails mehr.

>[!TIP]
>
>Erstellen Sie eine [Trigger Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"} using **Datenwert ändern** mit **Block Listed is true** für alle zukünftigen Personen mit Attributen, die über Blockierungsliste verfügen.
