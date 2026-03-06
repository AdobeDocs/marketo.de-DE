---
unique-page-id: 2360360
description: Erstellen Sie einen Webhook in Admin, um Webservices von Drittanbietern für SMS, Personendaten und mehr aufzurufen.
title: Erstellen eines [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---

# Erstellen eines [!DNL Webhook] {#create-a-webhook}

Verwenden Sie [!DNL Webhooks], um Web-Services von Drittanbietern zu nutzen, um Textnachrichten zu senden, Personendaten zu erweitern und vieles mehr.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/create-a-webhook-1.png)

1. Klicken Sie **[!UICONTROL Webhooks]**.

   ![](assets/create-a-webhook-2.png)

1. Klicken Sie auf **[!UICONTROL Neuer Webhook]**.

   ![](assets/create-a-webhook-3.png)

1. Benennen und konfigurieren Sie Ihre [!DNL Webhook].

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Dazu gehört häufig die Eingabe Ihrer Service-Anmeldeinformationen von Drittanbietern als URL-Parameter oder in der POST-Vorlage.

   * **[!UICONTROL URL]**: Geben Sie die URL ein, die Sie in Ihrer Anfrage an den Webservice verwenden. Um ein Token, z. B. die E-Mail-Adresse der Person (**`{{lead.Email Address}}`**), in Ihre Anfrage einzufügen, klicken Sie auf **[!UICONTROL Token einfügen]**.

   * **[!UICONTROL Vorlage]**: Wenn Sie Informationen im Textkörper der Anfrage übertragen möchten, geben Sie dies über die Payload-Vorlage ein. Vorlagen zulässig für die folgenden Anfragetypen: POST, DELETE, PATCH oder PUT. Sie können Datenformate wie JSON oder XML verwenden. Um ein Token in Ihre Vorlage einzufügen, klicken Sie auf **[!UICONTROL Token einfügen]**.

   * **[!UICONTROL Kodierung von Anfrage]**: Wenn die Token-Werte Sonderzeichen enthalten (z. B. ein kaufmännisches Und-Zeichen, &quot;&amp;„), geben Sie das Format Ihrer Anfrage an (**JSON** oder **Form/Url**).

   * **[!UICONTROL Antworttyp]**: Wählen Sie das Format der Antwort aus, die Sie vom Dienst erhalten (**JSON** oder **XML**).

   * **[!UICONTROL Anfragetyp]**: Wählen Sie die zu verwendende HTTP-Methode aus (DELETE, GET, PATCH, POST, PUT).

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>Weitere Informationen finden Sie in den [[!DNL Webhooks]](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/webhooks/webhooks){target="_blank"}.
