---
description: Einrichten der Microsoft Dynamics CRM-App für Online - Marketo Docs - Produktdokumentation
title: Einrichten der Microsoft Dynamics CRM-App für Online
exl-id: ec3123c9-e484-4736-9831-9559cc393bd9
source-git-commit: 4283f1b6936316f3053543e06e7eaee45a7f2436
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Einrichten der Microsoft Dynamics CRM-App für Online {#set-up-microsoft-dynamics-crm-app-for-online}

## Einrichten von {#set-up}

1. Navigieren Sie zu https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration.

1. Führen Sie alle Schritte aus. Geben Sie für Schritt 3 einen relevanten Anwendungsnamen ein (z. B. &quot;Marketo Integration&quot;). Wählen Sie unter Unterstützte Kontotypen nur die Option Konto in diesem Organisationsverzeichnis aus.

1. Notieren Sie sich die Anwendungs-ID (ClientId). Sie müssen sie später in Marketo eingeben.

1. Erteilen Sie die Admin-Zustimmung, indem Sie die Schritte in [diesem Artikel](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/set-up-oauth-authentication-for-dynamics/grant-consent-for-client-id-and-app-registration.md) ausführen.

1. Generieren Sie ein Client-Geheimnis im Admin Center, indem Sie auf **Zertifikate und Geheimnisse** klicken.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-1.png)

1. Klicken Sie auf **Neues Client-Geheimnis**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-2.png)

1. Fügen Sie eine Client-Geheimnisbeschreibung hinzu und klicken Sie auf **Hinzufügen**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-3.png)

   >[!CAUTION]
   >
   >Beachten Sie den Wert Client Secret (siehe Screenshot unten), da Sie ihn später benötigen werden. Es wird nur einmal angezeigt und Sie werden es nicht erneut abrufen können.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-4.png)

Marketo authentifiziert sich bei Azure AD mit OAuth mit grant_type Resource Owner Password Credentials( ROPC). Für dieses Szenario muss eine Home Realm Discovery-Richtlinie für die jeweilige Anwendung erstellt werden. Mit dieser Richtlinie leitet Azure AD die Authentifizierungsanforderung an den Föderierungsdienst weiter. Die Synchronisierung von Passwort-Hash muss hierfür in AD Connect aktiviert werden. Weitere Informationen finden Sie unter [OAuth mit ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) und [Festlegen einer Hotline für eine Anwendung](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

Weitere Verweise [finden Sie hier](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20also%20include%20federated,are%20federated%20to%20Azure%20AD.).

Wenn Sie fertig sind, ist es an der Zeit, **Geben Sie die Dynamics CRM-generierte Client-ID und den geheimen Schlüssel in Marketo** ein.

## Geben Sie die vom Dynamics CRM generierte Client-ID und den geheimen Schlüssel in Marketo ein {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}.

Die folgenden Schritte gelten für Online-Versionen _und_ On-Premise.

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-5.png)

1. Klicken Sie auf **Microsoft Dynamics**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-6.png)

1. Klicken Sie auf **Synchronisierung deaktivieren**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-7.png)

1. Klicken Sie neben den Anmeldedaten auf **Bearbeiten**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-8.png)

1. Geben Sie die **Client-ID** und das **Client-Geheimnis** ein, die Sie zuvor abgerufen haben, und drücken Sie **Speichern**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-9.png)

1. Klicken Sie auf **Einrichtung für die Überprüfung der Synchronisierung**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-10.png)

1. Klicken Sie auf **Next**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-11.png)

1. Sie sollten alle grünen Häkchen sehen. Klicken Sie auf **Close**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-12.png)

   >[!NOTE]
   >
   >Wenn unter Ihren grünen Häkchen ein rotes X angezeigt wird, finden Sie unter [diesen Artikel](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) weitere Fehlerbehebungsoptionen.

1. Klicken Sie auf **Synchronisierung aktivieren**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-online-13.png)

Und das ist es!
