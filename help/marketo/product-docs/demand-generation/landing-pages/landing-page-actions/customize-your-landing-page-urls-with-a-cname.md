---
unique-page-id: 2359746
description: Passen Sie Ihre Landingpage-URLs mit einem CNAME an - Marketo Docs - Produktdokumentation
title: Anpassen der Landingpage-URLs mit einem CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
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

## Munchkin-ID suchen {#find-your-munchkin-id}

1. Wechseln Sie zum Bereich **Admin** .

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Klicken Sie auf **Mein Konto**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**Erforderliche Administratorberechtigungen**

1. Scrollen Sie nach unten zu &quot;Support-Informationen&quot;und kopieren Sie Ihre Munchkin-ID.

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## Anfrage an IT senden {#send-request-to-it}

Bitten Sie Ihre IT-Mitarbeiter, den folgenden CNAME einzurichten: (Ersetzen Sie das Wort [CNAME] und [Munchkin ID] durch den Text aus dem vorherigen Schritt.)

[CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Vollständige CNAME-Einrichtung {#complete-cname-setup}

1. Nachdem Ihr IT-Mitarbeiter den CNAME erstellt hat, wechseln Sie zum Bereich **Admin** .

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Klicken Sie auf **Landingpages**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. Klicken Sie unter dem Abschnitt **Einstellungen** auf **Bearbeiten**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Geben Sie Ihren CNAME in **Domänennamen für Einstiegsseiten** ein, geben Sie Ihre **Fallback-Seite** ein, geben Sie Ihre **Homepage** ein und klicken Sie auf **Speichern**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>Ihre Fallback-Seite ist die Seite, an die Leads weitergeleitet werden, wenn Ihre Marketo-Landingpage nicht verfügbar ist.

Gut gemacht! Ihre Landingpages sind jetzt mit Ihrer Unternehmensdomäne gekennzeichnet.
