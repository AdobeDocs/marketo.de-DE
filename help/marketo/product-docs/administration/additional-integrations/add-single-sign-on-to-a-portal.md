---
unique-page-id: 2360356
description: Single Sign-On zu einem Portal hinzufügen - Marketo Docs - Produktdokumentation
title: Single Sign-On zu einem Portal hinzufügen
exl-id: 72f96239-7252-4cbc-bbe1-84ac7ae7f92e
feature: Administration
source-git-commit: 48f280eef0fb5762b8032307c5442906f7ceaae3
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Single Sign-On zu einem Portal hinzufügen {#add-single-sign-on-to-a-portal}

Wenn Sie über einen Verzeichnisdienst verfügen, der Benutzer authentifiziert, können Sie die einmalige Anmeldung (SSO) in Marketo zulassen. Wir unterstützen diese Funktion mithilfe von [!DNL Security Assertion Markup Language] (SAML) Version 2.0 und höher.

Marketo fungiert als SAML-Dienstanbieter (SP) und benötigt zur Authentifizierung von Benutzern einen externen Identitäts-Provider (IdP).

Sobald die einmalige Anmeldung aktiviert ist, kann der IdP die Anmeldeinformationen eines Benutzers überprüfen. Wenn ein Benutzer die Marketo-Software verwenden möchte, sendet der IdP dann eine signierte SAML-Nachricht an Marketo, die als SP fungiert. Diese Meldung bestätigt Marketo, dass der Benutzer zur Verwendung von Marketo-Software berechtigt ist.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!IMPORTANT]
>
>Dies gilt nicht für Anmeldungen, die mit Adobe Identity integriert wurden. Für Adobe Identity-Anmeldungen wird Single Sign-On auf der Adobe-Org-Ebene in Adobe Admin Console eingerichtet. [Weitere Informationen hier](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

>[!NOTE]
>
>Bist du ein [!DNL Microsoft Azure] Benutzer? Sehen Sie sich die [Integrations-Tutorial](https://azure.microsoft.com/en-us/documentation/articles/active-directory-saas-marketo-tutorial/){target="_blank"}. FYI, es gibt einen Tippfehler in Schritt 5c ihres Tutorials. Verwenden Sie `https://<munchkinid>.mktoweb.com`, **_not_** `https://<munchkinid>.marketo.com`.

## Senden der Anforderung {#how-to-send-the-request}

* Senden Sie die SSO-Anfrage, die eine SAML-Antwort ist, an `https://login.marketo.com/saml/assertion/<your-munchkin-id>`
* Als Zielgruppen-URL der SP. Verwendung `http://saml.marketo.com/sp`
* Wenn Sie das Attribut SPNameQualifier verwenden, setzen Sie das Element NameID für Subject auf `http://saml.marketo.com/sp`
* Wenn Sie mehrere Marketo-Abonnements mit demselben SSO-Provider verknüpfen, können Sie eindeutige SP-URLs für jeden Marketo-Unterordner im folgenden Format verwenden: `http://saml.marketo.com/sp/<munchkin_id>`

>[!NOTE]
>
>Marketo unterstützt nur Identity Provider-initiierte (auch als IdP-Initiated bezeichnete) Anwendungen, bei denen der Benutzer zuerst die IP-Anmeldeseite startet, sich authentifiziert und dann zu My Marketo navigiert.

## Weitere Hinweise {#additional-notes}

* **Synchronisierungszeit** - Für einen neuen Benutzer dauert es etwa 10 Minuten, bis eine erste SSO-Anfrage verarbeitet wird.
* **Benutzerbereitstellung** - Benutzer werden manuell von Marketo bereitgestellt.
* **Autorisierung** - Benutzerberechtigungen werden in Marketo verwaltet.
* **OAuth-Unterstützung** - Marketo unterstützt OAuth derzeit nicht.
* **Automatische Benutzerübertragung** - Wird auch als &quot;Just in Time Provisioning&quot;bezeichnet. Dies ist der Fall, wenn die erste SAML-Anmeldung eines Benutzers in der Lage ist, den Benutzer in einer beliebigen Webanwendung zu erstellen, auf die er zugreift (z. B. Marketo), und keine manuelle Administratoraktion erforderlich ist. Dies wird derzeit von Marketo nicht unterstützt.
* **Verschlüsselung** - Marketo unterstützt derzeit keine Verschlüsselung.

>[!NOTE]
>
>Vergewissern Sie sich vor dem Start, dass Ihr Identitätsanbieter-Zertifikat im X.509-Format und in der Erweiterung .crt, .der oder .cer vorliegt.

## SAML-Einstellungen aktualisieren {#update-saml-settings}

Die einmalige Anmeldung ist standardmäßig deaktiviert. Führen Sie diese Schritte aus, um SAML zu aktivieren und zu konfigurieren.

1. Navigieren Sie zu **[!UICONTROL Admin]** Bereich.

   ![](assets/add-single-sign-on-to-a-portal-1.png)

1. Klicks **[!UICONTROL Single Sign-on]**.

   ![](assets/add-single-sign-on-to-a-portal-2.png)

   >[!NOTE]
   >
   >Wenn Sie nicht sehen **[!UICONTROL Single Sign-on]** under **[!UICONTROL Admin]**, Kontakt [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. Unter dem **[!UICONTROL SAML-Einstellungen]** Abschnitt, klicken Sie auf **[!UICONTROL Bearbeiten]**.

   ![](assets/add-single-sign-on-to-a-portal-3.png)

1. Änderung **[!UICONTROL SAML Single Sign-On]** nach **[!UICONTROL Aktiviert]**.

   ![](assets/add-single-sign-on-to-a-portal-4.png)

1. Geben Sie Ihre **[!UICONTROL Aussteller-ID]**, **[!UICONTROL Entity ID]**, wählen Sie die **[!UICONTROL Standort der Benutzer-ID]** Klicken Sie auf **[!UICONTROL Durchsuchen]**.

   ![](assets/add-single-sign-on-to-a-portal-5.png)

1. Wählen Sie **[!UICONTROL Identitätsanbieterzertifikat]** -Datei.

   ![](assets/add-single-sign-on-to-a-portal-6.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/add-single-sign-on-to-a-portal-7.png)

## Einstellungen für Umleitungsseiten aktualisieren {#update-redirect-page-settings}

1. Unter dem **[!UICONTROL Umleitungsseiten]** Abschnitt, klicken Sie auf **[!UICONTROL Bearbeiten]**.

   ![](assets/add-single-sign-on-to-a-portal-8.png)

   >[!NOTE]
   >
   >Kunden, die eine universelle ID zusammen mit SSO verwenden, müssen die Anmelde-URL des Identitätsanbieters in die **[!UICONTROL Anmelde-URL]** -Feld.

1. Geben Sie einen **[!UICONTROL URL abmelden]**. Dies ist die URL, zu der der Benutzer weitergeleitet werden soll, wenn er sich von Marketo abmeldet.

   ![](assets/add-single-sign-on-to-a-portal-9.png)

1. Geben Sie eine **[!UICONTROL Fehler-URL]**. Dies ist die URL, zu der der Benutzer weitergeleitet werden soll, falls die Anmeldung bei Marketo fehlschlägt. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/add-single-sign-on-to-a-portal-10.png)

   >[!NOTE]
   >
   >Beide Seiten müssen öffentlich zugänglich sein.

>[!MORELIKETHIS]
>
>* [Verwendung einer universellen ID zur Anmeldung von Abonnements](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md){target="_blank"}
>* [Benutzeranmeldung auf &quot;Nur SSO&quot;beschränken](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md){target="_blank"}
>* [Einladen von Marketo-Benutzern zu zwei Instanzen mit universeller ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122){target="_blank"}
