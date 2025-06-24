---
unique-page-id: 2360356
description: Hinzufügen von Single Sign-on zu einem Portal - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen von Single Sign-On zu einem Portal
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
feature: Administration
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# Hinzufügen von Single Sign-On zu einem Portal {#add-single-sign-on-to-a-portal}

Wenn Sie über einen Verzeichnisdienst verfügen, der Benutzer authentifiziert, können Sie das einmalige Anmelden (SSO) bei Marketo zulassen. Wir unterstützen diese Funktion mit [!DNL Security Assertion Markup Language] (SAML) Version 2.0 und höher.

Marketo fungiert als SAML Service Provider (SP) und ist zur Benutzerauthentifizierung auf einen externen Identitätsanbieter (External Identity Provider, ID) angewiesen.

Sobald SSO aktiviert ist, kann der IdP die Anmeldeinformationen eines Benutzers überprüfen. Wenn eine Benutzerin oder ein Benutzer die Marketo-Software verwenden möchte, sendet der IdP eine signierte SAML-Nachricht an Marketo und fungiert als SP. Diese Meldung sichert Marketo zu, dass der Benutzer berechtigt ist, die Marketo-Software zu verwenden.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!IMPORTANT]
>
>Dies gilt nicht für Abonnements, die in Adobe Identity integriert wurden. Für Abonnements, die in Adobe Identity integriert sind, wird Single Sign-On auf Adobe-Organisationsebene in Adobe Admin Console eingerichtet. Adobe Admin Console unterstützt derzeit nur SP-initiierte . [Weitere Informationen finden Sie hier](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

>[!NOTE]
>
>Benutzt du [!DNL Microsoft Azure]? Sehen Sie sich das [Integrations-Tutorial](https://learn.microsoft.com/en-us/entra/identity/saas-apps/marketo-tutorial){target="_blank"} an. Zu Ihrer Information: In Schritt 5c des Tutorials gibt es einen Tippfehler. Bitte den Relaisstatus auf `https://<munchkinid>.mktoweb.com` setzen, **_nicht_** `https://<munchkinid>.marketo.com`.

## So senden Sie die Anfrage {#how-to-send-the-request}

* Senden Sie die SSO-Anfrage, die eine SAML-Antwort ist, an `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* als Zielgruppen-URL des SP. Verwenden von `http://saml.marketo.com/sp`
* Wenn Sie das Attribut SPNameQualifier verwenden, legen Sie das Element NameID für Subject auf `http://saml.marketo.com/sp` fest
* Wenn Sie mehrere Marketo-Abonnements mit demselben SSO-Provider verbinden, können Sie für jede Marketo-Untergruppe eindeutige SP-URLs im Format `http://saml.marketo.com/sp/<munchkin_id>` verwenden

>[!NOTE]
>
>Marketo unterstützt nur vom Identitätsanbieter initiierte (auch als „IdP-initiiert“ bezeichnet), bei denen der Benutzer zuerst die IdP-Anmeldeseite startet, sich authentifiziert und dann zu „Meine Marketo&quot; navigiert. Wenn Ihr Marketo-Abonnement in die Admin Console verschoben wurde, unterstützt Adobe Admin Console derzeit nur vom Dienstleister initiierte (auch als SP-initiiert bezeichnet). Möglicherweise wurde Ihr SSO-Erlebnis geändert.

## Zusätzliche Hinweise {#additional-notes}

* **Synchronisierungszeit** - Bei einem neuen Benutzer dauert es etwa 10 Minuten, bis eine erste SSO-Anfrage verarbeitet wird.
* **Benutzerbereitstellung** - Benutzer werden manuell von Marketo bereitgestellt.
* **Autorisierung** - Benutzerberechtigungen werden in Marketo verwaltet.
* **OAuth-Unterstützung** - Marketo unterstützt derzeit nicht OAuth.
* **Automatische Benutzerausbreitung** - Wird auch als „Just-in-time-Bereitstellung“ bezeichnet. Dies ist der Fall, wenn die erste SAML-Anmeldung eines Benutzers den Benutzer in der Web-Anwendung erstellen kann, auf die er zugreift (z. B. Marketo), und keine manuelle Verwaltungsaktion erforderlich ist. Dies wird derzeit von Marketo nicht unterstützt.
* **Encryption** - Marketo unterstützt derzeit keine Verschlüsselung.

>[!NOTE]
>
>Stellen Sie vor dem Start Ihr Identity Provider-Zertifikat im X.509-Format und in den Erweiterungen .crt, .der oder .cer bereit.

## SAML-Einstellungen aktualisieren {#update-saml-settings}

SSO ist standardmäßig deaktiviert. Führen Sie diese Schritte aus, um SAML zu aktivieren und zu konfigurieren.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/add-single-sign-on-to-a-portal-1.png)

1. Klicken Sie **[!UICONTROL Single Sign-On]**.

   ![](assets/add-single-sign-on-to-a-portal-2.png)

   >[!NOTE]
   >
   >Wenn „Single Sign **[!UICONTROL unter „Admin]** nicht angezeigt wird **[!UICONTROL wenden Sie]** an den [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. Klicken Sie **[!UICONTROL Abschnitt „SAML]** Einstellungen“ auf **[!UICONTROL Bearbeiten]**.

   ![](assets/add-single-sign-on-to-a-portal-3.png)

1. Ändern Sie **[!UICONTROL SAML Single Sign-On]** in **[!UICONTROL Aktiviert]**.

   ![](assets/add-single-sign-on-to-a-portal-4.png)

1. Geben Sie Ihre **[!UICONTROL Aussteller-ID]**, **[!UICONTROL Entitäts-ID]**, wählen Sie den **[!UICONTROL Benutzer-ID-Speicherort]** aus und klicken Sie dann auf **[!UICONTROL Durchsuchen]**.

   ![](assets/add-single-sign-on-to-a-portal-5.png)

1. Wählen Sie Ihre **[!UICONTROL Identity Provider-Zertifikat]**-Datei aus.

   ![](assets/add-single-sign-on-to-a-portal-6.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/add-single-sign-on-to-a-portal-7.png)

## Aktualisieren der Einstellungen der Umleitungsseite {#update-redirect-page-settings}

1. Klicken Sie **[!UICONTROL Abschnitt „Seiten]**&quot; auf **[!UICONTROL Bearbeiten]**.

   ![](assets/add-single-sign-on-to-a-portal-8.png)

   >[!NOTE]
   >
   >Kunden, die eine universelle ID zusammen mit SSO verwenden, müssen die Anmelde-URL des Identitätsanbieters im Feld **[!UICONTROL Anmelde-URL]** eingeben.

1. Geben Sie eine **[!UICONTROL Abmelde-URL]** ein. Dies ist die URL, zu der der Benutzer weitergeleitet werden soll, wenn er sich von Marketo abmeldet.

   ![](assets/add-single-sign-on-to-a-portal-9.png)

1. Geben Sie eine **[!UICONTROL Fehler-URL]** ein. Dies ist die URL, zu der der Benutzer weitergeleitet werden soll, falls die Anmeldung bei Marketo fehlschlägt. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/add-single-sign-on-to-a-portal-10.png)

   >[!NOTE]
   >
   >Beide Seiten müssen öffentlich verfügbar sein.

>[!MORELIKETHIS]
>
>* [Verwenden einer universellen ID für die Anmeldung bei einem Abonnement](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md){target="_blank"}
>* [Benutzeranmeldung auf SSO beschränken](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md){target="_blank"}
>* [Einladen von Marketo-Benutzern zu zwei Instanzen mit universeller ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122){target="_blank"}
