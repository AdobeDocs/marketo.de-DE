---
description: Schritt 3 von 4 - Einrichten der Client-App auf MS [!DNL Dynamics] - Marketo-Dokumente - Produktdokumentation
title: 'Schritt 3 von 4: Einrichten der Client-App auf MS [!DNL Dynamics]'
exl-id: e7897174-3303-4c3b-8832-3e10f34fca96
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Schritt 3 von 4: Einrichten der Client-App auf MS [!DNL Dynamics] {#step-3-of-4-set-up-client-app-ms-dynamics-ropc}

>[!PREREQUISITES]
>
>* [Schritt 1 von 4: Installieren Sie die Marketo-Lösung mit der Kennwortsteuerungsverbindung des Ressourceneigentümers](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}
>* [Schritt 2 von 4: Richten Sie die Marketo-Lösung mit der Kennwortsteuerungsverbindung für Ressourcenbesitzer ein](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}

1. Navigieren Sie zu diesem [Microsoft-Artikel](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}.

1. Befolgen Sie alle Schritte. Geben Sie für Schritt 3 einen relevanten Anwendungsnamen ein (z. B. &quot;[!DNL Marketo Integration]„). Wählen Sie unter Unterstützte Kontotypen die Option Konto nur in diesem Organisationsverzeichnis aus.

1. Notieren Sie sich die Anwendungs-ID (ClientId). Sie müssen sie später in Marketo eingeben.

1. Erteilen Sie die Zustimmung des Administrators, indem Sie die Schritte in [diesem Artikel) ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}.

1. Generieren Sie ein Client-Geheimnis im Admin Center, indem Sie auf **[!UICONTROL Zertifikate und Geheimnisse]** klicken.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-1.png)

1. Klicken Sie **[!UICONTROL Neues Client-Geheimnis]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-2.png)

1. Fügen Sie eine Beschreibung des Client-Geheimnisses hinzu und klicken Sie auf **[!UICONTROL Hinzufügen]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-3.png)

   >[!CAUTION]
   >
   >Notieren Sie sich den Wert des Client-Geheimnisses (siehe Screenshot unten), da Sie ihn später benötigen werden. Er wird nur einmal angezeigt und kann nicht erneut abgerufen werden.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-4.png)

## [!DNL Azure AD] mit [!DNL AD FS On-prem] verbunden {#azure-ad-federated-with-ad-fs-on-prem}

Federated [!DNL Azure] AD für [!DNL ADFS Onprem] erfordert die Erstellung einer Heimrealm-Ermittlungsrichtlinie für das jeweilige Programm. Mit dieser Richtlinie leitet [!DNL Azure] AD die Authentifizierungsanfrage an den Verbunddienst weiter. Die Synchronisierung von Passwort-Hashs muss dafür in [!DNL AD Connect] aktiviert sein. Weitere Informationen finden Sie unter [[!DNL OAuth] mit [!DNL ROPC]](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) und [Festlegen einer harten Richtlinie für eine Anwendung](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

Weitere Referenzen [finden Sie hier](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&text=This%20report%20also%20include%20federated,are%20federated%20to%20Azure%20AD.){target="_blank"}.

## Bevor Sie mit Schritt 4 fortfahren {#before-proceeding-to-step-4}

* Wenn Sie die Anzahl der zu synchronisierenden Datensätze einschränken möchten, richten [ jetzt einen benutzerdefinierten Synchronisierungsfilter ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md).
* Führen Sie den Prozess [validate [!DNL Microsoft Dynamics] sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) aus. Es stellt sicher, dass die anfänglichen Setups korrekt ausgeführt wurden.
* Melden Sie sich beim Marketo Sync User in [!DNL Microsoft Dynamics] CRM an.

>[!MORELIKETHIS]
>
>* [Schritt 4 von 4: Verbinden der Marketo-Lösung mit der Kennwortsteuerungsverbindung des Ressourceneigentümers](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md){target="_blank"}
