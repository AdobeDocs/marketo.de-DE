---
unique-page-id: 9438139
description: Person zu Blockierungsliste hinzufügen - Marketo Docs - Produktdokumentation
title: Person zu Blockierungsliste hinzufügen
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: de8eb7dd1b7f1da5d219ec8c182a02eb998a2a22
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 1%

---

# Person zu Blockierungsliste hinzufügen {#add-person-to-blocklist}

Wenn Sie Personen zu Ihrer Blockierungsliste hinzufügen, wird verhindert, dass sie Ihre Korrespondenz erhalten.

1. Erstellen Sie ein neues [Standardprogramm](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"} und nennen Sie es &quot;Zu Blockierungsliste hinzufügen&quot;.

1. Klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neues lokales Asset]** aus.

   ![](assets/add-person-to-blocklist-1.png)

1. Wählen Sie **[!UICONTROL Smart List]** aus.

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

1. Klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neue Smart-Kampagne]** aus.

   ![](assets/add-person-to-blocklist-6.png)

1. Benennen Sie die neue Smart-Kampagne. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/add-person-to-blocklist-7.png)

1. Ziehen Sie **[!UICONTROL Mitglied der Smart-Liste]** in den Arbeitsbereich.

   ![](assets/add-person-to-blocklist-8.png)

1. Wählen Sie die soeben erstellte Smart-Liste aus.

   ![](assets/add-person-to-blocklist-9.png)

1. Klicken Sie auf die Registerkarte **[!UICONTROL Fluss]**. Ziehen Sie die Flussaktion **[!UICONTROL Datenwert ändern]** in den Arbeitsbereich.

   ![](assets/add-person-to-blocklist-10.png)

1. Wählen Sie in der Dropdown-Liste **[!UICONTROL Attribut]** die Option **[!UICONTROL Block Listed]** und setzen Sie **[!UICONTROL New Value]** auf **[!UICONTROL true]**.

   ![](assets/add-person-to-blocklist-11.png)

1. Klicken Sie auf die Registerkarte **[!UICONTROL Plan]** und wählen Sie **[!UICONTROL Einmal ausführen]** aus.

   ![](assets/add-person-to-blocklist-12.png)

1. Wählen Sie **[!UICONTROL Jetzt ausführen]** und klicken Sie auf **[!UICONTROL Ausführen]**.

   ![](assets/add-person-to-blocklist-13.png)

1. Klicken Sie erneut auf **[!UICONTROL Ausführen]** .

   ![](assets/add-person-to-blocklist-14.png)

Diese Personen erhalten keine E-Mails mehr.

>[!TIP]
>
>Erstellen Sie eine [Trigger-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"} mit **Datenwert ändern** und dem Wert **-Auflistung ist wahr** für alle zukünftigen Personen, die über Blockierungsliste-fähige Attribute verfügen.
