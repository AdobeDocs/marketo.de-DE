---
description: 'Schritt 3 von 4: Einrichten der Client App auf MS Dynamics - Marketo Docs - Produktdokumentation'
title: 'Schritt 3 von 4: Einrichten der Client App auf MS Dynamics'
source-git-commit: 9ee27e22fec4e0ab85c193be2ea99d3c8b40568b
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---

# Schritt 3 von 4: Einrichten der Client App auf MS Dynamics {#step-3-of-4-set-up-client-app-ms-dynamics-ropc}

>[!PREREQUISITES]
>
>* [Schritt 1 von 4: Installieren Sie die Marketo-Lösung mit Resource Owner Password Control Connection.](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)
>* [Schritt 2 von 4: Einrichten der Marketo-Lösung mit Resource Owner Password Control Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)


1. Navigieren Sie zu https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration.

1. Führen Sie alle Schritte aus. Geben Sie für Schritt 3 einen relevanten Anwendungsnamen ein (z. B. &quot;Marketo Integration&quot;). Wählen Sie unter Unterstützte Kontotypen nur die Option Konto in diesem Organisationsverzeichnis aus.

1. Notieren Sie sich die Anwendungs-ID (ClientId). Sie müssen sie später in Marketo eingeben.

1. Befolgen Sie die Schritte unter [diesem Artikel](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md).

1. Erstellen Sie ein Client-Geheimnis im Admin Center durch Klicken auf **Zertifikate &amp; Geheimnisse**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-1.png)

1. Klicken **Neues Client-Geheimnis**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-2.png)

1. Fügen Sie eine Client-Geheimnisbeschreibung hinzu und klicken Sie auf **Hinzufügen**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-3.png)

   >[!CAUTION]
   >
   >Beachten Sie den Wert Client Secret (siehe Screenshot unten), da Sie ihn später benötigen werden. Es wird nur einmal angezeigt und Sie werden es nicht erneut abrufen können.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-4.png)

## Azure AD Federated mit AD FS On-Premise {#azure-ad-federated-with-ad-fs-on-prem}

Federated Azure AD to ADFS Onprem benötigt die Erstellung einer Home Realm Discovery-Richtlinie für die jeweilige Anwendung. Mit dieser Richtlinie leitet Azure AD die Authentifizierungsanforderung an den Föderierungsdienst weiter. Die Synchronisierung von Passwort-Hash muss hierfür in AD Connect aktiviert werden. Weitere Informationen finden Sie unter [OAuth mit ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) und [Festlegen einer Richtlinie für eine Anwendung](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

Zusätzliche Verweise [finden Sie hier .](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20also%20include%20federated,are%20federated%20to%20Azure%20AD.).

>[!MORELIKETHIS]
>
>* [Schritt 4 von 4: Verbinden der Marketo-Lösung mit der Kennwortsteuerungsverbindung des Ressourceneigentümers](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md)

