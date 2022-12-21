---
unique-page-id: 2359798
description: Zusätzliche CNAMEs der Einstiegsseite hinzufügen - Marketo-Dokumente - Produktdokumentation
title: Zusätzliche CNAMEs der Einstiegsseite hinzufügen
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

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

## Konto-Zeichenfolge suchen {#find-your-account-string}

1. Navigieren Sie zu **Admin** Bereich und Klicken **Landing Pages**.

   ![](assets/image2014-9-16-15-3a19-3a54.png)

1. Kopieren Sie die **Kontozeichenfolge** von **Einstellungen** Abschnitt.

   ![](assets/image2014-9-16-15-3a20-3a2.png)

1. Notieren Sie sich das für den nächsten Schritt.

## Anfrage an IT senden {#send-request-to-it}

1. Bitten Sie Ihre IT-Abteilung, den folgenden CNAME einzurichten: (Ersetzen Sie das Wort [CNAME] mit dem CNAME Ihrer Wahl und [KONTOZEICHENFOLGE] mit dem Text aus dem vorherigen Schritt).

   [CNAME].YourCompany.com > [KONTOZEICHENFOLGE].mktoweb.com

## Neuen CNAME hinzufügen {#add-a-new-cname}

1. Sobald Ihre IT-Abteilung den CNAME erstellt hat, gehen Sie zu **Admin** Klicken Sie dann auf **Landing Pages**.

   ![](assets/image2014-9-16-15-3a20-3a20.png)

1. Klicken **Neu** und wählen Sie **Neuer Domänenname**.

   ![](assets/image2014-9-16-15-3a20-3a28.png)

1. Geben Sie Ihre **Domänen-Alias.** Die **Standardseite** angezeigt, wenn der Besucher keine URL eingibt. Geben Sie an, wohin der Benutzer in diesem Fall wechseln sollte.

   >[!NOTE]
   >
   >Für die Standardseite können Sie eine Landingpage oder eine externe URL auswählen, z. B. Ihre öffentliche Website.

   ![](assets/image2014-9-16-15-3a20-3a36.png)

1. Geben Sie Ihre **Standardseite** und klicken Sie auf **Erstellen**.

   ![](assets/image2014-9-16-15-3a20-3a43.png)

Gut! Jetzt wissen Sie, was zu tun ist, wenn Sie jemals einen CNAME hinzufügen möchten.
