---
unique-page-id: 2360350
description: Erstellen eines benutzerdefinierten Dienstes zur Verwendung mit der ReST-API - Marketing Docs - Produktdokumentation
title: Erstellen eines benutzerdefinierten Dienstes zur Verwendung mit der ReST-API
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---


# Erstellen eines benutzerdefinierten Dienstes zur Verwendung mit der ReST-API {#create-a-custom-service-for-use-with-rest-api}

Wenn Sie die Integration mit Marketo über die ReST-API durchführen möchten, erstellen Sie einen benutzerdefinierten Dienst. So geht es.

>[!PREREQUISITES]
>
>* [Benutzerrolle &quot;Nur API erstellen&quot;](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Nur-API-Benutzer erstellen](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)

>



>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!TIP]
>
>Weitere Informationen zur [ReST-API](http://developers.marketo.com/documentation/rest/) finden Sie in der Entwicklerdokumentation. Wir haben auch die [SOAP-API](http://developers.marketo.com/documentation/soap/), wenn Sie das benötigen.

>[!NOTE]
>
>Sie können keinen benutzerdefinierten Dienst erstellen, wenn Sie die Spark-Ebene von Marketo haben.

## Benutzerspezifischen Dienst erstellen {#create-custom-service}

1. Gehen Sie zu **Admin** und klicken Sie auf **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a38-3a15.png)

1. Klicken Sie unter **Neu** auf **Neuer Dienst**.

   ![](assets/image2014-9-19-10-3a38-3a22.png)

1. Geben Sie einen **Anzeigenamen** für den Dienst ein. Wählen Sie **Nur Benutzer** [Zuvor erstellte](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) aus.

   >[!NOTE]
   >
   >Beachten Sie, dass wir bereits eine native Integration für populäre Webinar-Dienste haben.

   ![](assets/image2014-9-19-10-3a38-3a32.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/image2014-9-19-10-3a39-3a28.png)

   Oh ja! Der Dienst wurde jetzt erstellt. Lassen Sie uns fortfahren und alle Anmeldeinformationen abrufen, um Zugriff zu gewähren.

## Anmeldeinformationen für den API-Zugriff {#credentials-for-api-access}

1. Gehen Sie zu **Admin** und klicken Sie auf **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a42-3a11.png)

1. Klicken Sie für den oben erstellten benutzerdefinierten LaunchPoint-Dienst auf **Ansicht Details**.

   ![](assets/image2014-9-19-10-3a42-3a16.png)

1. Klicken Sie auf **Get Token**.

   ![](assets/image2014-9-19-10-3a42-3a24.png)

1. Stellen Sie die **Client-ID**, **geheimer Clientschlüssel**, **autorisierter Benutzer** und **Token** der Person bereit, die für die Einrichtung der Verbindung zuständig ist.

   ![](assets/image2014-9-19-10-3a42-3a38.png)

>[!CAUTION]
>
>Geben Sie diese Informationen nicht weiter. es ist die Hintertür zu Ihren Daten. Halte es in Sicherheit!
