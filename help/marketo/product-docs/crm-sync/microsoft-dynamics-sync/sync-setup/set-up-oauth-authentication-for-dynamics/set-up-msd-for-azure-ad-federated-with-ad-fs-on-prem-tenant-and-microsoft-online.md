---
description: Einrichten von MSD für Azure AD Federated mit AD FS On-Premise, Mandant und Microsoft Online - Marketo Docs - Produktdokumentation
title: Einrichten von MSD für Azure AD Federated mit AD FS On-Premise, Mandant und Microsoft Online
exl-id: b6c10048-d27e-4135-beef-232deddc2984
source-git-commit: 91ce0914755b578c896996fae1805022cb11c438
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Einrichten von MSD für Azure AD Federated mit AD FS On-Premise, Mandant und Microsoft Online {#set-up-msd-for-azure-ad-federated-with-ad-fs-on-prem-tenant-and-microsoft-online}

## Einrichten der Microsoft Dynamics CRM-App {#set-up-microsoft-dynamics-crm-app}

1. Navigieren Sie zu https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration.

1. Führen Sie alle Schritte aus. Geben Sie für Schritt 3 einen relevanten Anwendungsnamen ein (z. B. &quot;Marketo Integration&quot;). Wählen Sie unter Unterstützte Kontotypen nur die Option Konto in diesem Organisationsverzeichnis aus.

1. Notieren Sie sich die Anwendungs-ID (ClientId). Sie müssen sie später in Marketo eingeben.

1. Befolgen Sie die Schritte unter [diesem Artikel](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md).

1. Erstellen Sie ein Client-Geheimnis im Admin Center durch Klicken auf **Zertifikate &amp; Geheimnisse**.

   ![](assets/set-up-msd-for-azure-ad-federated-1.png)

1. Klicken **Neues Client-Geheimnis**.

   ![](assets/set-up-msd-for-azure-ad-federated-2.png)

1. Fügen Sie eine Client-Geheimnisbeschreibung hinzu und klicken Sie auf **Hinzufügen**.

   ![](assets/set-up-msd-for-azure-ad-federated-3.png)

   >[!CAUTION]
   >
   >Beachten Sie den Wert Client Secret (siehe Screenshot unten), da Sie ihn später benötigen werden. Es wird nur einmal angezeigt und Sie werden es nicht erneut abrufen können.

   ![](assets/set-up-msd-for-azure-ad-federated-4.png)

Marketo authentifiziert sich bei Azure AD mit OAuth mit grant_type Resource Owner Password Credentials( ROPC). Für dieses Szenario muss eine Home Realm Discovery-Richtlinie für die jeweilige Anwendung erstellt werden. Mit dieser Richtlinie leitet Azure AD die Authentifizierungsanforderung an den Föderierungsdienst weiter. Die Synchronisierung von Passwort-Hash muss hierfür in AD Connect aktiviert werden. Weitere Informationen finden Sie unter [OAuth mit ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) und [Festlegen einer Richtlinie für eine Anwendung](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

Zusätzliche Verweise [finden Sie hier .](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20also%20include%20federated,are%20federated%20to%20Azure%20AD.).

Wenn du fertig bist, ist es Zeit, **Geben Sie die vom Dynamics CRM generierte Client-ID und den geheimen Schlüssel in Marketo ein.**.

## Geben Sie die vom Dynamics CRM generierte Client-ID und den geheimen Schlüssel in Marketo ein. {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/set-up-msd-for-azure-ad-federated-5.png)

1. Klicken **Microsoft Dynamics**.

   ![](assets/set-up-msd-for-azure-ad-federated-6.png)

1. Klicken **Synchronisierung deaktivieren**.

   ![](assets/set-up-msd-for-azure-ad-federated-7.png)

1. Klicken Sie neben den Anmeldedaten auf **Bearbeiten**.

   ![](assets/set-up-msd-for-azure-ad-federated-8.png)

1. Geben Sie die **Client-ID** und **Client Secret** Sie haben zuvor abgerufen und drücken **Speichern**.

   ![](assets/set-up-msd-for-azure-ad-federated-9.png)

1. Klicken **Überprüfen der Synchronisierungseinrichtung**.

   ![](assets/set-up-msd-for-azure-ad-federated-10.png)

1. Klicken **Nächste**.

   ![](assets/set-up-msd-for-azure-ad-federated-11.png)

1. Sie sollten alle grünen Häkchen sehen. Klicken **Schließen**.

   ![](assets/set-up-msd-for-azure-ad-federated-12.png)

   >[!NOTE]
   >
   >Wenn unter Ihren grünen Häkchen ein rotes X angezeigt wird, lesen Sie [diesem Artikel](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) für Optionen zur Fehlerbehebung.

1. Klicken **Synchronisierung aktivieren**.

   ![](assets/set-up-msd-for-azure-ad-federated-13.png)

Und das ist es!
