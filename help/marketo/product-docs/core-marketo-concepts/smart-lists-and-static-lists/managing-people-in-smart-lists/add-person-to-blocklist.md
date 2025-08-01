---
unique-page-id: 9438139
description: Person zur Blockierungsliste hinzufügen - Marketo-Dokumente - Produktdokumentation
title: Person zur Blockierungsliste hinzufügen
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 1%

---

# Person zur Blockierungsliste hinzufügen {#add-person-to-blocklist}

Wenn Sie Personen zu Ihrer Blockierungsliste hinzufügen, können diese Ihre Korrespondenz nicht erhalten.

1. Erstellen Sie ein neues [Standardprogramm](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"} und nennen Sie es „Zu Blockierungsliste hinzufügen“.

1. Klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neues lokales Asset]**.

   ![](assets/add-person-to-blocklist-1.png)

1. Wählen Sie **[!UICONTROL Smart-Liste]** aus.

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

1. Klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neue Smart-Kampagne]**.

   ![](assets/add-person-to-blocklist-6.png)

1. Benennen Sie die neue Smart-Kampagne. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/add-person-to-blocklist-7.png)

1. Drag-and-Drop **[!UICONTROL Mitglied der Smart-]**)

   ![](assets/add-person-to-blocklist-8.png)

1. Wählen Sie die soeben erstellte Smart-Liste aus.

   ![](assets/add-person-to-blocklist-9.png)

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Fluss“. Ziehen Sie die Flussaktion **[!UICONTROL Datenwert ändern]** per Drag-and-Drop.

   ![](assets/add-person-to-blocklist-10.png)

1. Wählen Sie in **[!UICONTROL Dropdown]** Attribut“ **[!UICONTROL Blockierungsliste]** aus und setzen Sie **[!UICONTROL Neuer Wert]** auf **[!UICONTROL true]**.

   ![](assets/add-person-to-blocklist-11.png)

1. Klicken Sie auf die **[!UICONTROL Zeitplan]** und wählen Sie **[!UICONTROL Einmal ausführen]**.

   ![](assets/add-person-to-blocklist-12.png)

1. Wählen Sie **[!UICONTROL Jetzt ausführen]** und klicken Sie auf **[!UICONTROL Ausführen]**.

   ![](assets/add-person-to-blocklist-13.png)

1. Klicken Sie **[!UICONTROL erneut auf]** Ausführen“.

   ![](assets/add-person-to-blocklist-14.png)

Diese Personen erhalten keine E-Mails mehr.

>[!TIP]
>
>Erstellen Sie eine [&#128279;](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}-Kampagne mit **Datenwert ändern** mit **Blockierungsliste ist wahr** für alle Personen in der Zukunft, die Attribut für eine Trigger auf die Blockierungsliste setzte haben.
