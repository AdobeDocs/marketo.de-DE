---
unique-page-id: 2360360
description: Webhook erstellen - Marketo-Dokumente - Produktdokumentation
title: Webhook erstellen
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
source-git-commit: 6f17d79344653d1b2c364753d774998e343c9808
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 3%

---

# Webhook erstellen {#create-a-webhook}

Verwenden Sie Webhooks, um Webdienste von Drittanbietern zu nutzen, um Textnachrichten zu senden, Personendaten zu erweitern und vieles mehr.

>[!AVAILABILITY]
>
>Nicht alle Kunden haben diese Funktion erworben. Detaillierte Informationen erhalten Sie vom zuständigen Vertriebsmitarbeiter.

1. Navigieren Sie zu **Admin** und klicken Sie auf **Webhooks**.

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. Klicken **Neuer Webhook**.

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. Benennen und konfigurieren Sie Ihren Webhook.

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >Dazu gehört häufig die Eingabe Ihrer Anmeldedaten für den Drittanbieterdienst als URL-Parameter oder in die POST-Vorlage.

   * **URL**: Geben Sie die URL ein, die Sie in Ihrer Anfrage an den Webdienst verwenden. So fügen Sie ein Token ein, z. B. die E-Mail-Adresse der Person (**`{{lead.Email Address}}`**), klicken Sie in Ihrer Anfrage auf **Token einfügen**.

   * **Vorlage**: Wenn Sie Informationen im Hauptteil der POST übermitteln möchten, geben Sie die Vorlage ein. Verwenden Sie jedes Datenformat, das die HTTP-POST unterstützt, einschließlich XML, JSON oder SOAP. Um ein Token in Ihre Vorlage einzufügen, klicken Sie auf **Token einfügen**.

   * **Token-Kodierung anfordern**: Wenn die Token-Werte Sonderzeichen enthalten (z. B. ein kaufmännisches Und-Zeichen, &quot;&amp;&quot;), geben Sie das Format Ihrer Anfrage an (**JSON** oder **Formular/URL**).

   * **Antworttyp**: Wählen Sie das Format der Antwort aus, die Sie vom Dienst erhalten (**JSON** oder **XML**).

   * **Anfragetyp**: Wählen Sie die zu verwendende HTTP-Methode aus (DELETE, GET, PATCH, POST, PUT)

   Klicken Sie auf **Erstellen**.

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>Weitere Informationen finden Sie unter [webhooks](https://developers.marketo.com/documentation/webhooks/) tief tauchen.
