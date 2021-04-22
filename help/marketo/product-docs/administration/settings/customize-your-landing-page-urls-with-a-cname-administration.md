---
unique-page-id: 2360189
description: Passen Sie Ihre Landingpages-URLs mit einem CNAME (Administration) - Marketo Docs - Produktdokumentation an.
title: Passen Sie Ihre Landingpages-URLs mit einem CNAME (Administration) an
exl-id: a5aa1c76-15f7-4e8c-a736-77c79f65c368
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 2%

---

# Passen Sie Ihre Landingpages-URLs mit einem CNAME (Administration) {#customize-your-landing-page-urls-with-a-cname-administration} an

Auch wenn Marketo Ihre Landingpages hostet, sollte die URL für Ihre Firma angepasst werden.

>[!NOTE]
>
>Kein CNAME:
>
>https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>Markenbezeichnung CNAME:
>
>https://go.**YourCompany**.com/UnsuscribePage.html

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

Wir helfen Ihnen gerne bei der Einrichtung!

1. Wählen Sie einen CNAME.

   Es ist der erste Teil der URL. Beispiele:

   * **go**.YourCompany.com/NameOfPage.html
   * **info**.YourCompany.com/NameOfPage.html
   * **pages**.YourCompany.com/NameOfPage.html

   Das eine Wort (plus YourCompany.com) wird als CNAME bezeichnet. Sie werden dies später benötigen, also notieren Sie es sich.

1. Suchen Sie Ihre Kontozeichenfolge.

1. Gehen Sie zum Bereich **Admin** und klicken Sie auf **Landingpages**.

   ![](assets/image2014-9-16-13-3a9-3a44.png)

1. Kopieren Sie unter der Registerkarte **Landingpages** die Kontozeichenfolge aus dem Abschnitt Einstellungen.

   ![](assets/image2014-9-16-13-3a9-3a57.png)

1. Sie werden dies auch später benötigen, also notieren Sie es sich.

1. Anforderung an IT senden

1. Bitten Sie Ihre IT-Mitarbeiter, den folgenden CNAME einzurichten (ersetzen Sie das Wort [CNAME] und [ACCOUNT STRING] durch den Text aus dem vorherigen Schritt):

   [CNAME].YourCompany.com >  [ACCOUNT STRING].mktoweb.com

1. Führen Sie die CNAME-Einrichtung durch.

1. Nachdem der CNAME von Ihrer IT-Abteilung erstellt wurde, gehen Sie zu **Admin** und klicken Sie auf **Landingpages**.

   ![](assets/image2014-9-16-13-3a10-3a14.png)

1. Klicken Sie unter dem Abschnitt **Einstellungen** auf **Bearbeiten**.

   ![](assets/image2014-9-16-13-3a10-3a31.png)

1. Geben Sie Ihren CNAME in **Domänennamen für Landingpages** ein, geben Sie Ihre **Fallback-Seite** ein, geben Sie Ihre **Homepage** ein und klicken Sie auf **Speichern**.

   ![](assets/image2014-9-16-13-3a10-3a45.png)

Auf Ihrer Ausweichseite werden Personen umgeleitet, wenn Ihre Marketo-Landingpage nicht verfügbar ist.

Gute Arbeit! Ihre Landingpages werden jetzt mit Ihrer Firma-Domäne gekennzeichnet.
