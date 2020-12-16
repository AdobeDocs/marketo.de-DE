---
unique-page-id: 2360360
description: Erstellen eines Webhofs - Marketing Docs - Produktdokumentation
title: Erstellen eines Webhofs
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---


# Erstellen eines Webhofs {#create-a-webhook}

Verwenden Sie Webhooks, um Webdienste von Drittanbietern zu nutzen, um Textnachrichten zu senden, personenbezogene Daten zu erweitern und vieles mehr.

>[!NOTE]
>
>**Verfügbarkeit**
>
>Nicht alle Kunden haben diese Funktion erworben. Weitere Informationen erhalten Sie von Ihrem Vertriebsmitarbeiter.

1. Gehen Sie zu **Admin **und klicken Sie auf **Webhooks**.

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. Klicken Sie auf **Neuer Webhaken**.

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. Benennen und konfigurieren Sie Ihren Webshaken.

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >Hierzu gehört oft die Eingabe Ihrer Drittanbieter-Dienstanmeldeinformationen als URL-Parameter oder in die Vorlage &quot;POST&quot;.

   * **URL**: Geben Sie die URL ein, die Sie zur POST Ihrer Anforderung an den Webdienst verwenden. Klicken Sie zum Einfügen eines Tokens, z. B. der E-Mail-Adresse (**`{{lead.Email Address}}`**) der Person, in Ihre Anforderung auf Token **einfügen**.

   * **Vorlage**: Wenn Sie Informationen im Hauptteil der POST übermitteln möchten, geben Sie die Vorlage ein. Verwenden Sie alle Datenformate, die HTTP-POST unterstützen, einschließlich XML, JSON oder SOAP. Um ein Token in Ihre Vorlage einzufügen, klicken Sie auf &quot;Token **einfügen&quot;**.

   * **Token-Kodierung** anfordern: Wenn die Tokenwerte Sonderzeichen enthalten (z. B. ein kaufmännisches Und, &quot;&amp;&quot;), geben Sie das Format Ihrer Anforderung an (**JSON** oder **Form/URL**).

   * **Antworttyp**: Wählen Sie das Format der Antwort aus, die Sie vom Dienst erhalten (**JSON** oder **XML**).

   Klicken Sie auf Erstellen.

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>**Tieftauchen**
>
>Erfahren Sie mehr in den [Webhooks](http://developers.marketo.com/documentation/webhooks/) Deep Dive.

