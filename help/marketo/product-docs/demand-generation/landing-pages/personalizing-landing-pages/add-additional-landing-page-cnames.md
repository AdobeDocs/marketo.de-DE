---
unique-page-id: 2359798
description: Zusätzliche CNAMEs der Einstiegsseite hinzufügen - Marketo-Dokumente - Produktdokumentation
title: Zusätzliche CNAMEs der Einstiegsseite hinzufügen
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
source-git-commit: 6c1699ce986608e8b9d991f21fd649f9330e3d12
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 3%

---

# Zusätzliche CNAMEs der Einstiegsseite hinzufügen {#add-additional-landing-page-cnames}

Möglicherweise möchten Sie Landingpage-CNAMEs hinzufügen, damit unterschiedliche URLs auf Ihre Marketo-Landingpages verweisen können. Die folgenden Schritte helfen Ihnen bei der Verwaltung mehrerer Domänen.

>[!CAUTION]
>
>Cookies können nicht domänenübergreifend verwendet werden.

>[!TIP]
>
>**Dieselbe Top-Level-Domain - Gut! Cookies werden freigegeben**.<br/> **go**.mycompany.com > **Info**.mycompany.com
>
>**Verschiedene Top-Level-Domains - Schlecht! Cookies sind _not_ shared**.<br/> gehen.**mycompany**.com > go.**mynewcompany**.com

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

1. Navigieren Sie zum **Admin**-Bereich.

   ![](assets/add-additional-landing-page-cnames-1.png)

1. Klicken **Mein Konto**.

   ![](assets/add-additional-landing-page-cnames-2.png)

1. Scrollen Sie nach unten zu &quot;Support-Informationen&quot;und kopieren Sie Ihre Munchkin-ID.

   ![](assets/add-additional-landing-page-cnames-3.png)

## Anfrage an IT senden {#send-request-to-it}

1. Bitten Sie Ihre IT-Abteilung, den folgenden CNAME einzurichten: (Ersetzen Sie das Wort [CNAME] mit dem CNAME Ihrer Wahl und [Munchkin-ID] mit dem Text aus dem vorherigen Schritt).

   [CNAME].YourCompany.com > [Munchkin-ID].mktoweb.com

## Neuen CNAME hinzufügen {#add-a-new-cname}

1. Nachdem Ihre IT-Abteilung den CNAME erstellt hat, wechseln Sie zum **Admin** Bereich.

   ![](assets/add-additional-landing-page-cnames-4.png)

1. Klicken Sie auf **Landing Pages**.

   ![](assets/add-additional-landing-page-cnames-5.png)

1. Klicken **Neu** und wählen Sie **Neuer Domänenname**.

   ![](assets/add-additional-landing-page-cnames-6.png)

1. Geben Sie Ihre **Domänen-Alias.** Die **Standardseite** angezeigt, wenn der Besucher keine URL eingibt. Geben Sie an, wohin der Benutzer in diesem Fall wechseln sollte.

   >[!NOTE]
   >
   >Für die Standardseite können Sie eine Landingpage oder eine externe URL auswählen, z. B. Ihre öffentliche Website.

   ![](assets/add-additional-landing-page-cnames-7.png)

1. Geben Sie Ihre **Standardseite** und klicken Sie auf **Erstellen**.

   ![](assets/add-additional-landing-page-cnames-8.png)

Gut! Jetzt wissen Sie, was zu tun ist, wenn Sie jemals einen CNAME hinzufügen möchten.
