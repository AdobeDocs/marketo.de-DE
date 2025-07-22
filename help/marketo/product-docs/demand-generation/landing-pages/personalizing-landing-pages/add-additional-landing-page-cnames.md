---
unique-page-id: 2359798
description: Hinzufügen zusätzlicher Landingpage-CNAMEs - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen zusätzlicher Landingpage-CNAMEs
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
feature: Landing Pages
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Hinzufügen zusätzlicher Landingpage-CNAMEs {#add-additional-landing-page-cnames}

Sie können CNAMEs für Landingpages hinzufügen, damit verschiedene URLs auf Ihre Marketo-Landingpages verweisen können. Die folgenden Schritte helfen Ihnen bei der Verwaltung mehrerer Domains.

>[!CAUTION]
>
>Cookies können nicht domänenübergreifend freigegeben werden.

>[!TIP]
>
>**Gleiche Top-Level-Domain - Gut! Cookies werden freigegeben**.<br/> **go**.mycompany.com > **info**.mycompany.com
>
>**Verschiedene Domains auf oberster Ebene - Schlecht! Cookies werden _nicht_ freigegeben**.<br/> los.**mycompany**.com > GO.**mynewcompany**.com

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Navigieren Sie zum Bereich **Admin**.

   ![](assets/add-additional-landing-page-cnames-1.png)

1. Klicken Sie **Mein Konto**.

   ![](assets/add-additional-landing-page-cnames-2.png)

1. Scrollen Sie nach unten zu „Support-Informationen“ und kopieren Sie Ihre Munchkin ID.

   ![](assets/add-additional-landing-page-cnames-3.png)

## Anforderung an IT senden {#send-request-to-it}

1. Bitten Sie Ihre IT-Abteilung, den folgenden CNAME einzurichten: (Ersetzen Sie das Wort [CNAME] durch den CNAME Ihrer Wahl und [Munchkin ID] durch den Text aus dem vorherigen Schritt).

   [CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Neuen CNAME hinzufügen {#add-a-new-cname}

1. Sobald Ihre IT-Abteilung den CNAME erstellt hat, wechseln Sie zum Bereich **Admin**.

   ![](assets/add-additional-landing-page-cnames-4.png)

1. Klicken Sie auf **Landingpages**.

   ![](assets/add-additional-landing-page-cnames-5.png)

1. Klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neuer Domain-Alias]**.

   ![](assets/add-additional-landing-page-cnames-6.png)

1. Geben Sie Ihren **[!UICONTROL Domain-Alias] ein.** Die **[!UICONTROL Standardseite]** wird angezeigt, wenn der Besucher keine URL eingibt. Geben Sie an, wohin sie in diesem Fall gehen sollen.

   >[!NOTE]
   >
   >Für die [!UICONTROL Standardseite] können Sie eine Landingpage oder eine externe URL auswählen, z. B. Ihre öffentliche Website.

   ![](assets/add-additional-landing-page-cnames-7.png)

1. Geben Sie Ihre **[!UICONTROL Standardseite]** ein und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/add-additional-landing-page-cnames-8.png)

Schön! Jetzt wissen Sie, was zu tun ist, wenn Sie jemals einen CNAME hinzufügen möchten.
