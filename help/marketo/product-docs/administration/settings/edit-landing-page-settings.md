---
unique-page-id: 2359918
description: Landingpage-Einstellungen bearbeiten - Marketo-Dokumente - Produktdokumentation
title: Bearbeiten der Landingpage-Einstellungen
exl-id: 019b4651-3a66-46f9-8722-66af30194380
feature: Administration, Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 6%

---

# Bearbeiten der Landingpage-Einstellungen {#edit-landing-page-settings}

Sie können Ihren Domain-Namen und die Fallback-Seite bearbeiten, das Vorbefüllen von Formularen aktivieren oder deaktivieren, einen Missbrauch Ihrer Landingpage verhindern und vieles mehr. Und so geht das.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/edit-landing-page-settings-1.png)

1. Klicken Sie auf **[!UICONTROL Landingpages]**.

   ![](assets/edit-landing-page-settings-2.png)

1. Klicken Sie **[!UICONTROL Abschnitt &quot;]**&quot; auf **[!UICONTROL Bearbeiten]**.

   ![](assets/edit-landing-page-settings-3.png)

1. Geben Sie Ihre Domain- und Seiteninformationen ein.

   ![](assets/edit-landing-page-settings-4.png)

   | Begriff | Definition |
   |---|---|
   | [!UICONTROL Domain-Name für Landingpages] | Dies ist Ihr CNAME. Ein CNAME ist der erste Teil der URL, die Sie Personen für Landingpages geben. In `https://go.yourCompany.com` ist beispielsweise das Wort „go“ der CNAME. Man kann mehrere haben, aber die meisten Leute benutzen nur den einen. |
   | [!UICONTROL Fallback-Seite] | Hier geht es, wenn die Landingpage nicht vorhanden oder ausgefallen ist. Weitere Informationen zu [Fallback-Seiten](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | [!UICONTROL Startseite] | Geben Sie die URL Ihrer Unternehmens-Site ein. |

1. Aktivieren Sie das **[!UICONTROL Formular vorbefüllen]**, damit Formulare Informationen für bekannte (Cookie-)Personen vorbefüllen können. Deaktivieren Sie diese Option, um zu blockieren.

   ![](assets/edit-landing-page-settings-5.png)

   >[!NOTE]
   >
   >Wenn das Tag `<script>` Vorbefüllungs-Code am Ende des `<head>`-Tags im Code angezeigt werden soll, aktivieren Sie das Kontrollkästchen **[!UICONTROL Vorbefüllungs-Skript am Ende des]** einfügen. Deaktivieren Sie diese Option, wenn sie am Anfang angezeigt werden soll.
   >
   >Aktivieren Sie **[!UICONTROL Standard-Favicon-Links entfernen]**, um zu verhindern, dass Marketo Favicon-Links in den Code einfügt.

1. Klicken Sie nach der Auswahl auf **[!UICONTROL Speichern]**.

   ![](assets/edit-landing-page-settings-6.png)

   Gut gemacht! Ihre Landingpages verfügen jetzt über die richtigen Informationen und sollten sofort mit der Arbeit beginnen.
