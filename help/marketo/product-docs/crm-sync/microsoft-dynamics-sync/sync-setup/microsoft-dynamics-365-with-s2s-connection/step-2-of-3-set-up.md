---
unique-page-id: 3571827
description: 'Schritt 2 von 3: Einrichten der Marketo-Lösung mit Server-zu-Server-Verbindung - Marketo-Dokumente - Produktdokumentation'
title: 'Schritt 2 von 3: Einrichten der Marketo-Lösung mit einer Server-zu-Server-Verbindung'
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# Schritt 2 von 3: Einrichten der Marketo-Lösung mit einer Server-zu-Server-Verbindung {#step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s}

>[!PREREQUISITES]
>
>[Schritt 1 von 3: Installieren Sie die Marketo-Lösung mit einer Server-zu-Server-Verbindung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"}

## Erstellen einer Client-Anwendung in [!DNL Azure AD] {#create-client-application-in-azure-ad}

1. Navigieren Sie zu [diesem Microsoft-Artikel](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}.

1. Befolgen Sie alle Schritte. Geben Sie für Schritt 3 einen relevanten Anwendungsnamen ein (z. B. &quot;[!DNL Marketo Integration]„). Wählen Sie unter Unterstützte Kontotypen die Option **Nur Konto in diesem Organisationsverzeichnis** aus.

1. Notieren Sie die Anwendungs-ID (ClientId) und Mandanten-ID. Sie müssen sie später in Marketo eingeben.

1. Erteilen Sie die Zustimmung des Administrators, indem Sie die Schritte [in diesem Artikel) ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}.

1. Generieren Sie ein Client-Geheimnis im Admin Center, indem Sie auf **[!UICONTROL Zertifikate und Geheimnisse]** klicken.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-1.png)

1. Klicken Sie auf **[!UICONTROL Schaltfläche „Neuer geheimer]**&quot;.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-2.png)

1. Geben Sie eine Beschreibung des Client-Geheimnisses ein und klicken Sie auf **[!UICONTROL Hinzufügen]**.

   ![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-3.png)

>[!CAUTION]
>
>Notieren Sie sich den Wert des Client-Geheimnisses (siehe Screenshot unten), da Sie ihn später benötigen werden. Er wird nur einmal angezeigt und kann nicht erneut abgerufen werden.

![](assets/step-2-of-3-set-up-marketo-sync-user-in-dynamics-s2s-4.png)

## Programmbenutzer in Microsoft erstellen {#create-application-user-in-microsoft}

1. Folgen Sie den Schritten unter dem folgenden Link, um [einen Programmbenutzer in Microsoft einzurichten](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/use-single-tenant-server-server-authentication#application-user-creation){target="_blank"}.

   >[!IMPORTANT]
   >
   >* Achten Sie darauf, dem Programmbenutzer beim Gewähren von Berechtigungen die Rolle &quot;Marketo-Benutzersynchronisierung“ zuzuweisen.
   >* Notieren Sie sich die E-Mail-Adresse des Anwendungsbenutzers in der Option [Details anzeigen](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) in Power Platform. Diese E-Mail-Adresse wird beim Einrichten der Verbindung zu MS [!DNL Dynamics] in Marketo als Benutzername verwendet.

## [!DNL Azure AD] mit [!DNL AD FS On-prem] verbunden {#azure-ad-federated-with-ad-fs-on-prem}

Federated [!DNL Azure AD] to [!DNL ADFS Onprem] erfordert die Erstellung einer Heimrealm-Ermittlungsrichtlinie für das jeweilige Programm. Mit dieser Richtlinie leiten [!DNL Azure AD] die Authentifizierungsanfrage an den Verbunddienst weiter. Die Synchronisierung von Passwort-Hashs muss dafür in [!DNL AD Connect] aktiviert sein. Weitere Informationen finden Sie unter [[!DNL OAuth] mit [!DNL ROPC]](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) und [Festlegen einer harten Richtlinie für eine Anwendung](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

Weitere Referenzen [finden Sie hier](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&text=This%20report%20also%20include%20federated,are%20federated%20to%20Azure%20AD.){target="_blank"}.

## Marketo-Lösung konfigurieren {#configure-marketo-solution}

Fast da! Uns bleibt nur noch, die Marketo-Lösung über den neu erstellten Benutzer zu informieren.

1. Gehen Sie zurück zum Abschnitt [!UICONTROL Erweiterte Einstellungen] und klicken Sie auf das ![](assets/image2015-5-13-15-3a49-3a19.png) neben [!UICONTROL Einstellungen] und wählen Sie **[!UICONTROL Marketo Config]**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Wenn &quot;Marketo Config“ im Menü Einstellungen nicht angezeigt wird, aktualisieren Sie die Seite. Wenn dies nicht funktioniert, versuchen Sie erneut, [die Marketo-Lösung zu veröffentlichen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"} oder melden Sie sich ab und wieder an.

1. Klicken Sie auf **[!UICONTROL Standard]**.

   ![](assets/fifteen.png)

1. Klicken Sie im Feld **[!UICONTROL Marketo-Benutzer]** auf die Schaltfläche „Suchen“ und wählen Sie den erstellten Synchronisierungsbenutzer aus.

   ![](assets/sixteen.png)

1. Klicken Sie auf das ![](assets/image2015-3-13-15-3a10-3a11.png) in der rechten unteren Ecke, um die Änderungen zu speichern.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Klicken Sie auf **X** oben rechts, um den Bildschirm zu schließen.

   ![](assets/seventeen.png)

1. Klicken Sie auf das ![](assets/image2015-5-13-15-3a49-3a19-1.png) neben [!UICONTROL Einstellungen] und wählen Sie **[!UICONTROL Lösungen]** aus.

   ![](assets/eighteen.png)

1. Klicken Sie auf **[!UICONTROL Schaltfläche Alle Anpassungen]**.

   ![](assets/nineteen.png)

   >[!NOTE]
   >
   >Wenn Sie ein Upgrade von der einfachen Authentifizierung auf [!DNL OAuth] durchführen, können Sie [diesen Artikel](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md) verwenden, um Ihre Authentifizierung neu zu konfigurieren.

## Bevor Sie mit Schritt 3 fortfahren {#before-proceeding-to-step}

* Wenn Sie die Anzahl der zu synchronisierenden Datensätze einschränken möchten, richten [ jetzt einen benutzerdefinierten Synchronisierungsfilter ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md).
* Führen Sie den Prozess [validate [!DNL Microsoft Dynamics] sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) aus. Es stellt sicher, dass die anfänglichen Setups korrekt ausgeführt wurden.
* Melden Sie sich beim Marketo Sync User in [!DNL Microsoft Dynamics] CRM an.

>[!MORELIKETHIS]
>
>* [Schritt 3 von 3: Marketo-Lösung mit Server-zu-Server-Verbindung verbinden](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-3-of-3-connect.md)
>* [Authentifizierungsmethode  [!DNL Dynamics] Neu konfigurieren](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)
