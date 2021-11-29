---
description: Einrichten eines benutzerdefinierten Bereitstellungskanals - Marketo Docs - Produktdokumentation
title: Einrichten eines benutzerdefinierten Bereitstellungskanals
hide: true
hidefromtoc: true
source-git-commit: 55afdc537d0a5d0b6114f478c4dd2ded09c84e34
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---

# Einrichten eines benutzerdefinierten Bereitstellungskanals {#setting-up-a-custom-delivery-channel}

Mit Marketo Sales Connect können Sie für die Zustellung Ihrer E-Mails einen benutzerdefinierten SMTP-Server integrieren. Dies ist eine großartige Option für diejenigen, die keine Massen-E-Mails aus ihrem Gmail- oder Exchange-Versandkanal versenden möchten.

Benutzer können einen benutzerdefinierten SMTP-Server für ihre eigene individuelle Verwendung einrichten oder Administratoren können ein Team-SMTP einrichten, das für alle Sales Connect-Benutzer in Ihrer Instanz freigegeben wird.

>[!NOTE]
>
>* Zusätzlich zur Einrichtung Ihres SMTP-Servers muss Ihr [E-Mail-Identität muss überprüft werden](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md) bevor Sie E-Mails versenden können.
>* Wir empfehlen, mit Ihrem IT-Team oder SMTP-Serveranbieter zusammenzuarbeiten, um die richtigen Serverberechtigungen für Ihren SMTP-Server zu erhalten.
>* Sie können Ihren Gmail- und Exchange-Server nicht mit den SMTP-Server-Anmeldedaten verbinden. Bitte nutzen Sie unseren Email Connection-Dienst, um sich mit diesen Anbietern zu integrieren.


## Benutzerdefiniertes SMTP {#custom-smtp}

1. Melden Sie sich bei der [Webanwendung](https://toutapp.com/login), klicken Sie auf das Zahnradsymbol oben rechts und wählen Sie **Einstellungen**.

PICC

1. Klicken Sie unter &quot;Mein Konto&quot;auf **E-Mail-Einstellungen**.

PICC

1. Klicken **Benutzerspezifischer Bereitstellungskanal**.

PICC

1. Geben Sie Ihre SMTP Server-Anmeldedaten ein und klicken Sie auf **Verbinden**.

PICC

>[!NOTE]
>
>Wenn dies Ihr einziger Versandkanal ist, wird er automatisch all Ihren E-Mail-Identitäten zugewiesen und Sie sind hier fertig. Wenn dies nicht Ihr einziger Versandkanal ist, fahren Sie mit Schritt 5 fort.

1. Klicken Sie weiterhin in den E-Mail-Einstellungen auf **Adresse und Unterschrift**.

PICC

1. Suchen Sie die E-Mail-Identität, für die Sie einen Versandkanal auswählen möchten, und klicken Sie auf **Versandkanal auswählen**.

PICC

1. Klicken Sie in der Zustellbarkeits-Karte auf **Bearbeiten**.

PICC

1. Klicken Sie auf das Dropdown-Menü Kanal und wählen Sie den soeben hinzugefügten benutzerdefinierten Versandkanal aus. Klicken **Speichern**.

PICC

>[!NOTE]
>
>Wenn Ihr Team-Administrator den Team-SMTP-Server eingerichtet hat, wird dieser automatisch nur auf Ihre Standard-E-Mail-Identität angewendet und ist als Option für Ihre anderen E-Mail-Identitäten verfügbar.

## Team SMTP-Server {#team-smtp-server}

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

1. Melden Sie sich bei der [Webanwendung](https://toutapp.com/login), klicken Sie auf das Zahnradsymbol oben rechts und wählen Sie **Einstellungen**.

PICC

1. Klicken Sie unter &quot;Admin Settings&quot;auf **Allgemein**.

PICC

1. Klicken **Team Delivery Channel**.

PICC

1. Geben Sie Ihre SMTP Server-Anmeldedaten ein und klicken Sie auf **Verbinden**.

PICC

>[!NOTE]
>
>Der Team-SMTP-Server ist der standardmäßige Versandkanal der Standard-E-Mail-Identität für alle Teammitglieder. Darüber hinaus ist es als Option für den Versandkanal für alle anderen E-Mail-Identitäten verfügbar.

>[!MORELIKETHIS]
>
>* [E-Mail-Verbindung für Gmail-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [E-Mail-Verbindung für Outlook-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

