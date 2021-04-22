---
unique-page-id: 2360356
description: hinzufügen Single-Sign-On für ein Portal - Marketo Docs - Produktdokumentation
title: hinzufügen Einmal-Anmeldung bei einem Portal
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%

---

# hinzufügen Single-Sign-On für ein Portal {#add-single-sign-on-to-a-portal}

Wenn Sie über einen Ordnerdienst verfügen, der Benutzer authentifiziert, können Sie Single Sign-On (SSO) in Marketo zulassen. Diese Funktion wird mit der SAML-Version (Security Assertion Markup Language) 2.0 und höher unterstützt.

Marketo fungiert als SAML-Dienstleister (SP) und benötigt zur Benutzerauthentifizierung einen externen Identitätsanbieter (IdP).

Sobald die einmalige Anmeldung aktiviert ist, kann der IdP die Anmeldeinformationen eines Benutzers überprüfen. Wenn ein Benutzer Marketo-Software verwenden möchte, sendet der IdP dann eine signierte SAML-Nachricht an Marketo, das als SP fungiert. Diese Meldung bestätigt Marketo, dass der Benutzer zur Verwendung von Marketo-Software berechtigt ist.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!NOTE]
>
>Sind Sie ein Microsoft-Azurblauer Benutzer? Sehen Sie sich ihr [Integrationstutorial](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/) an.

## Senden der Anforderung {#how-to-send-the-request}

* Senden Sie die SSO-Anforderung (eine SAML-Antwort) an `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* Als Audiencen-URL des SP. Verwenden `https://saml.marketo.com/sp`
* Wenn Sie das SPNameQualifier-Attribut verwenden, setzen Sie das NameID-Element für Subject auf `https://saml.marketo.com/sp`
* Wenn Sie mehrere Marketo-Abonnement mit demselben SSO-Anbieter verbinden, können Sie für jedes Marketo-Unterelement eindeutige SP-URLs mit dem Format `https://saml.marketo.com/sp/<munchkin_id>` verwenden

>[!NOTE]
>
>Marketo unterstützt nur Identitäts-Provider-initiierte (auch als IdP-initiiert bezeichnet), bei denen der Benutzer zuerst die IDP-Anmeldeseite startet, sich authentifiziert und dann zu &quot;Mein Marketo&quot;navigiert.

## Zusätzliche Hinweise {#additional-notes}

* **Synchronisierungszeit** : Für einen neuen Benutzer ist eine Verzögerung von etwa 10 Minuten vor der Verarbeitung einer anfänglichen SSO-Anforderung erforderlich.
* **Benutzerbereitstellung**  - Benutzer werden manuell von Marketo bereitgestellt.
* **Autorisierung** : Benutzerberechtigungen werden innerhalb von Marketo verwaltet.
* **OAuth-Support**  - Marketo unterstützt OAuth derzeit nicht.
* **Automatische Benutzerübertragung**  - Wird auch als &quot;Just-in-time-Bereitstellung&quot;bezeichnet. Dies ist der Fall, wenn die erste SAML-Anmeldung eines Benutzers in der Lage ist, den Benutzer in einer beliebigen Webanwendung zu erstellen, auf die er zugreifen kann (z. B. Marketo), und keine manuelle Administratoraktion erforderlich ist. Dies wird derzeit von Marketo nicht unterstützt.
* **Verschlüsselung** : Marketo unterstützt derzeit keine Verschlüsselung.

>[!NOTE]
>
>Bevor Sie beginnen, müssen Sie das Identitäts-Provider-Zertifikat im X.509-Format und in der Erweiterung .crt, .der oder .cer verwenden.

## SAML-Einstellungen {#update-saml-settings} aktualisieren

Die einmalige Anmeldung ist standardmäßig deaktiviert. Führen Sie die folgenden Schritte aus, um SAML zu aktivieren und zu konfigurieren.

1. Gehen Sie zu **Admin** und klicken Sie auf **Single-Sign-On**.

   ![](assets/image2014-9-24-14-3a36-3a50.png)

   >[!NOTE]
   >
   >Wenn **Single-Sign-On** unter **Admin** nicht angezeigt wird, wenden Sie sich an [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Klicken Sie unter dem Abschnitt **SAML-Einstellungen** auf **Bearbeiten**.

   ![](assets/image2014-9-24-14-3a37-3a3.png)

1. Ändern Sie **SAML Single Sign-On** in **Enabled**.

   ![](assets/image2014-9-24-14-3a37-3a17.png)

1. Geben Sie **Aussteller-ID**, **Entitäts-ID**, wählen Sie **Benutzer-ID-Speicherort** und klicken Sie dann auf **Durchsuchen**.

   ![](assets/image2014-9-24-14-3a37-3a32.png)

1. Wählen Sie die Datei **Identitätsanbieter-Zertifikat** aus.

   ![](assets/image2014-9-24-14-3a38-3a8.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2014-9-24-14-3a38-3a22.png)

## Einstellungen für Umleitungsseiten aktualisieren {#update-redirect-page-settings}

1. Klicken Sie unter dem Abschnitt **Seiten umleiten** auf **Bearbeiten**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Kunden, die eine universelle ID zusammen mit einer einmaligen Anmeldung verwenden, müssen die Anmelde-URL des Identitätsanbieters im Feld **Anmelde-URL** eingeben.

1. Geben Sie eine **Abmelden-URL** ein. Dies ist die URL, zu der der Benutzer weitergeleitet werden soll, wenn er sich von Marketo abmeldet.

   ![](assets/eight.png)

1. Geben Sie eine **Fehler-URL** ein. Dies ist die URL, zu der der Benutzer weitergeleitet werden soll, falls die Anmeldung bei Marketo fehlschlägt. Klicken Sie auf **Speichern**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Beide Seiten müssen öffentlich zugänglich sein.

>[!MORELIKETHIS]
>
>* [Verwenden einer universellen ID für die Abonnement-Anmeldung](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Benutzeranmeldung auf SSO beschränken](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
>* [Einladen von Marketo-Benutzern zu zwei Instanzen mit universeller ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

