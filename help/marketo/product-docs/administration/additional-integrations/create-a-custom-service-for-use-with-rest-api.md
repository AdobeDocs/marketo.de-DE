---
unique-page-id: 2360350
description: Erstellen eines benutzerdefinierten Services zur Verwendung mit der ReST-API - Marketo-Dokumente - Produktdokumentation
title: Erstellen eines benutzerdefinierten Service zur Verwendung mit der REST-API
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 7f8968210659ed2c51640966115f22da47e42ebf
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 12%

---

# Erstellen eines benutzerdefinierten Service zur Verwendung mit der REST-API {#create-a-custom-service-for-use-with-rest-api}

Wenn Sie eine Integration mit Marketo über die REST-API durchführen möchten, sollten Sie einen benutzerdefinierten Service erstellen. Und so geht das.

>[!PREREQUISITES]
>
>* [Erstellen einer Benutzerrolle nur für API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Nur API-Benutzer erstellen](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md)
>

>[!NOTE]
>
>**Admin-Berechtigungen erforderlich**

>[!TIP]
>
>Weitere Informationen zur (REST-API) finden Sie in [&#x200B; Entwicklerdokumentation &#x200B;](https://developer.adobe.com/marketo-apis/). Wir verfügen auch über die [SOAP](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/soap/soap-api)API, falls Sie sie benötigen.

## Benutzerdefinierten Service erstellen {#create-custom-service}

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Klicken Sie **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Wählen Sie **[!UICONTROL Neu]** und dann **[!UICONTROL Neuer Service]** aus.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Geben Sie einen **[!UICONTROL Anzeigenamen]** für den Dienst ein. Wählen Sie den **[!UICONTROL Nur API-Benutzer]** [zuvor erstellt](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md) aus.

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >Beachten Sie, dass wir bereits über native Integrationen für beliebte Webinar-Services verfügen.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   Oh ja! Der Service ist jetzt erstellt. Rufen wir nun alle Anmeldeinformationen ab, um Zugriff zu gewähren.

## Anmeldedaten für den API-Zugriff {#credentials-for-api-access}

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. Klicken Sie **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. Klicken Sie **[!UICONTROL Details anzeigen]** für den benutzerdefinierten [!UICONTROL LaunchPoint]-Service, der oben erstellt wurde.

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. Klicken Sie **[!UICONTROL Token abrufen]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. Geben Sie **[!UICONTROL Client-ID]**, **[!UICONTROL Client-Geheimnis]**, **[!UICONTROL Autorisierter Benutzer]** und **[!UICONTROL Token]** an die Person weiter, die für die Herstellung der Verbindung verantwortlich ist.

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>Teilen Sie diese Informationen nicht; sie sind die Hintertür Ihrer Daten. Bewahren Sie es auf!
