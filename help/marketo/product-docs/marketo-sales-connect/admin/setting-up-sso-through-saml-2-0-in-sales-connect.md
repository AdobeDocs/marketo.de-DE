---
unique-page-id: 14352405
description: Einrichten von SSO über SAML 2.0 in Sales Connect - Marketo Docs - Produktdokumentation
title: Einrichten von SSO über SAML 2.0 in Sales Connect
exl-id: aab80626-d6d1-4194-9733-09c90c0b49a6
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Einrichten von SSO über SAML 2.0 in Sales Connect {#setting-up-sso-through-saml-in-sales-connect}

Wir unterstützen SSO über die SAML 2.0-Spezifikation. Derzeit gibt es jedoch keine direkten Integrationen mit anderen Anbietern. Wir müssen einige Informationen von Ihrem SSO-Provider erfassen, um diese Einrichtung zu erhalten.

>[!NOTE]
>
>Dies gilt nur für Benutzer von **Marketo Sales Connect**. Wenn Sie nicht über Sales Connect verfügen, aber mehr erfahren möchten, wenden Sie sich an das Adobe Account Team (Ihren Kundenbetreuer).

## Anforderungen {#requirements}

* SSO-Konto
* Marketo Sales Connect-Abonnement
* Metadata.xml aus dem SSO-Konto (Problem-URL, Endpunkt zur Validierung und öffentlicher Schlüssel)

## Setup {#setup}

Die Datei &quot;metadata.xml&quot;aus der SSO-Instanz Ihres Teams sollte die Emittenten-URL, den Endpunkt für die Validierung und einen öffentlichen Schlüssel enthalten.

Außerdem benötigen wir die SSO-Position, damit das SSO-Konto Ihres Unternehmens eine eindeutige Domäne sein kann. Beispielsweise benötigen wir eine eindeutige Subdomäne wie `toutapp.pingidentity.com` oder eine ähnliche. Ohne diesen eindeutigen Bezeichnungstyp können wir SAML nicht im Dashboard einrichten.

Bei einer Anmeldung und Okta werden beim Zuweisen einer URL nicht immer eindeutige Kennungen angegeben. Wenn Sie Okta oder One Login verwenden, bedeutet dies, dass wir nicht in der Lage sein werden, eine Anmeldung über die Dashboard-Schaltfläche einzurichten. Sie können weiterhin über die Schaltfläche Single Sign-On in der [Webanwendung](https://toutapp.com/login) eingerichtet werden.

Sobald wir diese Informationen haben, arbeiten wir mit unserem Technikerteam zusammen, um diese für Ihr Abonnement einzurichten.
