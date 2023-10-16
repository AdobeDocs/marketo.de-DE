---
unique-page-id: 1147154
description: Synchronisieren einer SFDC-Kampagne mit einem Programm - Marketo Docs - Produktdokumentation
title: Synchronisieren einer SFDC-Kampagne mit einem Programm
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: e49860ae611f2f77789bb491aeccbee46a911a2c
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 1%

---

# Synchronisieren einer SFDC-Kampagne mit einem Programm {#sync-an-sfdc-campaign-with-a-program}

Mit Marketo Engage können Sie Ihre Programme synchronisieren mit [!DNL Salesforce] Kampagnen, um in beiden Systemen die gleiche Liste von Personen zu verwalten, einschließlich ihres Status. Los geht’s!

>[!PREREQUISITES]
>
>Sie müssen [enable [!DNL Salesforce] Kampagnensynchronisierung](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) zuerst.

>[!CAUTION]
>
>Beim Synchronisieren einer SFDC-Kampagne mit einem Marketo Engage-Programm werden die impliziten SFDC-Aktionen (z. B. Hinzufügen zu SFDC Campaign, Synchronisieren mit SFDC) für untergeordnete Kampagnen des Programms deaktiviert.

1. Navigieren Sie zu **[!UICONTROL Marketingaktivitäten]**.

   ![](assets/login-marketing-activities-1.png)

1. Wählen Sie Ihr Programm aus.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Klicks **[!UICONTROL Programmaktionen]**, wählen Sie **[!UICONTROL Salesforce Campaign Sync]**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Auswählen **[!UICONTROL Neu erstellen]** oder wählen Sie eine bestehende Salesforce-Kampagne aus.

   >[!TIP]
   >
   >Wenn Sie eine bestehende Salesforce-Kampagne auswählen, stellen Sie sicher, dass [Übereinstimmung mit dem Programmstatus der Salesforce-Kampagne und des Marketo-Programms](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

1. Benennen Sie die neue Kampagne und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Jetzt können Sie die Details der Kampagnensynchronisierung auf der Seite mit der Programmzusammenfassung überprüfen.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Ausgezeichnet! Jetzt werden alle Änderungen des Programmstatus in Marketo mit der SFDC-Kampagne synchronisiert und umgekehrt.
