---
unique-page-id: 2359798
description: Zusätzliche CNAMEs der Einstiegsseite hinzufügen - Marketo-Dokumente - Produktdokumentation
title: Zusätzliche CNAMEs der Einstiegsseite hinzufügen
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Zusätzliche CNAMEs der Einstiegsseite hinzufügen {#add-additional-landing-page-cnames}

Möglicherweise möchten Sie Landingpage-CNAMEs hinzufügen, damit unterschiedliche URLs auf Ihre Marketo-Landingpages verweisen können. Die folgenden Schritte helfen Ihnen bei der Verwaltung mehrerer Domänen.

>[!CAUTION]
>
>Cookies können nicht domänenübergreifend verwendet werden.

>[!TIP]
>
>**Dieselbe Domäne auf oberster Ebene - Gut! Cookies werden freigegeben**.<br/> **go**.mycompany.com > **info**.mycompany.com
>
>**Verschiedene Top-Level-Domänen - Schlecht! Cookies sind _nicht_ freigegeben**.<br/> los.**mycompany**.com > go.**mynewcompany**.com

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

1. Wechseln Sie zum Bereich **Admin** .

   ![](assets/add-additional-landing-page-cnames-1.png)

1. Klicken Sie auf **Mein Konto**.

   ![](assets/add-additional-landing-page-cnames-2.png)

1. Scrollen Sie nach unten zu &quot;Support-Informationen&quot;und kopieren Sie Ihre Munchkin-ID.

   ![](assets/add-additional-landing-page-cnames-3.png)

## Anfrage an IT senden {#send-request-to-it}

1. Bitten Sie Ihre IT-Abteilung, den folgenden CNAME einzurichten: (Ersetzen Sie das Wort [CNAME] durch den CNAME Ihrer Wahl und [Munchkin ID] durch den Text aus dem vorherigen Schritt).

   [CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Neuen CNAME hinzufügen {#add-a-new-cname}

1. Nachdem Ihre IT-Abteilung den CNAME erstellt hat, wechseln Sie zum Bereich **Admin** .

   ![](assets/add-additional-landing-page-cnames-4.png)

1. Klicken Sie auf **Landingpages**.

   ![](assets/add-additional-landing-page-cnames-5.png)

1. Klicken Sie auf **Neu** und wählen Sie dann **Neuer Domänenname** aus.

   ![](assets/add-additional-landing-page-cnames-6.png)

1. Geben Sie Ihren **Domänennamen-Alias ein.** Die **Standardseite** wird angezeigt, wenn der Besucher keine URL eingibt. Geben Sie an, wohin der Benutzer in diesem Fall wechseln sollte.

   >[!NOTE]
   >
   >Für die Standardseite können Sie eine Landingpage oder eine externe URL auswählen, z. B. Ihre öffentliche Website.

   ![](assets/add-additional-landing-page-cnames-7.png)

1. Geben Sie Ihre **Standardseite** ein und klicken Sie auf **Erstellen**.

   ![](assets/add-additional-landing-page-cnames-8.png)

Gut! Jetzt wissen Sie, was zu tun ist, wenn Sie jemals einen CNAME hinzufügen möchten.
