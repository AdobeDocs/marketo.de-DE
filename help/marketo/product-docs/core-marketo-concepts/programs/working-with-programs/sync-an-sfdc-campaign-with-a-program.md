---
unique-page-id: 1147154
description: Synchronisieren einer SFDC-Kampagne mit einem Programm - Marketo Docs - Produktdokumentation
title: Synchronisieren einer SFDC-Kampagne mit einem Programm
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# Synchronisieren einer SFDC-Kampagne mit einem Programm {#sync-an-sfdc-campaign-with-a-program}

Mit Marketo Engage können Sie Ihre Programme mit [!DNL Salesforce] -Kampagnen synchronisieren, um in beiden Systemen die gleiche Personenliste einschließlich ihres Status zu erhalten. Fangen wir an!

>[!PREREQUISITES]
>
>Sie müssen zuerst [die [!DNL Salesforce] Kampagnensynchronisierung](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"} aktivieren.

>[!CAUTION]
>
>Beim Synchronisieren einer SFDC-Kampagne mit einem Marketo Engage-Programm werden die impliziten SFDC-Aktionen (z. B. Hinzufügen zu SFDC Campaign, Synchronisieren mit SFDC) für untergeordnete Kampagnen des Programms deaktiviert.

1. Wechseln Sie zu **[!UICONTROL Marketingaktivitäten]**.

   ![](assets/login-marketing-activities-1.png)

1. Wählen Sie Ihr Programm aus.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Klicken Sie auf **[!UICONTROL Programmaktionen]** und wählen Sie dann **[!UICONTROL Salesforce-Kampagnensynchronisierung]** aus.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Wählen Sie **[!UICONTROL Neu erstellen]** oder eine vorhandene [!DNL Salesforce] Kampagne aus.

   >[!TIP]
   >
   >Wenn Sie eine bestehende [!DNL Salesforce] -Kampagne auswählen, achten Sie darauf, dass [mit dem Programmstatus der [!DNL Salesforce] Kampagne und des Marketo-Programms](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"} übereinstimmt.

1. Geben Sie einen Namen für die neue Kampagne ein und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Jetzt können Sie die Details der Kampagnensynchronisierung auf der Seite mit der Programmzusammenfassung überprüfen.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Ausgezeichnet! Jetzt werden alle Änderungen des Programmstatus in Marketo mit der SFDC-Kampagne synchronisiert und umgekehrt.
