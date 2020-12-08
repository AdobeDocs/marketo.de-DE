---
unique-page-id: 2359746
description: Passen Sie Ihre Landingpages-URLs mit einem CNAME - Marketing Docs - Produktdokumentation an.
title: Passen Sie Ihre Landingpages-URLs mit einem CNAME an
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---


# Passen Sie Ihre Landingpages-URLs mit einem CNAME an {#customize-your-landing-page-urls-with-a-cname}

Obwohl Marketo Ihre Landingpages hostet, kann die URL komplett angepasst werden. Wie es ohne CNAME aussieht:
`<pre data-theme="Confluence">http://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html</pre>` So sollte es aussehen:
`<pre data-theme="Confluence"> http://go.YourCompany.com/UnsubscribePage.html</pre>`

## CNAME auswählen {#choose-a-cname}

Wählen Sie ein Wort, das Sie am Anfang der URL für Ihre Landingpages suchen möchten. Es ist nur ein Wort und sollte relativ kurz sein. Beispiele:

* gehen. [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)
* info. [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)
* Seiten. [YourCompany.com/NameOfPage.html](http://YourCompany.com/NameOfPage.html)

Das eine Wort (plus [YourCompany.com](http://YourCompany.com)) wird als CNAME bezeichnet. Sie werden dies später benötigen, also notieren Sie es sich.

## Ihre Kontozeichenfolge suchen {#find-your-account-string}

1. Gehen Sie zum **Admin** -Bereich und klicken Sie auf **Landingpages.**

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**Administratorberechtigungen erforderlich**

1. Kopieren Sie unter der Registerkarte &quot; **Einstiegsseiten** &quot; **Seiten** die **Kontozeichenfolge****aus dem Abschnitt** Einstellungen **** .

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. Sie werden später auch benötigen, also notieren Sie es sich.

## Anforderung an IT senden {#send-request-to-it}

Bitten Sie Ihre IT-Mitarbeiter, den folgenden CNAME einzurichten: (Ersetzen Sie das Wort [CNAME] und [ACCOUNT STRING] durch den Text aus dem vorherigen Schritt.)

[CNAME]. [YourCompany.com](http://yourcompany.com/) > [KONTOZEICHENFOLGE]. [mktoweb.com](http://mktoweb.com/)

## Vollständige CNAME-Einrichtung {#complete-cname-setup}

1. Nachdem der CNAME von Ihrer IT-Abteilung erstellt wurde, gehen Sie zu **Admin** und klicken Sie auf **Einstiegsseiten** ****.

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. Klicken Sie im Abschnitt **Einstellungen** auf **Bearbeiten**.

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. Geben Sie Ihren CNAME in **Domain** **name** **für** **Landing** **Pages****** ******** **** ein, geben Sie Ihren Fallbackpageein, geben Sie IhreHomepageein und klicken Sie aufSave.

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>Ihre Ausweichseite ist die Seite, zu der Interessenten umgeleitet werden, wenn Ihre Marketing-Landingpage nicht verfügbar ist.

Gute Arbeit! Ihre Landingpages werden jetzt mit Ihrer Firma-Domäne gekennzeichnet.