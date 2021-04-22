---
unique-page-id: 2360360
description: Erstellen eines Webhofs - Marketo Docs - Produktdokumentation
title: Erstellen eines Webhofs
exl-id: 3e753d2d-6f33-4987-884e-8e13167cf3df
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 4%

---

# Erstellen eines Webhofs {#create-a-webhook}

Verwenden Sie Webhooks, um Webdienste von Drittanbietern zu nutzen, um Textnachrichten zu senden, personenbezogene Daten zu erweitern und vieles mehr.

>[!AVAILABILITY]
>
>Nicht alle Kunden haben diese Funktion erworben. Detaillierte Informationen erhalten Sie vom zuständigen Vertriebsmitarbeiter.

1. Gehen Sie zu **Admin** und klicken Sie auf **Webhooks**.

   ![](assets/image2014-9-24-14-3a52-3a57.png)

1. Klicken Sie auf **Neuer WebHaken**.

   ![](assets/image2014-9-24-14-3a53-3a9.png)

1. Benennen und konfigurieren Sie Ihren Webshaken.

   ![](assets/image2014-9-24-14-3a53-3a19.png)

   >[!NOTE]
   >
   >Hierzu gehört oft die Eingabe Ihrer Drittanbieter-Dienstanmeldeinformationen als URL-Parameter oder in die Vorlage &quot;POST&quot;.

   * **URL**: Geben Sie die URL ein, die Sie zur POST Ihrer Anforderung an den Webdienst verwenden. Klicken Sie zum Einfügen eines Tokens, z. B. der E-Mail-Adresse der Person (**`{{lead.Email Address}}`**), in Ihre Anforderung auf **Token einfügen**.

   * **Vorlage**: Wenn Sie Informationen im Hauptteil der POST übermitteln möchten, geben Sie die Vorlage ein. Verwenden Sie alle Datenformate, die HTTP-POST unterstützen, einschließlich XML, JSON oder SOAP. Um ein Token in Ihre Vorlage einzufügen, klicken Sie auf **Token einfügen**.

   * **Token-Kodierung** anfordern: Wenn die Tokenwerte Sonderzeichen enthalten (z. B. ein kaufmännisches Und, &quot;&amp;&quot;), geben Sie das Format Ihrer Anforderung an (**** JSONs oder  **Form/URL**).

   * **Antworttyp**: Wählen Sie das Format der Antwort aus, die Sie vom Dienst erhalten (**** JSON oder  **XML**).

   Klicken Sie auf Erstellen.

   ![](assets/image2014-9-24-14-3a53-3a35.png)

>[!NOTE]
>
>Erfahren Sie mehr in den [Webhooks](https://developers.marketo.com/documentation/webhooks/) Deep Dive.
