---
unique-page-id: 2359746
description: Passen Sie Ihre Landingpage-URLs mit einem CNAME an - Marketo Docs - Produktdokumentation
title: Anpassen der Landingpage-URLs mit einem CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 3%

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

## Munchkin-ID suchen {#find-your-munchkin-id}

1. Navigieren Sie zum **Admin**-Bereich.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Klicks **Mein Konto**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**Erforderliche Administratorberechtigungen**

1. Scrollen Sie nach unten zu &quot;Support-Informationen&quot;und kopieren Sie Ihre Munchkin-ID.

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## Anfrage an IT senden {#send-request-to-it}

Bitten Sie Ihre IT-Mitarbeiter, den folgenden CNAME einzurichten: (Ersetzen Sie das Wort: [CNAME] und [Munchkin-ID] mit dem Text aus dem vorherigen Schritt.)

[CNAME].YourCompany.com > [Munchkin-ID].mktoweb.com

## Vollständige CNAME-Einrichtung {#complete-cname-setup}

1. Nachdem Ihre IT den CNAME erstellt hat, wechseln Sie zum **Admin** Bereich.

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Klicken Sie auf **Landing Pages**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. Unter dem **Einstellungen** Abschnitt, klicken Sie auf **Bearbeiten**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Geben Sie Ihren CNAME in ein. **Domänenname für Einstiegsseiten** eingeben **Fallback-Seite** eingeben **Homepage** und klicken **Speichern**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>Ihre Fallback-Seite ist die Seite, an die Leads weitergeleitet werden, wenn Ihre Marketo-Landingpage nicht verfügbar ist.

Gut gemacht! Ihre Landingpages sind jetzt mit Ihrer Unternehmensdomäne gekennzeichnet.
