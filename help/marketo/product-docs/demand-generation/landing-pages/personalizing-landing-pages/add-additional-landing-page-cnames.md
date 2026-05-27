---
unique-page-id: 2359798
description: Erfahren Sie, wie Sie in Marketo zusätzliche Landingpage-CNAMEs hinzufügen. Verwenden Sie mehrere benutzerdefinierte Domains für Ihre Landingpages.
title: Hinzufügen zusätzlicher CNAMEs zu einer Landingpage
exl-id: eb5a7f69-552e-49a2-91db-a784f4639cd0
feature: Landing Pages
TQID: https://experienceleague.adobe.com/IhpbLwq0syIQpnKsRApy6YtEKhe56dbDciW8lSYJ9tI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: b2861922f7d2732a3286bab93243bdc0515a5995
workflow-type: tm+mt
source-wordcount: 232
ht-degree: 6%

---

# Hinzufügen zusätzlicher CNAMEs zu einer Landingpage {#add-additional-landing-page-cnames}

Sie können CNAMEs für Landingpages hinzufügen, damit verschiedene URLs auf Ihre Marketo-Landingpages verweisen können. Die folgenden Schritte helfen Ihnen bei der Verwaltung mehrerer Domains.

>[!CAUTION]
>
>Cookies können nicht domänenübergreifend freigegeben werden.

>[!TIP]
>
>**Gleiche Top-Level-Domain - Gut! Cookies werden freigegeben**.<br/> **go**.mycompany.com > **info**.mycompany.com
>
>**Verschiedene Domains auf oberster Ebene - Schlecht! Cookies werden _nicht_ freigegeben**.<br/> go.**mycompany**.com > go.**mynewcompany**.com

>[!NOTE]
>
>**Admin-Berechtigungen erforderlich**

1. Navigieren Sie zum Bereich **Admin**.

   ![](assets/add-additional-landing-page-cnames-1.png)

1. Klicken Sie auf **Mein Konto**.

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

1. Geben Sie Ihren **[!UICONTROL Domain-Alias]** ein. Die **[!UICONTROL Standardseite]** wird angezeigt, wenn der Besucher keine URL eingibt. Geben Sie an, wohin sie in diesem Fall gehen sollen.

   >[!NOTE]
   >
   >Für die [!UICONTROL Standardseite] können Sie eine Landingpage oder eine externe URL auswählen, z. B. Ihre öffentliche Website.

   ![](assets/add-additional-landing-page-cnames-7.png)

1. Geben Sie Ihre **[!UICONTROL Standardseite]** ein und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/add-additional-landing-page-cnames-8.png)

Sie wissen jetzt, wie Sie Ihren Landingpages einen CNAME hinzufügen.
