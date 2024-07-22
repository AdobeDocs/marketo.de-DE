---
unique-page-id: 2360350
description: Erstellen eines benutzerdefinierten Dienstes zur Verwendung mit der ReST-API - Marketo Docs - Produktdokumentation
title: Erstellen eines benutzerdefinierten Dienstes zur Verwendung mit der ReST-API
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Erstellen eines benutzerdefinierten Dienstes zur Verwendung mit der ReST-API {#create-a-custom-service-for-use-with-rest-api}

Wenn Sie die Integration mit Marketo über die ReST-API durchführen möchten, möchten Sie einen benutzerdefinierten Dienst erstellen. So geht es.

>[!PREREQUISITES]
>
>* [Erstellen einer reinen API-Benutzerrolle](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Erstellen eines reinen API-Benutzers](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)
>

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!TIP]
>
>Weitere Informationen zur [REST-API](https://developer.adobe.com/marketo-apis/) finden Sie in der Entwicklerdokumentation . Wir verfügen auch über die [SOAP-API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/soap/soap-api) , wenn Sie dies benötigen.

## Benutzerspezifischen Dienst erstellen {#create-custom-service}

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Klicken Sie auf **LaunchPoint**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Wählen Sie **[!UICONTROL Neu]** und dann **[!UICONTROL Neuer Dienst]** aus.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Geben Sie einen **[!UICONTROL Anzeigenamen]** für den Dienst ein. Wählen Sie den zuvor erstellten **[!UICONTROL Nur API-Benutzer]** [ aus.](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >Beachten Sie, dass wir bereits eine native Integration für beliebte Webinar-Dienste haben.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   Oh ja! Der Dienst wird jetzt erstellt. Lassen Sie uns fortfahren und alle Anmeldedaten abrufen, um Zugriff bereitzustellen.

## Anmeldedaten für den API-Zugriff {#credentials-for-api-access}

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. Klicken Sie auf **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. Klicken Sie für den oben erstellten benutzerdefinierten [!UICONTROL LaunchPoint]-Dienst auf **[!UICONTROL Details anzeigen]** .

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. Klicken Sie auf **[!UICONTROL Token abrufen]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. Stellen Sie die **[!UICONTROL Client-ID]**, das **[!UICONTROL Client-Geheimnis]**, den **[!UICONTROL autorisierten Benutzer]** und den **[!UICONTROL Token]** der Person bereit, die für die Herstellung der Verbindung verantwortlich ist.

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>Geben Sie diese Informationen nicht weiter, sondern sind die Hintertür Ihrer Daten. Halte es sicher!
