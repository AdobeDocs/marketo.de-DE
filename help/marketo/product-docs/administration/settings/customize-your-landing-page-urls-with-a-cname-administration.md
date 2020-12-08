---
unique-page-id: 2360189
description: Passen Sie Ihre Landingpages-URLs mit einem CNAME (Administration) - Marketing Docs - Produktdokumentation an.
title: Passen Sie Ihre Landingpages-URLs mit einem CNAME (Administration) an
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# Passen Sie Ihre Landingpages-URLs mit einem CNAME (Administration) an {#customize-your-landing-page-urls-with-a-cname-administration}

Obwohl Marketo Ihre Landingpages hostet, sollte die URL für Ihre Firma angepasst werden.

>[!NOTE]
>
>**Beispiel**
>
>Kein CNAME:
>
>http://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>Markenbezeichnung CNAME:
>
>http://go.**YourCompany**.com/UnsuscribePage.html

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

Lasst uns euch einrichten!

1. CNAME auswählen

   Es ist der erste Teil der URL. Beispiele:

   * **go**.YourCompany.com/NameOfPage.html
   * **info**.YourCompany.com/NameOfPage.html
   * **pages**.YourCompany.com/NameOfPage.html

   Das eine Wort (plus YourCompany.com) wird als CNAME bezeichnet. Sie werden dies später benötigen, also notieren Sie es sich.

1. Ihre Kontozeichenfolge suchen
1. Gehen Sie zum **Admin** -Bereich und klicken Sie auf **Landingpages**.

   ![](assets/image2014-9-16-13-3a9-3a44.png)

1. Kopieren Sie unter der Registerkarte **Landingpages **die Kontozeichenfolge aus dem Abschnitt Einstellungen.

   ![](assets/image2014-9-16-13-3a9-3a57.png)

1. Sie werden dies auch später benötigen, also notieren Sie es sich.
1. Anforderung an IT senden
1. Bitten Sie Ihre IT-Mitarbeiter, den folgenden CNAME einzurichten (ersetzen Sie das Wort [CNAME] und [KONTOZEICHENFOLGE] durch den Text aus dem vorherigen Schritt):

   [CNAME].YourCompany.com > [ACCOUNT STRING].mktoweb.com

1. Vollständige CNAME-Einrichtung
1. Sobald der CNAME von Ihrer IT-Abteilung erstellt wurde, gehen Sie zu **Admin** und klicken Sie auf **Landingpages**.

   ![](assets/image2014-9-16-13-3a10-3a14.png)

1. Klicken Sie im Abschnitt **Einstellungen** auf **Bearbeiten**.

   ![](assets/image2014-9-16-13-3a10-3a31.png)

1. Geben Sie Ihren CNAME in **Domänennamen für Landingpages** ein, geben Sie Ihre **Fallback-Seite** ein, geben Sie Ihre **Homepage** ein und klicken Sie auf **Speichern**.

   ![](assets/image2014-9-16-13-3a10-3a45.png)

   Auf Ihrer Fallback-Seite werden Personen umgeleitet, wenn Ihre Marketing-Landingpage nicht verfügbar ist.
Gute Arbeit! Ihre Landingpages werden jetzt mit Ihrer Firma-Domäne gekennzeichnet.

