---
unique-page-id: 2360350
description: Erstellen eines benutzerdefinierten Dienstes zur Verwendung mit der ReST-API - Marketo Docs - Produktdokumentation
title: Erstellen eines benutzerdefinierten Dienstes zur Verwendung mit der ReST-API
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 5%

---

# Erstellen eines benutzerdefinierten Dienstes zur Verwendung mit der ReST-API {#create-a-custom-service-for-use-with-rest-api}

Wenn Sie die Integration mit Marketo über die ReST-API durchführen möchten, möchten Sie einen benutzerdefinierten Dienst erstellen. So geht es.

>[!PREREQUISITES]
>
>* [Erstellen einer Benutzerrolle &quot;Nur API&quot;](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Erstellen eines reinen API-Benutzers](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)
>

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!TIP]
>
>Weitere Informationen finden Sie in der Entwicklerdokumentation . [ReST-API](https://developers.marketo.com/documentation/rest/). Wir haben auch die [SOAP-API](https://developers.marketo.com/documentation/soap/) wenn das das ist, was du brauchst.

## Benutzerspezifischen Dienst erstellen {#create-custom-service}

1. Navigieren Sie zum **[!UICONTROL Admin]**-Bereich.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Klicks **LaunchPoint**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Auswählen **[!UICONTROL Neu]** und dann **[!UICONTROL Neuer Dienst]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Geben Sie einen **[!UICONTROL Anzeigename]** für den Dienst. Wählen Sie die **[!UICONTROL Nur API-Benutzer]** [zuvor erstellt](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >Beachten Sie, dass wir bereits eine native Integration für beliebte Webinar-Dienste haben.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   Oh ja! Der Dienst wird jetzt erstellt. Lassen Sie uns fortfahren und alle Anmeldedaten abrufen, um Zugriff bereitzustellen.

## Anmeldedaten für den API-Zugriff {#credentials-for-api-access}

1. Navigieren Sie zum **[!UICONTROL Admin]**-Bereich.

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. Klicks **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. Klicks **[!UICONTROL Details anzeigen]** für die benutzerdefinierte [!UICONTROL LaunchPoint] -Dienst, der oben erstellt wurde.

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. Klicks **[!UICONTROL Token abrufen]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. Stellen Sie die **[!UICONTROL Client-ID]**, **[!UICONTROL Client Secret]**, **[!UICONTROL Autorisierter Benutzer]**, und **[!UICONTROL Token]** an die Person, die für die Herstellung der Verbindung verantwortlich ist.

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>Geben Sie diese Informationen nicht weiter, sondern sind die Hintertür Ihrer Daten. Halte es sicher!
