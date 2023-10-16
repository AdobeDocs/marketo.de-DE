---
unique-page-id: 2360360
description: Erstellen Sie eine [!DNL Webhook] - Marketo-Dokumente - Produktdokumentation
title: Erstellen Sie eine [!DNL Webhook]
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
feature: Administration, Webhooks
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 3%

---

# Erstellen Sie eine [!DNL Webhook] {#create-a-webhook}

Verwendung [!DNL Webhooks] , um Webdienste von Drittanbietern zu nutzen, um Textnachrichten zu senden, Personendaten zu erweitern und vieles mehr.

>[!AVAILABILITY]
>
>Nicht alle Marketo Engage-Benutzer haben diese Funktion erworben. Weitere Informationen erhalten Sie vom Adobe Account Team (Ihrem Kundenbetreuer).

1. Navigieren Sie zum **[!UICONTROL Admin]**-Bereich.

   ![](assets/create-a-webhook-1.png)

1. Klicks **[!UICONTROL Webhooks]**.

   ![](assets/create-a-webhook-2.png)

1. Klicks **[!UICONTROL Neuer Webhook]**.

   ![](assets/create-a-webhook-3.png)

1. Benennen und konfigurieren Sie Ihre [!DNL Webhook].

   ![](assets/create-a-webhook-4.png)

   >[!NOTE]
   >
   >Dazu gehört häufig die Eingabe Ihrer Anmeldedaten für den Drittanbieterdienst als URL-Parameter oder in die POST-Vorlage.

   * **[!UICONTROL URL]**: Geben Sie die URL ein, die Sie in Ihrer Anforderung für den Webdienst verwenden. So fügen Sie ein Token ein, z. B. die E-Mail-Adresse der Person (**`{{lead.Email Address}}`**), klicken Sie in Ihrer Anfrage auf **[!UICONTROL Token einfügen]**.

   * **[!UICONTROL Vorlage]**: Wenn Sie Informationen im Hauptteil der Anfrage übermitteln möchten, geben Sie dies über die Payload-Vorlage ein. Für die folgenden Anforderungstypen zulässige Vorlagen: POST, DELETE, PATCH oder PUT. Sie können Datenformate wie JSON oder XML verwenden. Um ein Token in Ihre Vorlage einzufügen, klicken Sie auf **[!UICONTROL Token einfügen]**.

   * **[!UICONTROL Token-Kodierung anfordern]**: Wenn die Token-Werte Sonderzeichen enthalten (z. B. ein kaufmännisches Und-Zeichen, &quot;&amp;&quot;), geben Sie das Format Ihrer Anfrage an (**JSON** oder **Formular/URL**).

   * **[!UICONTROL Antworttyp]**: Wählen Sie das Format der Antwort aus, die Sie vom Dienst erhalten (**JSON** oder **XML**).

   * **[!UICONTROL Anfragetyp]**: Wählen Sie die zu verwendende HTTP-Methode aus (DELETE, GET, PATCH, POST, PUT).

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/create-a-webhook-5.png)

>[!NOTE]
>
>Weitere Informationen finden Sie unter [[!DNL Webhooks]](https://developers.marketo.com/documentation/webhooks/){target="_blank"} tief tauchen.
