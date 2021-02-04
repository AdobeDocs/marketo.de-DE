---
unique-page-id: 2359798
description: hinzufügen CNAMEs zusätzlicher Landingpages - Marketing Docs - Produktdokumentation
title: hinzufügen CNAMEs zusätzlicher Landingpages
translation-type: tm+mt
source-git-commit: 2969e6f94f5fd781e2167ae2aa8680bb8d134754
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---


# hinzufügen zusätzliche Landingpage CNAMEs {#add-additional-landing-page-cnames}

Möglicherweise möchten Sie CNAMEs der Landingpage hinzufügen, damit verschiedene URLs auf Ihre Marketo-Landingpages verweisen können. Gehen Sie wie folgt vor, um mehrere Domänen zu verwalten.

>[!CAUTION]
>
>Cookies können nicht domänenübergreifend verwendet werden.

>[!TIP]
>
>**Gleiche Domäne auf oberster Ebene - Gut! Cookies werden freigegeben**.<br/> **go**.mycompany.com >  **info**.mycompany.com
>
>**Verschiedene Top Level Domains - Schlecht! Cookies sind _nicht_ freigegeben**.<br/> gehen.**mycompany**.com > go.**mynewcompany**.com

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Suchen Sie Ihre Kontozeichenfolge {#find-your-account-string}

1. Wechseln Sie zum Bereich **Admin** und klicken Sie auf **Landingpages**.

   ![](assets/image2014-9-16-15-3a19-3a54.png)

1. Kopieren Sie die **Kontozeichenfolge** aus dem Abschnitt **Einstellungen**.

   ![](assets/image2014-9-16-15-3a20-3a2.png)

1. Notieren Sie sich dies für den nächsten Schritt.

## Anforderung an IT senden {#send-request-to-it}

1. Bitten Sie Ihre IT-Abteilung, den folgenden CNAME einzurichten: (Ersetzen Sie das Wort [CNAME] durch den CNAME Ihrer Wahl und [ACCOUNT STRING] durch den Text aus dem vorherigen Schritt).

   [CNAME].YourCompany.com >  [ACCOUNT STRING].mktoweb.com

## hinzufügen eines neuen CNAME {#add-a-new-cname}

1. Nachdem die IT-Abteilung den CNAME erstellt hat, gehen Sie zu **Admin** und klicken Sie dann auf **Landingpages**.

   ![](assets/image2014-9-16-15-3a20-3a20.png)

1. Klicken Sie auf **Neu** und wählen Sie **Neue Domänenalias**.

   ![](assets/image2014-9-16-15-3a20-3a28.png)

1. Geben Sie Ihren **Domänenalias ein.** Die  **Standardseite** wird angezeigt, wenn der Besucher keine URL eingibt. Geben Sie an, wohin sie in diesem Fall gehen sollten.

   >[!NOTE]
   >
   >Für die Standardseite können Sie eine Landingpage oder eine externe URL auswählen, z. B. Ihre öffentliche Website.

   ![](assets/image2014-9-16-15-3a20-3a36.png)

1. Geben Sie Ihre **Standardseite** ein und klicken Sie auf **Erstellen**.

   ![](assets/image2014-9-16-15-3a20-3a43.png)

Schön! Jetzt wissen Sie, was zu tun ist, wenn Sie jemals einen CNAME hinzufügen möchten.
