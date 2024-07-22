---
unique-page-id: 2360207
description: Erstellen eines reinen API-Benutzers - Marketo-Dokumente - Produktdokumentation
title: Erstellen eines reinen API-Benutzers
exl-id: 23c92255-07a8-41c2-b7b8-8e495d135671
feature: Users and Roles
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Erstellen eines reinen API-Benutzers {#create-an-api-only-user}

Wenn Sie die Integration mit Marketo über die [REST-API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} durchführen möchten, müssen Sie nur einen API-Benutzer erstellen. So geht es.

>[!IMPORTANT]
>
>Wenn Sie &quot;Nur API-Benutzer&quot;in einem Abonnement erstellen, das mit Adobe Identity integriert wurde, sind Ihre Schritte anders und [finden Sie hier](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md){target="_blank"}.

>[!PREREQUISITES]
>
>[Erstellen einer reinen API-Benutzerrolle](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/create-an-api-only-user-1.png)

1. Klicken Sie auf **[!UICONTROL Benutzer und Rollen]**.

   ![](assets/create-an-api-only-user-2.png)

1. Klicken Sie auf **[!UICONTROL Neuen Benutzer einladen]**.

   ![](assets/create-an-api-only-user-3.png)

1. Geben Sie eine E-Mail, einen Vornamen und einen Nachnamen für den Benutzer &quot;Nur API&quot;ein. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/create-an-api-only-user-4.png)

   >[!TIP]
   >
   >Fügen Sie einen optionalen Grund oder ein Ablaufdatum für den Zugriff hinzu. Für kurzfristige Mitarbeiter eignen sich die Zugriffs-Ablaufdaten.

1. Wählen Sie die Rolle **[!UICONTROL Nur API]** aus und aktivieren Sie das Kontrollkästchen **[!UICONTROL Nur API]** . Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/create-an-api-only-user-5.png)

1. Klicken Sie auf **[!UICONTROL Senden]**.

   ![](assets/create-an-api-only-user-6.png)

>[!NOTE]
>
>Im Popup steht: &quot;Eine Einladung ist nicht nur für API erforderlich&quot;, aber das bedeutet nicht, dass Sie etwas falsch gemacht haben. Es bedeutet nur, dass wir die Rolle erstellen, ohne dass eine Einladungs-E-Mail gesendet werden muss.

Dann ja! Erstellen wir nun den benutzerdefinierten Dienst.

>[!MORELIKETHIS]
>
>[Erstellen eines benutzerdefinierten Dienstes zur Verwendung mit der REST-API](/help/marketo/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.md){target="_blank"}
