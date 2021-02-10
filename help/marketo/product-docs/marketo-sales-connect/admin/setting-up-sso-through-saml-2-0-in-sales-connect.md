---
unique-page-id: 14352405
description: Einrichten der einmaligen Anmeldung über SAML 2.0 in Sales Connect - Marketing Docs - Produktdokumentation
title: Einrichten der einmaligen Anmeldung über SAML 2.0 in Sales Connect
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# EINRICHTUNG DER EINRICHTUNG DURCH SAML 2.0 in Sales Connect {#setting-up-sso-through-saml-in-sales-connect}

Wir unterstützen die einmalige Anmeldung über die SAML 2.0-Spezifikation. Es gibt derzeit jedoch keine direkten Integrationen mit anderen Anbietern. Wir müssen einige Informationen von Ihrem SSO-Anbieter sammeln, um diese Einrichtung zu erhalten.

>[!NOTE]
>
>Dies gilt nur für **Marketing Connect**-Kunden. Wenn Sie nicht über Sales Connect verfügen, aber mehr erfahren möchten, wenden Sie sich bitte an Ihren Kundenbetreuer.

## Voraussetzungen {#requirements}

* SSO-Konto
* Marketing-Sales-Connect-Abonnement
* Metadata.xml aus einem SSO-Konto (Ausgabe-URL, Endpunkt für die Überprüfung und öffentlicher Schlüssel)

## Setup {#setup}

Die Datei &quot;metadata.xml&quot;aus der SSO-Instanz Ihres Teams sollte die Aussteller-URL, den Endpunkt für die Überprüfung und einen öffentlichen Schlüssel enthalten.

Außerdem benötigen wir den SSO-Standort, damit Ihr SSO-Konto eine eindeutige Domäne sein kann. Beispielsweise benötigen wir eine eindeutige Subdomäne wie `toutapp.pingidentity.com` oder Ähnliches. Ohne diesen eindeutigen Bezeichner können wir keine SAML aus dem Dashboard einrichten.

Bei einer Anmeldung und Okta werden beim Zuweisen einer URL nicht immer eindeutige IDs bereitgestellt. Wenn Sie Okta oder One Login verwenden, bedeutet das, dass wir nicht in der Lage sein werden, eine Anmeldung über die Schaltfläche Dashboard einzurichten. Wir können sie weiterhin über die Schaltfläche Single Sign-On auf der [Webanwendung](http://toutapp.com/login) einrichten.

Sobald uns diese Informationen vorliegen, werden wir mit unserem Ingenieurteam zusammenarbeiten, um dies für Ihr Abonnement einzurichten.
