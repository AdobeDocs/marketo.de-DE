---
unique-page-id: 14746470
description: Einrichten eines benutzerspezifischen Versand-Kanals - Marketing Docs - Produktdokumentation
title: Einrichten eines benutzerspezifischen Versand-Kanals
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Einrichten eines benutzerspezifischen Versand-Kanals {#setting-up-a-custom-delivery-channel}

Mit Marketo Sales Connect können Sie zum Versand Ihrer E-Mails einen benutzerdefinierten SMTP-Server integrieren. Dies ist eine großartige Option für diejenigen, die keine Massen-E-Mails aus ihrem Gmail- oder Exchange-Versand-Kanal senden möchten.

Benutzer können einen benutzerdefinierten SMTP-Server für ihre eigene individuelle Nutzung einrichten oder Administratoren können ein Team-SMTP einrichten, das für alle Sales Connect-Benutzer in Ihrer Instanz freigegeben wird.

>[!NOTE]
>
>* Neben der Einrichtung Ihres SMTP-Servers muss Ihre [E-Mail-Identität überprüft werden, bevor Sie E-Mails senden können.](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md)
>* Es wird empfohlen, mit Ihrem IT-Team oder dem Anbieter des SMTP-Servers zusammenzuarbeiten, um die richtigen Serverberechtigungen für Ihren SMTP-Server zu erhalten.
>* Sie können Ihren Gmail- und Exchange-Server nicht mit den Anmeldeinformationen des SMTP-Servers verbinden. Bitte nutzen Sie unseren E-Mail-Verbindungsdienst, um sich mit diesen Anbietern zu integrieren.


## Benutzerspezifisches SMTP {#custom-smtp}

1. Melden Sie sich bei der [Webanwendung](https://toutapp.com/login) an, klicken Sie auf das Zahnradsymbol oben rechts und wählen Sie **Einstellungen**.

   ![](assets/setting-up-a-custom-delivery-channel-1.png)

1. Klicken Sie unter Mein Konto auf **E-Mail-Einstellungen**.

   ![](assets/setting-up-a-custom-delivery-channel-2.png)

1. Klicken Sie auf **Benutzerdefinierter Versand Kanal**.

   ![](assets/setting-up-a-custom-delivery-channel-3.png)

1. Geben Sie Ihre SMTP Server-Anmeldeinformationen ein und klicken Sie auf **Connect**.

   ![](assets/setting-up-a-custom-delivery-channel-4.png)

   >[!NOTE]
   >
   >Wenn dies Ihr einziger Versand-Kanal ist, wird er automatisch all Ihren E-Mail-Identitäten zugewiesen und Sie sind hier fertig. Wenn dies nicht Ihr einziger Versand-Kanal ist, fahren Sie mit Schritt 5 fort.

1. Klicken Sie in den E-Mail-Einstellungen weiterhin auf **Adresse und Unterschrift**.

   ![](assets/setting-up-a-custom-delivery-channel-5.png)

1. Suchen Sie die E-Mail-Identität, für die Sie einen Versand-Kanal auswählen möchten, und klicken Sie auf **Wählen Sie den Kanal Versand**.

   ![](assets/setting-up-a-custom-delivery-channel-6.png)

1. Klicken Sie in der Auslieferungskarte auf **Bearbeiten**.

   ![](assets/setting-up-a-custom-delivery-channel-7.png)

1. Klicken Sie auf die Dropdownliste Kanal und wählen Sie den soeben hinzugefügten benutzerspezifischen Versand-Kanal aus. Klicken Sie auf **Speichern**.

   ![](assets/setting-up-a-custom-delivery-channel-8.png)

   >[!NOTE]
   >
   >Wenn Ihr Team-Administrator den Team SMTP Server eingerichtet hat, wird dieser automatisch nur auf Ihre Standard-E-Mail-Identität angewendet und als Option für Ihre anderen E-Mail-Identitäten verfügbar sein.

## Team SMTP Server {#team-smtp-server}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Melden Sie sich bei der [Webanwendung](https://toutapp.com/login) an, klicken Sie auf das Zahnradsymbol oben rechts und wählen Sie **Einstellungen**.

   ![](assets/setting-up-a-custom-delivery-channel-9.png)

1. Klicken Sie unter &quot;Admin-Einstellungen&quot;auf **Allgemein**.

   ![](assets/setting-up-a-custom-delivery-channel-10.png)

1. Klicken Sie auf **Team Versand Kanal**.

   ![](assets/setting-up-a-custom-delivery-channel-11.png)

1. Geben Sie Ihre SMTP Server-Anmeldeinformationen ein und klicken Sie auf **Connect**.

   ![](assets/setting-up-a-custom-delivery-channel-12.png)

   >[!NOTE]
   >
   >Der Team SMTP Server ist der Standard-Versand der Standard-E-Mail-Identität aller Teammitglieder. Darüber hinaus ist sie als Versand-Kanal für alle anderen E-Mail-Identitäten verfügbar.

   >[!MORELIKETHIS]
   >
   >* [E-Mail-Verbindung für Gmail-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
      >
      >
   * [E-Mail-Verbindung für Outlook-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

