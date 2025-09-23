---
unique-page-id: 14746470
description: Einrichten eines benutzerdefinierten Versandkanals - Marketo-Dokumente - Produktdokumentation
title: Einrichten eines benutzerdefinierten Versandkanals
exl-id: a31f7bfd-a4ee-4948-9bdc-b49d47054d40
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 4%

---

# Einrichten eines benutzerdefinierten Versandkanals {#setting-up-a-custom-delivery-channel}

[!DNL Marketo Sales Connect] ermöglicht die Integration mit einem benutzerdefinierten SMTP-Server für den Versand Ihrer E-Mails. Dies ist eine großartige Option für diejenigen, die keine Massen-E-Mails aus ihrem Gmail- oder [!DNL Exchange]-Versandkanal senden möchten.

Benutzer können einen benutzerdefinierten SMTP-Server für ihre eigene Verwendung einrichten, oder Administratoren können ein SMTP-Team einrichten, das für alle Benutzer [!DNL Sales Connect] Instanz freigegeben wird.

>[!NOTE]
>
>* Zusätzlich zur Einrichtung Ihres SMTP-Servers muss Ihre [E-Mail-Identität überprüft werden](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md) bevor Sie E-Mails versenden können.
>* Es wird empfohlen, mit Ihrem IT-Team oder SMTP-Server-Anbieter zusammenzuarbeiten, um die richtigen Server-Anmeldeinformationen für Ihren SMTP-Server zu erhalten.
>* Sie können Ihre Gmail- und [!DNL Exchange]-Server-Anmeldedaten nicht über den SMTP-Server verbinden. Nutzen Sie unseren E-Mail-Verbindungsservice, um sich mit diesen Anbietern zu integrieren.

## Benutzerdefiniertes SMTP {#custom-smtp}

1. Melden Sie sich bei der [Web-Anwendung](https://toutapp.com/login) an, klicken Sie oben rechts auf das Zahnradsymbol und wählen Sie **[!UICONTROL Einstellungen]** aus.

   ![](assets/setting-up-a-custom-delivery-channel-1.png)

1. Klicken [!UICONTROL  unter „Mein ]&quot; auf **[!UICONTROL E-Mail-Einstellungen]**.

   ![](assets/setting-up-a-custom-delivery-channel-2.png)

1. Klicken Sie **[!UICONTROL Benutzerdefinierter Versandkanal]**.

   ![](assets/setting-up-a-custom-delivery-channel-3.png)

1. Geben Sie Ihre [!UICONTROL SMTP-Server]-Anmeldeinformationen ein und klicken Sie auf **[!UICONTROL Verbinden]**.

   ![](assets/setting-up-a-custom-delivery-channel-4.png)

   >[!NOTE]
   >
   >Wenn dies Ihr einziger Versandkanal ist, wird er automatisch allen Ihren E-Mail-Identitäten zugewiesen und Sie sind hier fertig. Wenn dies nicht der einzige Versandkanal ist, fahren Sie mit Schritt 5 fort.

1. Klicken Sie noch in [!UICONTROL E-Mail]Einstellungen) auf **[!UICONTROL Adresse und Signatur]**.

   ![](assets/setting-up-a-custom-delivery-channel-5.png)

1. Suchen Sie die E-Mail-Identität, für die Sie einen Versandkanal auswählen möchten, und klicken Sie auf **[!UICONTROL Versandkanal auswählen]**.

   ![](assets/setting-up-a-custom-delivery-channel-6.png)

1. Klicken Sie auf [!UICONTROL  Karte ]Zustellbarkeit **[!UICONTROL auf]**.

   ![](assets/setting-up-a-custom-delivery-channel-7.png)

1. Klicken Sie auf [!UICONTROL Kanal] und wählen Sie den benutzerdefinierten Versandkanal aus, den Sie soeben hinzugefügt haben. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/setting-up-a-custom-delivery-channel-8.png)

   >[!NOTE]
   >
   >Wenn Ihr Teamadministrator den SMTP-Server für das Team einrichtet, wird er automatisch nur auf Ihre Standard-E-Mail-Identität angewendet und steht als Option für Ihre anderen E-Mail-Identitäten zur Verfügung.

## Team SMTP-Server {#team-smtp-server}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Melden Sie sich bei der [Web-Anwendung](https://toutapp.com/login) an, klicken Sie oben rechts auf das Zahnradsymbol und wählen Sie **[!UICONTROL Einstellungen]** aus.

   ![](assets/setting-up-a-custom-delivery-channel-9.png)

1. Klicken [!UICONTROL  unter &quot;]&quot; auf **[!UICONTROL Allgemein]**.

   ![](assets/setting-up-a-custom-delivery-channel-10.png)

1. Klicken Sie **[!UICONTROL Versandkanal des Teams]**.

   ![](assets/setting-up-a-custom-delivery-channel-11.png)

1. Geben Sie Ihre [!UICONTROL SMTP-Server]-Anmeldeinformationen ein und klicken Sie auf **[!UICONTROL Verbinden]**.

   ![](assets/setting-up-a-custom-delivery-channel-12.png)

   >[!NOTE]
   >
   >Der SMTP-Server des Teams ist der Standard-Versandkanal der Standard-E-Mail-Identität für alle Team-Mitglieder. Darüber hinaus ist sie als Versandkanal-Option für alle anderen E-Mail-Identitäten verfügbar.

   >[!MORELIKETHIS]
   >
   >* [E-Mail-Verbindung für Gmail-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
   >
   >* [E-Mail-Verbindung für [!DNL Outlook] Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
