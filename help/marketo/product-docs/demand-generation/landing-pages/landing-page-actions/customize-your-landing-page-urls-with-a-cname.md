---
unique-page-id: 2359746
description: Erfahren Sie, wie Sie in Marketo Landingpage-URLs mit einem CNAME anpassen. Eigene Domain für Landingpage-Links verwenden
title: Benutzerdefinierte Landingpage-URLs mit einem CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
feature: Landing Pages
TQID: 'https://experienceleague.adobe.com/8G3a-7YZlycD5xXJLqlny12XL7M-T2ouYDhjBnRAMfo'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: edda586e-0147-48f2-b791-992622a00783
    internal-label: Landing pages
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 9%
---
# Benutzerdefinierte Landingpage-URLs mit einem CNAME {#customize-your-landing-page-urls-with-a-cname}

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

1. Klicken Sie auf **Mein Konto**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**Admin-Berechtigungen erforderlich**

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

1. Geben Sie Ihren CNAME in **[!UICONTROL Domain-Name für Landingpages]**, Ihre **[!UICONTROL Ausweisseite]**, Ihre **[!UICONTROL Homepage]** ein und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>Ihre Fallback-Seite ist die Seite, auf die Leads weitergeleitet werden, wenn Ihre Marketo-Landingpage nicht verfügbar ist.

Ihre Landingpages sind jetzt mit der Domain Ihres Unternehmens gekennzeichnet.
