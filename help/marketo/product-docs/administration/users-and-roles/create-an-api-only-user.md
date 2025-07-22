---
unique-page-id: 2360207
description: Nur API-Benutzer erstellen - Marketo-Dokumente - Produktdokumentation
title: Nur API-Benutzer erstellen
exl-id: 23c92255-07a8-41c2-b7b8-8e495d135671
feature: Users and Roles
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 3%

---

# Nur API-Benutzer erstellen {#create-an-api-only-user}

Wenn Sie eine Integration mit Marketo über die [REST-API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} durchführen möchten, müssen Sie nur einen API-Benutzer erstellen. So geht&#39;s.

>[!IMPORTANT]
>
>Wenn Sie Benutzende nur mit einer API in einem Abonnement erstellen, das in Adobe Identity integriert wurde, sind Ihre Schritte anders und [finden Sie hier](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md){target="_blank"}.

>[!PREREQUISITES]
>
>[Erstellen einer Benutzerrolle nur für API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/create-an-api-only-user-1.png)

1. Klicken Sie auf **[!UICONTROL Benutzer und Rollen]**.

   ![](assets/create-an-api-only-user-2.png)

1. Klicken Sie **[!UICONTROL Neuen Benutzer einladen]**.

   ![](assets/create-an-api-only-user-3.png)

1. Geben Sie eine E-Mail-Adresse, einen Vor- und einen Nachnamen nur für den API-Benutzer ein. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/create-an-api-only-user-4.png)

   >[!TIP]
   >
   >Fügen Sie einen optionalen [!UICONTROL Grund] oder ein [!UICONTROL Zugriffsgültigkeitsdatum] hinzu. Das Ablaufdatum des Zugriffs ist für kurzfristige Mitarbeiter praktisch.

1. Wählen Sie die Rolle **[!UICONTROL Nur API]** aus und aktivieren Sie das Kontrollkästchen **[!UICONTROL Nur API]**. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/create-an-api-only-user-5.png)

1. Klicken Sie auf **[!UICONTROL Senden]**.

   ![](assets/create-an-api-only-user-6.png)

>[!NOTE]
>
>Im Popup-Fenster steht: „Eine Einladung ist nicht nur für die API erforderlich“, aber das bedeutet nicht, dass Sie etwas falsch gemacht haben. Das bedeutet nur, dass wir die Rolle erstellen, ohne dass eine Einladungs-E-Mail gesendet werden muss.

Gut dann! Erstellen wir nun den benutzerdefinierten Service.

>[!MORELIKETHIS]
>
>[Erstellen eines benutzerdefinierten Services zur Verwendung mit der REST-API](/help/marketo/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.md){target="_blank"}
