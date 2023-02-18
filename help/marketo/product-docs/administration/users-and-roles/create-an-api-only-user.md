---
unique-page-id: 2360207
description: Erstellen eines reinen API-Benutzers - Marketo-Dokumente - Produktdokumentation
title: Erstellen eines reinen API-Benutzers
exl-id: 23c92255-07a8-41c2-b7b8-8e495d135671
source-git-commit: 07ebe804d9888c214f9e1ae246ab80dafad54ea3
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 3%

---

# Erstellen eines reinen API-Benutzers {#create-an-api-only-user}

Wenn Sie die Integration mit Marketo über die [REST-API](https://developers.marketo.com/documentation/rest/), müssen Sie nur einen API-Benutzer erstellen. So geht es.

>[!PREREQUISITES]
>
>[Erstellen einer Benutzerrolle &quot;Nur API&quot;](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

1. Navigieren Sie zum **Admin**-Bereich.

   ![](assets/create-an-api-only-user-1.png)

1. Klicken **Benutzer und Rollen**.

   ![](assets/create-an-api-only-user-2.png)

1. Klicken **Neuen Benutzer einladen**.

   ![](assets/create-an-api-only-user-3.png)

1. Geben Sie eine E-Mail, einen Vornamen und einen Nachnamen für den Benutzer &quot;Nur API&quot;ein. Klicken **Nächste**.

   ![](assets/create-an-api-only-user-4.png)

   >[!TIP]
   >
   >Fügen Sie einen optionalen Grund oder ein Ablaufdatum für den Zugriff hinzu. Für kurzfristige Mitarbeiter eignen sich die Zugriffs-Ablaufdaten.

1. Wählen Sie die **Nur API** Rolle und überprüfen Sie die **Nur API** aktivieren. Klicken **Nächste**.

   ![](assets/create-an-api-only-user-5.png)

1. Klicken **Senden**.

   ![](assets/create-an-api-only-user-6.png)

>[!NOTE]
>
>Im Popup steht: &quot;Eine Einladung ist nicht nur für API erforderlich&quot;, aber das bedeutet nicht, dass Sie etwas falsch gemacht haben. Es bedeutet nur, dass wir die Rolle erstellen, ohne dass eine Einladungs-E-Mail gesendet werden muss.

Dann ja! Erstellen wir nun den benutzerdefinierten Dienst.

>[!MORELIKETHIS]
>
>[Erstellen eines benutzerdefinierten Dienstes zur Verwendung mit der ReST-API](/help/marketo/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.md)
