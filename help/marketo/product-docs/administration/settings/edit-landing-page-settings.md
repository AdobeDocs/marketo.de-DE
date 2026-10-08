---
unique-page-id: 2359918
description: Anleitung zum Bearbeiten von Domain-Namen, Fallback-Seite, vorausgefülltem Formular und anderen Landingpage-Optionen.
title: Bearbeiten der Landingpage-Einstellungen
exl-id: 019b4651-3a66-46f9-8722-66af30194380
feature: Administration, Landing Pages
TQID: 'https://experienceleague.adobe.com/dOvxpv09JPPBMNjqA0JTe-L4wIWUtkEELLl-PCs4CME'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: edda586e-0147-48f2-b791-992622a00783
    internal-label: Landing pages
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 7%
---
# Bearbeiten der Landingpage-Einstellungen {#edit-landing-page-settings}

Sie können Ihren Domain-Namen und die Fallback-Seite bearbeiten, das Vorbefüllen von Formularen aktivieren oder deaktivieren, einen Missbrauch Ihrer Landingpage verhindern und vieles mehr. Gehen Sie wie folgt vor.

>[!NOTE]
>
>**Admin-Berechtigungen erforderlich**

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
   | [!UICONTROL Domain-Name für Landingpages] | Dies ist Ihr CNAME. Ein CNAME ist der erste Teil der URL, die Sie Personen für Landingpages geben. In `https://go.yourCompany.com` ist beispielsweise das Wort „go“ der CNAME. Man kann mehrere haben, aber die meisten Leute benutzen nur eine. |
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

   Ihre Landingpages verfügen jetzt über die richtigen Informationen und sollten sofort funktionieren.
