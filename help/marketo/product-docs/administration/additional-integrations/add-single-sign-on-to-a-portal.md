---
unique-page-id: 2360356
description: Single Sign-On zu einem Portal hinzufügen - Marketo Docs - Produktdokumentation
title: Single Sign-On zu einem Portal hinzufügen
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
source-git-commit: e4d581ab258a875747a6d5323764e8b4a3949cba
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%

---

# Single Sign-On zu einem Portal hinzufügen {#add-single-sign-on-to-a-portal}

Wenn Sie über einen Verzeichnisdienst verfügen, der Benutzer authentifiziert, können Sie die einmalige Anmeldung (SSO) in Marketo zulassen. Diese Funktion wird mit der SAML-Version (Security Assertion Markup Language) ab Version 2.0 unterstützt.

Marketo fungiert als SAML-Dienstanbieter (SP) und benötigt zur Authentifizierung von Benutzern einen externen Identitäts-Provider (IdP).

Sobald die einmalige Anmeldung aktiviert ist, kann der IdP die Anmeldeinformationen eines Benutzers überprüfen. Wenn ein Benutzer die Marketo-Software verwenden möchte, sendet der IdP dann eine signierte SAML-Nachricht an Marketo, die als SP fungiert. Diese Meldung bestätigt Marketo, dass der Benutzer zur Verwendung von Marketo-Software berechtigt ist.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!NOTE]
>
>Sind Sie ein Microsoft Azure-Benutzer? Sehen Sie sich das [Integrations-Tutorial](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/) an.

## Senden der Anforderung {#how-to-send-the-request}

* Senden Sie die SSO-Anfrage, die eine SAML-Antwort ist, an `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* Als Zielgruppen-URL der SP. Verwenden `http://saml.marketo.com/sp`
* Wenn Sie das Attribut SPNameQualifier verwenden, setzen Sie das Element NameID für Subject auf `http://saml.marketo.com/sp`
* Wenn Sie mehrere Marketo-Abonnements mit demselben SSO-Provider verknüpfen, können Sie eindeutige SP-URLs für jedes Marketo-Unterelement im Format `http://saml.marketo.com/sp/<munchkin_id>` verwenden.

>[!NOTE]
>
>Marketo unterstützt nur Identity Provider-initiierte (auch als IdP-Initiated bezeichnete) Anwendungen, bei denen der Benutzer zuerst die IP-Anmeldeseite startet, sich authentifiziert und dann zu My Marketo navigiert.

## Weitere Hinweise {#additional-notes}

* **Synchronisierungszeit** : Für einen neuen Benutzer dauert es etwa 10 Minuten, bis eine erste SSO-Anfrage verarbeitet wird.
* **Benutzerbereitstellung**  - Benutzer werden manuell von Marketo bereitgestellt.
* **Autorisierung**  - Benutzerberechtigungen werden in Marketo verwaltet.
* **OAuth-Unterstützung**  - Marketo unterstützt OAuth derzeit nicht.
* **Automatische Benutzerübertragung**  - Wird auch als &quot;Just in Time Provisioning&quot;bezeichnet. Dies ist der Fall, wenn die erste SAML-Anmeldung eines Benutzers in der Lage ist, den Benutzer in einer beliebigen Webanwendung zu erstellen, auf die er zugreift (z. B. Marketo), und keine manuelle Administratoraktion erforderlich ist. Dies wird derzeit von Marketo nicht unterstützt.
* **Verschlüsselung**  - Marketo unterstützt derzeit nicht die Verschlüsselung.

>[!NOTE]
>
>Vergewissern Sie sich vor dem Start, dass Ihr Identitätsanbieter-Zertifikat im X.509-Format und in der Erweiterung .crt, .der oder .cer vorliegt.

## SAML-Einstellungen aktualisieren {#update-saml-settings}

Die einmalige Anmeldung ist standardmäßig deaktiviert. Führen Sie diese Schritte aus, um SAML zu aktivieren und zu konfigurieren.

1. Gehen Sie zu **Admin** und klicken Sie auf **Single Sign-On**.

   ![](assets/image2014-9-24-14-3a36-3a50.png)

   >[!NOTE]
   >
   >Wenn **Single Sign-On** unter **Admin** nicht angezeigt wird, wenden Sie sich an [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Klicken Sie unter dem Abschnitt **SAML Settings** auf **Edit**.

   ![](assets/image2014-9-24-14-3a37-3a3.png)

1. Ändern Sie **SAML Single Sign-On** in **Aktiviert**.

   ![](assets/image2014-9-24-14-3a37-3a17.png)

1. Geben Sie Ihre **Aussteller-ID**, **Entitäts-ID**, wählen Sie den **Benutzer-ID-Speicherort** aus und klicken Sie dann auf **Durchsuchen**.

   ![](assets/image2014-9-24-14-3a37-3a32.png)

1. Wählen Sie die Datei **Identity Provider Certificate** aus.

   ![](assets/image2014-9-24-14-3a38-3a8.png)

1. Klicken Sie auf **Save**.

   ![](assets/image2014-9-24-14-3a38-3a22.png)

## Einstellungen für Umleitungsseiten aktualisieren {#update-redirect-page-settings}

1. Klicken Sie unter dem Abschnitt **Umleitungsseiten** auf **Bearbeiten**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Kunden, die eine universelle ID zusammen mit SSO verwenden, müssen die Anmelde-URL des Identitätsanbieters im Feld **Anmelde-URL** eingeben.

1. Geben Sie eine **Abmelde-URL** ein. Dies ist die URL, zu der der Benutzer weitergeleitet werden soll, wenn er sich von Marketo abmeldet.

   ![](assets/eight.png)

1. Geben Sie eine **Fehler-URL** ein. Dies ist die URL, zu der der Benutzer weitergeleitet werden soll, falls die Anmeldung bei Marketo fehlschlägt. Klicken Sie auf **Save**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Beide Seiten müssen öffentlich zugänglich sein.

>[!MORELIKETHIS]
>
>* [Verwendung einer universellen ID zur Anmeldung von Abonnements](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
* [Benutzeranmeldung auf SSO beschränken](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
* [Einladen von Marketo-Benutzern zu zwei Instanzen mit universeller ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

