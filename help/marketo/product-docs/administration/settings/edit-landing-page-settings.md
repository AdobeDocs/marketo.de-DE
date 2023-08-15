---
unique-page-id: 2359918
description: Bearbeiten von Einstellungen für Landingpages - Marketo-Dokumente - Produktdokumentation
title: Einstellungen der Landingpage bearbeiten
exl-id: 019b4651-3a66-46f9-8722-66af30194380
feature: Administration, Landing Pages
source-git-commit: 43565104a7f6512d2f99eae6bc47e1ae048b2231
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 6%

---

# Einstellungen der Landingpage bearbeiten {#edit-landing-page-settings}

Sie können Ihren Domänennamen und Ihre Fallback-Seite bearbeiten, das Vorausfüllen von Formularen aktivieren oder deaktivieren, Missbrauch bei Landingpages verhindern und vieles mehr. So geht es.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

1. Navigieren Sie zum **[!UICONTROL Admin]**-Bereich.

   ![](assets/edit-landing-page-settings-1.png)

1. Klicken Sie auf **[!UICONTROL Landing Pages]**.

   ![](assets/edit-landing-page-settings-2.png)

1. Im **[!UICONTROL Landing Pages]** Abschnitt, klicken Sie auf **[!UICONTROL Bearbeiten]**.

   ![](assets/edit-landing-page-settings-3.png)

1. Geben Sie Ihre Domäne und Seiteninformationen ein.

   ![](assets/edit-landing-page-settings-4.png)

   | Begriff | Definition |
   |---|---|
   | [!UICONTROL Domänenname für Landingpages] | Dies ist Ihr CNAME. Ein CNAME ist der erste Teil der URL, die Sie Personen für Landingpages geben. Beispiel: in `https://go.yourCompany.com`, ist das Wort &quot;go&quot;der CNAME. Sie können mehrere haben, aber die meisten verwenden nur die. |
   | [!UICONTROL Fallback-Seite] | Hier können Sie einsteigen, wenn die Landingpage nicht vorhanden oder nicht vorhanden ist. Weitere Informationen [Fallback-Seiten](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | [!UICONTROL Startseite] | Geben Sie Ihre Unternehmens-Site-URL ein. |

1. Überprüfen Sie die **[!UICONTROL Vorab ausfüllen]** aktivieren, damit Formulare Informationen für bekannte (Cookies) Personen vorbefüllen können. Deaktivieren Sie die Option zum Blockieren.

   ![](assets/edit-landing-page-settings-5.png)

   >[!NOTE]
   >
   >Wenn Sie die Vorbefüllung vornehmen möchten `<script>` -Tag, das am Ende der `<head>` -Tag im Code, überprüfen Sie die **[!UICONTROL Skript zum Vorfüllen am Ende des Kopfes einfügen]** ankreuzen. Lassen Sie die Option deaktiviert, wenn sie am Anfang angezeigt werden soll.
   >
   >Überprüfen **[!UICONTROL Standardmäßige Favicon-Links entfernen]** um zu verhindern, dass Marketo Favicon-Links in den Code einfügt.

1. Klicken Sie nach der Auswahl auf **[!UICONTROL Speichern]**.

   ![](assets/edit-landing-page-settings-6.png)

   Gut gemacht! Ihre Landingpages verfügen jetzt über die richtigen Informationen und sollten sofort mit der Arbeit beginnen.
