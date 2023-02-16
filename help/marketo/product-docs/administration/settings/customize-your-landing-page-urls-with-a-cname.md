---
unique-page-id: 2360189
description: Passen Sie Ihre Landingpage-URLs mit einem CNAME (Administration) an - Marketo Docs - Produktdokumentation
title: Landingpage-URLs mit einem CNAME (Administration) anpassen
exl-id: a5aa1c76-15f7-4e8c-a736-77c79f65c368
source-git-commit: 07899e541b3624e99e0ead59d898ced2ab4e57af
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 6%

---

# Landingpage-URLs mit einem CNAME anpassen  {#customize-your-landing-page-urls-with-a-cname}

Auch wenn Marketo Ihre Landingpages hostet, sollte die URL für Ihr Unternehmen angepasst werden.

>[!NOTE]
>
>Kein CNAME:
>
>https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>MarkenCNAME:
>
>https://go **YourCompany**.com/UnsuscribePage.html

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

Wir helfen Ihnen gerne bei der Einrichtung!

1. Wählen Sie einen CNAME aus.

   Dies ist der erste Teil der URL. Beispiele:

   * **go**.YourCompany.com/NameOfPage.html
   * **Info**.YourCompany.com/NameOfPage.html
   * **pages**.YourCompany.com/NameOfPage.html

   Das eine Wort (plus YourCompany.com) wird als CNAME bezeichnet. Sie werden dies später benötigen, damit Sie es sich notieren können.

1. Suchen Sie Ihre Kontozeichenfolge.

1. Navigieren Sie zum **Admin**-Bereich.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Klicken Sie auf **Landing Pages**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

1. Unter dem **Landing Pages** -Registerkarte, kopieren Sie die Kontozeichenfolge aus dem Abschnitt Einstellungen .

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

1. Sie werden dies auch später benötigen, also notieren Sie es sich.

1. Anfrage an IT senden.

1. Bitten Sie Ihre IT-Mitarbeiter, den folgenden CNAME einzurichten (ersetzen Sie das Wort [CNAME] und [KONTOZEICHENFOLGE] mit dem Text aus dem vorherigen Schritt):

   [CNAME].YourCompany.com > [KONTOZEICHENFOLGE].mktoweb.com

1. Vollständige CNAME-Einrichtung.

1. Sobald Ihre IT den CNAME erstellt hat, kehren Sie zum **Admin** Bereich.

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Klicken Sie auf **Landing Pages**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. Unter dem **Einstellungen** Abschnitt, klicken Sie auf **Bearbeiten**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Geben Sie Ihren CNAME in ein. **Domänenname für Einstiegsseiten** eingeben **Fallback-Seite** eingeben **Homepage** und klicken Sie auf **Speichern**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

Auf Ihrer Fallback-Seite werden Personen umgeleitet, wenn Ihre Marketo-Landingpage nicht verfügbar ist.

Gut gemacht! Ihre Landingpages sind jetzt mit Ihrer Unternehmensdomäne gekennzeichnet.
