---
unique-page-id: 14352405
description: Einrichten von SSO über SAML 2.0 in [!DNL Sales Connect] - Marketo-Dokumente - Produktdokumentation
title: Einrichten von SSO über SAML 2.0 in [!DNL Sales Connect]
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# Einrichten von SSO über SAML 2.0 in [!DNL Sales Connect] {#setting-up-sso-through-saml-in-sales-connect}

Wir unterstützen SSO durch die SAML 2.0-Spezifikation. Wir verfügen derzeit jedoch über keine direkten Integrationen mit Anbietern. Wir müssen einige Informationen von Ihrem SSO-Provider erfassen, um diese Einrichtung zu erhalten.

>[!NOTE]
>
>Dies gilt nur für **Marketo Sales Connect**-Benutzer. Wenn Sie kein Sales Connect besitzen, aber mehr darüber erfahren möchten, wenden Sie sich bitte an das Adobe Account Team (Ihren Account Manager).

## Anforderungen {#requirements}

* SSO-Konto
* Marketo Sales Connect-Abonnement
* Metadata.xml aus SSO-Konto (Problem-URL, der zu validierende Endpunkt und ein öffentlicher Schlüssel)

## Einrichten {#setup}

Die Datei „metadata.xml“ der SSO-Instanz Ihres Teams sollte die Aussteller-URL, den zu validierenden Endpunkt und einen öffentlichen Schlüssel enthalten.

Wir benötigen außerdem den SSO-Speicherort für das SSO-Konto Ihres Unternehmens, um eine eindeutige Domain zu sein. Wir benötigen beispielsweise eine eindeutige Subdomain wie `toutapp.pingidentity.com` oder Ähnliches. Ohne diesen Typ der eindeutigen Kennung können wir SAML nicht über das Dashboard einrichten.

One Login und Okta stellen beim Zuweisen einer URL nicht immer eindeutige Kennungen bereit. Wenn Sie Okta oder One Login verwenden, bedeutet dies, dass wir nicht in der Lage sein werden, eine Anmeldung über die Dashboard-Schaltfläche einzurichten. Wir können sie weiterhin über die Single Sign-On-Schaltfläche in der [Web-Anwendung) ](https://toutapp.com/login).

Sobald wir diese Informationen haben, werden wir mit unserem Engineering-Team zusammenarbeiten, um diese für Ihr Abonnement einzurichten.
