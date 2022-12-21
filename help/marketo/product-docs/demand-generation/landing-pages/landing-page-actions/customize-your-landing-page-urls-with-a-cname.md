---
unique-page-id: 2359746
description: Passen Sie Ihre Landingpage-URLs mit einem CNAME an - Marketo Docs - Produktdokumentation
title: Anpassen der Landingpage-URLs mit einem CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Anpassen der Landingpage-URLs mit einem CNAME {#customize-your-landing-page-urls-with-a-cname}

Auch wenn Marketo Ihre Landingpages hostet, kann die URL vollständig angepasst werden. Wie es ohne CNAME aussieht:

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

So sollte es aussehen:

`https://go.YourCompany.com/UnsubscribePage.html`

## CNAME auswählen {#choose-a-cname}

Wählen Sie ein Wort aus, um am Anfang der URL für Ihre Landingpages zu gehen. Es ist nur ein Wort und sollte relativ kurz sein. Beispiele:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

Das eine Wort (plus YourCompany.com) wird als CNAME bezeichnet. Sie werden dies später benötigen, damit Sie es sich notieren können.

## Kontozeichenfolge suchen {#find-your-account-string}

1. Navigieren Sie zu **Admin** Bereich und klicken Sie auf **Landing Pages**.

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**Erforderliche Administratorberechtigungen**

1. Unter dem **Landing** **Seiten** Registerkarte, kopieren Sie die **Konto** **Zeichenfolge** von **Einstellungen** Abschnitt.

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. Sie werden später auch benötigen, also notieren Sie sich das.

## Anfrage an IT senden {#send-request-to-it}

Bitten Sie Ihre IT-Mitarbeiter, den folgenden CNAME einzurichten: (Ersetzen Sie das Wort [CNAME] und [KONTOZEICHENFOLGE] mit dem Text aus dem vorherigen Schritt.)

[CNAME].YourCompany.com > [KONTOZEICHENFOLGE].mktoweb.com

## Vollständige CNAME-Einrichtung {#complete-cname-setup}

1. Sobald Ihr IT den CNAME erstellt hat, navigieren Sie zu **Admin** und klicken Sie auf **Landing Pages**.

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. Unter dem **Einstellungen** Abschnitt, klicken Sie auf **Bearbeiten**.

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. Geben Sie Ihren CNAME in ein. **Domänenname für Einstiegsseiten** eingeben **Fallback-Seite** eingeben **Homepage** und klicken Sie auf **Speichern**.

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>Ihre Fallback-Seite ist die Seite, an die Leads weitergeleitet werden, wenn Ihre Marketo-Landingpage nicht verfügbar ist.

Gut gemacht! Ihre Landingpages sind jetzt mit Ihrer Unternehmensdomäne gekennzeichnet.
