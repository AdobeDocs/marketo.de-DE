---
unique-page-id: 3571827
description: 'Schritt 2 von 3: Einrichten der Marketo-Lösung mit Server-zu-Server-Verbindung - Marketo Docs - Produktdokumentation'
title: 'Schritt 2 von 3: Einrichten der Marketo-Lösung mit Server-zu-Server-Verbindung'
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Schritt 2 von 3: Einrichten der Marketo-Lösung mit Server-zu-Server-Verbindung {#step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s}

>[!PREREQUISITES]
>
>[Schritt 1 von 3: Installieren der Marketo-Lösung mit Server-zu-Server-Verbindung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"}

## Erstellen einer Client-Anwendung in Azure AD {#create-client-application-in-azure-ad}

1. Navigieren Sie zu [diesem Microsoft-Artikel](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}.

1. Führen Sie alle Schritte aus. Geben Sie für Schritt 3 einen relevanten Anwendungsnamen ein (z. B. &quot;Marketo Integration&quot;). Wählen Sie unter &quot;Unterstützte Kontotypen&quot;die Option **Nur Konto in diesem Organisationsverzeichnis**.

1. Notieren Sie sich die Anwendungs-ID (ClientId) und die Mandantenkennung. Sie müssen sie später in Marketo eingeben.

1. Erteilen Sie die Admin-Zustimmung, indem Sie die Schritte [in diesem Artikel](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"} befolgen.

1. Generieren Sie ein Client-Geheimnis im Admin Center, indem Sie auf **[!UICONTROL Zertifikate und Geheimnisse]** klicken.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-1.png)

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Neues Client-Geheimnis]** .

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-2.png)

1. Geben Sie eine Client-Geheimbeschreibung ein und klicken Sie auf **[!UICONTROL Hinzufügen]**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-3.png)

>[!CAUTION]
>
>Beachten Sie den Wert Client Secret (siehe Screenshot unten), da Sie ihn später benötigen werden. Es wird nur einmal angezeigt und Sie werden es nicht erneut abrufen können.

![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-4.png)

## Anwendungsbenutzer in Microsoft erstellen {#create-application-user-in-microsoft}

1. Führen Sie die folgenden Schritte aus, um [einen Anwendungsbenutzer in Microsoft einzurichten](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/use-single-tenant-server-server-authentication#application-user-creation){target="_blank"}.

   >[!IMPORTANT]
   >
   >* Achten Sie beim Gewähren von Berechtigungen für den Anwendungsbenutzer darauf, diese der &quot;Benutzerrolle für Marketo-Synchronisierung&quot;zuzuweisen.
   >* Notieren Sie die E-Mail-Adresse des Anwendungsbenutzers über die Option [Details anzeigen](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user){target="_blank"} in Power Platform. Diese E-Mail-Adresse wird beim Einrichten der Verbindung zu MS Dynamics in Marketo als Benutzername verwendet.
   >* Alle vom Synchronisierungsbenutzer in Ihrem CRM-System vorgenommenen Aktualisierungen werden **nicht** mit Marketo synchronisiert.

## Azure AD Federated mit AD FS On-Premise {#azure-ad-federated-with-ad-fs-on-prem}

Federated Azure AD to ADFS Onprem benötigt die Erstellung einer Home Realm Discovery-Richtlinie für die jeweilige Anwendung. Mit dieser Richtlinie leitet Azure AD die Authentifizierungsanforderung an den Föderierungsdienst weiter. Die Synchronisierung von Passwort-Hash muss hierfür in AD Connect aktiviert werden. Weitere Informationen finden Sie unter [OAuth mit ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc){target="_blank"} und [Festlegen einer RT-Richtlinie für eine Anwendung](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application){target="_blank"}.

Weitere Verweise [finden Sie hier](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20also%20include%20federated,are%20federated%20to%20Azure%20AD.){target="_blank"}.

## Konfigurieren der Marketo-Lösung {#configure-marketo-solution}

Fast da! Wir haben nur noch die Möglichkeit, Marketo Solution über den neu erstellten Benutzer zu informieren.

1. Gehen Sie zurück zum Abschnitt &quot;Erweiterte Einstellungen&quot;, klicken Sie auf das Symbol &quot;![](assets/image2015-5-13-15-3a49-3a19.png)&quot;neben &quot;Einstellungen&quot;und wählen Sie &quot;**[!UICONTROL Marketo-Konfiguration]**&quot;.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Wenn Sie im Einstellungsmenü &quot;Marketo-Konfiguration&quot;nicht sehen, aktualisieren Sie die Seite. Wenn dies nicht funktioniert, versuchen Sie, die Marketo-Lösung ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"} erneut zu veröffentlichen oder melden Sie sich ab und wieder an.[

1. Klicken Sie auf **[!UICONTROL Standard]**.

   ![](assets/fifteen.png)

1. Klicken Sie auf die Suchschaltfläche im Feld **[!UICONTROL Marketo-Benutzer]** und wählen Sie den erstellten Synchronisierungsbenutzer aus.

   ![](assets/sixteen.png)

1. Klicken Sie unten rechts auf das Symbol &quot;![](assets/image2015-3-13-15-3a10-3a11.png)&quot;, um die Änderungen zu speichern.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Klicken Sie oben rechts auf den **X** , um den Bildschirm zu schließen.

   ![](assets/seventeen.png)

1. Klicken Sie auf das Symbol &quot;![](assets/image2015-5-13-15-3a49-3a19-1.png)&quot;neben &quot;Einstellungen&quot;und wählen Sie &quot;**[!UICONTROL Lösungen]**&quot;.

   ![](assets/eighteen.png)

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Alle Anpassungen der Publish]** .

   ![](assets/nineteen.png)

   >[!NOTE]
   >
   >Wenn Sie von der einfachen Authentifizierung auf OAuth aktualisieren, können Sie [diesen Artikel](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"} verwenden, um Ihre Authentifizierung neu zu konfigurieren.

## Bevor Sie mit Schritt 3 fortfahren {#before-proceeding-to-step}

* Wenn Sie die Anzahl der synchronisierten Datensätze beschränken möchten, richten Sie [jetzt einen benutzerdefinierten Synchronisierungsfilter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} ein.
* Führen Sie den Prozess [Microsoft Dynamics-Synchronisation überprüfen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} aus. Es wird überprüft, ob Ihre ersten Setups ordnungsgemäß durchgeführt wurden.
* Melden Sie sich beim Marketo Sync User in Microsoft Dynamics CRM an.

>[!MORELIKETHIS]
>
>* [Schritt 3 von 3: Verbinden der Marketo-Lösung mit der Server-Verbindung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-3-of-3-connect.md){target="_blank"}
>* [Dynamics-Authentifizierungsmethode neu konfigurieren](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md){target="_blank"}
