---
unique-page-id: 2359746
description: Passen Sie Ihre Landingpages-URLs mit einem CNAME - Marketing Docs - Produktdokumentation an.
title: Passen Sie Ihre Landingpages-URLs mit einem CNAME an
translation-type: tm+mt
source-git-commit: 2969e6f94f5fd781e2167ae2aa8680bb8d134754
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---


# Passen Sie Ihre Landingpages-URLs mit einem CNAME {#customize-your-landing-page-urls-with-a-cname} an

Obwohl Marketo Ihre Landingpages hostet, kann die URL komplett angepasst werden. Wie es ohne CNAME aussieht:

`http://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

So sollte es aussehen:

`http://go.YourCompany.com/UnsubscribePage.html`

## Wählen Sie einen CNAME {#choose-a-cname}

Wählen Sie ein Wort, das Sie am Anfang der URL für Ihre Landingpages suchen möchten. Es ist nur ein Wort und sollte relativ kurz sein. Beispiele:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

Das eine Wort (plus YourCompany.com) wird als CNAME bezeichnet. Du wirst das später brauchen, also notiere es dir.

## Suchen Sie die Kontozeichenfolge {#find-your-account-string}

1. Gehen Sie zum Bereich **Admin** und klicken Sie auf **Landingpages**.

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**Administratorberechtigungen erforderlich**

1. Kopieren Sie unter der Registerkarte **Einstieg** **Seiten** das **Konto** **Zeichenfolge** aus dem Abschnitt **Einstellungen**.

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. Sie werden später auch benötigen, also notieren Sie es sich.

## Anforderung an IT senden {#send-request-to-it}

Bitten Sie Ihre IT-Mitarbeiter, den folgenden CNAME einzurichten: (Ersetzen Sie das Wort [CNAME] und [ACCOUNT STRING] durch den Text aus dem vorherigen Schritt.)

[CNAME].YourCompany.com >  [ACCOUNT STRING].mktoweb.com

## Complete CNAME Setup {#complete-cname-setup}

1. Nachdem der CNAME von Ihrer IT-Abteilung erstellt wurde, gehen Sie zu **Admin** und klicken Sie auf **Landingpages**.

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. Klicken Sie im Abschnitt **Einstellungen** auf **Bearbeiten**.

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. Geben Sie Ihren CNAME in **Domänennamen für Landingpages** ein, geben Sie Ihre **Fallback-Seite** ein, geben Sie Ihre **Homepage** ein und klicken Sie auf **Speichern**.

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>Ihre Ausweichseite ist die Seite, zu der Interessenten umgeleitet werden, wenn Ihre Marketing-Landingpage nicht verfügbar ist.

Gute Arbeit! Ihre Landingpages werden jetzt mit Ihrer Firma-Domäne gekennzeichnet.
