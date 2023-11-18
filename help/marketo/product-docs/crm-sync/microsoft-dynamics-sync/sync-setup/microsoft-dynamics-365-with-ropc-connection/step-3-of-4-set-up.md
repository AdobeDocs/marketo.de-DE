---
description: 'Schritt 3 von 4: Einrichten der Client App auf MS Dynamics - Marketo Docs - Produktdokumentation'
title: 'Schritt 3 von 4: Einrichten der Client App auf MS Dynamics'
exl-id: e7897174-3303-4c3b-8832-3e10f34fca96
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Schritt 3 von 4: Einrichten der Client App auf MS Dynamics {#step-3-of-4-set-up-client-app-ms-dynamics-ropc}

>[!PREREQUISITES]
>
>* [Schritt 1 von 4: Installieren der Marketo-Lösung mit Resource Owner Password Control Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}
>* [Schritt 2 von 4: Einrichten der Marketo-Lösung mit Resource Owner Password Control Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}

1. Navigieren Sie dazu [Microsoft-Artikel](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}.

1. Führen Sie alle Schritte aus. Geben Sie für Schritt 3 einen relevanten Anwendungsnamen ein (z. B. &quot;Marketo Integration&quot;). Wählen Sie unter Unterstützte Kontotypen nur die Option Konto in diesem Organisationsverzeichnis aus.

1. Notieren Sie sich die Anwendungs-ID (ClientId). Sie müssen sie später in Marketo eingeben.

1. Befolgen Sie die Schritte unter [diesem Artikel](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}.

1. Erstellen Sie ein Client-Geheimnis im Admin Center durch Klicken auf **[!UICONTROL Zertifikate &amp; Geheimnisse]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-1.png)

1. Klicks **[!UICONTROL Neues Client-Geheimnis]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-2.png)

1. Fügen Sie eine Client-Geheimnisbeschreibung hinzu und klicken Sie auf **[!UICONTROL Hinzufügen]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-3.png)

   >[!CAUTION]
   >
   >Beachten Sie den Wert Client Secret (siehe Screenshot unten), da Sie ihn später benötigen werden. Es wird nur einmal angezeigt und Sie werden es nicht erneut abrufen können.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-4.png)

## Azure AD Federated mit AD FS On-Premise {#azure-ad-federated-with-ad-fs-on-prem}

Federated Azure AD to ADFS Onprem benötigt die Erstellung einer Home Realm Discovery-Richtlinie für die jeweilige Anwendung. Mit dieser Richtlinie leitet Azure AD die Authentifizierungsanforderung an den Föderierungsdienst weiter. Die Synchronisierung von Passwort-Hash muss hierfür in AD Connect aktiviert werden. Weitere Informationen finden Sie unter [OAuth mit ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc){target="_blank"} and [Set an hrd policy for an application](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application){target="_blank"}.

Zusätzliche Verweise [finden Sie hier .](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20also%20include%20federated,are%20federated%20to%20Azure%20AD.){target="_blank"}.

## Bevor Sie mit Schritt 4 fortfahren {#before-proceeding-to-step-4}

* Wenn Sie die Anzahl der zu synchronisierenden Datensätze einschränken möchten, [Einrichten eines benutzerdefinierten Synchronisierungsfilters](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} jetzt.
* Führen Sie die [Überprüfen der Synchronisierung mit Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} -Prozess. Es wird überprüft, ob Ihre ersten Setups ordnungsgemäß durchgeführt wurden.
* Melden Sie sich beim Marketo Sync User in Microsoft Dynamics CRM an.

>[!MORELIKETHIS]
>
>* [Schritt 4 von 4: Verbinden der Marketo-Lösung mit der Resource Owner Password Control Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md){target="_blank"}
