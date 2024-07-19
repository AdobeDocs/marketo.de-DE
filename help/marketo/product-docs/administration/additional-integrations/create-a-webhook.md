---
unique-page-id: 2360360
description: Erstellen von  [!DNL Webhook]  - Marketo-Dokumenten - Produktdokumentation
title: Erstellen eines  [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
source-git-commit: 23a7b8cb1cd07c0194c08d30218602a52d03df5b
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 1%

---

# Erstellen einer [!DNL Webhook] {#create-a-webhook}

Verwenden Sie [!DNL Webhooks] , um Webdienste von Drittanbietern zu nutzen, um Textnachrichten zu senden, Personendaten zu erweitern und vieles mehr.

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/create-a-webhook-1.png)

1. Klicken Sie auf **[!UICONTROL Webhooks]**.

   ![](assets/create-a-webhook-2.png)

1. Klicken Sie auf **[!UICONTROL New Webhook]**.

   ![](assets/create-a-webhook-3.png)

1. Benennen und konfigurieren Sie Ihren [!DNL Webhook].

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Dazu gehört häufig die Eingabe Ihrer Anmeldedaten für den Drittanbieterdienst als URL-Parameter oder in die POST-Vorlage.

   * **[!UICONTROL URL]**: Geben Sie die URL ein, die Sie in Ihrer Anfrage an den Webdienst verwenden. Um ein Token wie die E-Mail-Adresse der Person (**`{{lead.Email Address}}`**) in Ihre Anfrage einzufügen, klicken Sie auf **[!UICONTROL Token einfügen]**.

   * **[!UICONTROL Vorlage]**: Wenn Sie Informationen im Hauptteil der Anfrage übermitteln möchten, geben Sie dies über die Payload-Vorlage ein. Für die folgenden Anforderungstypen zulässige Vorlagen: POST, DELETE, PATCH oder PUT. Sie können Datenformate wie JSON oder XML verwenden. Um ein Token in Ihre Vorlage einzufügen, klicken Sie auf **[!UICONTROL Token einfügen]**.

   * **[!UICONTROL Token-Kodierung anfordern]**: Wenn die Token-Werte Sonderzeichen enthalten (z. B. ein kaufmännisches Und-, &#39;&amp;&#39;-Zeichen), geben Sie das Format Ihrer Anfrage an (**JSON** oder **Formular/URL**).

   * **[!UICONTROL Antworttyp]**: Wählen Sie das Format der Antwort aus, die Sie vom Dienst erhalten (**JSON** oder **XML**).

   * **[!UICONTROL Anforderungstyp]**: Wählen Sie die zu verwendende HTTP-Methode aus (DELETE, GET, PATCH, POST, PUT).

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>Weitere Informationen finden Sie im tiefen Tauchgang [[!DNL Webhooks]](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/webhooks/webhooks){target="_blank"} .
