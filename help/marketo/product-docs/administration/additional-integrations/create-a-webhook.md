---
unique-page-id: 2360360
description: Webhook erstellen - Marketo-Dokumente - Produktdokumentation
title: Webhook erstellen
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
source-git-commit: a498dcc5dc95bd7f732481d30db021485cf052c0
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 5%

---

# Webhook erstellen {#create-a-webhook}

Verwenden Sie Webhooks, um Webdienste von Drittanbietern zu nutzen, um Textnachrichten zu senden, Personendaten zu erweitern und vieles mehr.

>[!AVAILABILITY]
>
>Nicht alle Kunden haben diese Funktion erworben. Detaillierte Informationen erhalten Sie vom zuständigen Vertriebsmitarbeiter.

1. Navigieren Sie zum **Admin**-Bereich.

   ![](assets/create-a-webhook-1.png)

1. Klicken **Webhooks**.

   ![](assets/create-a-webhook-2.png)

1. Klicken **Neuer Webhook**.

   ![](assets/create-a-webhook-3.png)

1. Benennen und konfigurieren Sie Ihren Webhook.

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Dazu gehört häufig die Eingabe Ihrer Anmeldedaten für den Drittanbieterdienst als URL-Parameter oder in die POST-Vorlage.

   * **URL**: Geben Sie die URL ein, die Sie in Ihrer Anfrage an den Webdienst verwenden. So fügen Sie ein Token ein, z. B. die E-Mail-Adresse der Person (**`{{lead.Email Address}}`**), klicken Sie in Ihrer Anfrage auf **Token einfügen**.

   * **Vorlage**: Wenn Sie Informationen im Hauptteil der Anfrage übermitteln möchten, geben Sie dies über die Payload-Vorlage ein. Für die folgenden Anforderungstypen zulässige Vorlagen: POST, DELETE, PATCH oder PUT. Sie können Datenformate wie JSON oder XML verwenden. Um ein Token in Ihre Vorlage einzufügen, klicken Sie auf **Token einfügen**.

   * **Token-Kodierung anfordern**: Wenn die Token-Werte Sonderzeichen enthalten (z. B. ein kaufmännisches Und-Zeichen, &quot;&amp;&quot;), geben Sie das Format Ihrer Anfrage an (**JSON** oder **Formular/URL**).

   * **Antworttyp**: Wählen Sie das Format der Antwort aus, die Sie vom Dienst erhalten (**JSON** oder **XML**).

   * **Anfragetyp**: Wählen Sie die zu verwendende HTTP-Methode aus (DELETE, GET, PATCH, POST, PUT).

1. Klicken Sie auf **Erstellen**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>Weitere Informationen finden Sie unter [webhooks](https://developers.marketo.com/documentation/webhooks/) tief tauchen.
