---
unique-page-id: 2359746
description: Anpassen der Landingpage-URLs mit einem CNAME - Marketo-Dokumente - Produktdokumentation
title: Anpassen der Landingpage-URLs mit einem CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Anpassen der Landingpage-URLs mit einem CNAME {#customize-your-landing-page-urls-with-a-cname}

Obwohl Marketo Ihre Landingpages hostet, kann die URL vollständig angepasst werden. Wie es ohne CNAME aussieht:

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

So sollte es aussehen:

`https://go.YourCompany.com/UnsubscribePage.html`

## CNAME auswählen {#choose-a-cname}

Wählen Sie ein Wort, das am Anfang der URL Ihrer Landingpages stehen soll. Es ist nur ein Wort und sollte relativ kurz sein. Beispiele:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

Das eine Wort (plus YourCompany.com) wird als CNAME bezeichnet. Sie werden das später benötigen. Notieren Sie es sich also.

## Ermitteln der Munchkin ID {#find-your-munchkin-id}

1. Navigieren Sie zum Bereich **Admin**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Klicken Sie **Mein Konto**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**Administratorberechtigungen erforderlich**

1. Scrollen Sie nach unten zu „Support-Informationen“ und kopieren Sie Ihre Munchkin ID.

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## Anforderung an IT senden {#send-request-to-it}

Bitten Sie Ihre IT-Mitarbeiter, den folgenden CNAME einzurichten: (Ersetzen Sie [ Wort „CNAME] und [Munchkin ID] durch den Text aus dem vorherigen Schritt.)

[CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Abschließen der CNAME-Einrichtung {#complete-cname-setup}

1. Sobald Ihre IT den CNAME erstellt hat, wechseln Sie zum Bereich **Admin** .

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Klicken Sie auf **Landingpages**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. Klicken **im Abschnitt** auf **Bearbeiten**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Geben Sie Ihren CNAME in **Domain-Name für Landingpages**, Ihre **Ausweisseite**, Ihre **Homepage** ein und klicken Sie auf **Speichern**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>Ihre Fallback-Seite ist die Seite, auf die Leads weitergeleitet werden, wenn Ihre Marketo-Landingpage nicht verfügbar ist.

Gute Arbeit! Ihre Landingpages sind jetzt mit der Domain Ihres Unternehmens gekennzeichnet.
