---
unique-page-id: 2359918
description: Einstellungen für die Landingpage bearbeiten - Marketing Docs - Produktdokumentation
title: Einstellungen für Landingpages bearbeiten
translation-type: tm+mt
source-git-commit: f79909ce8f2e37bf0748596774fe47ac03618696
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Einstellungen für Landingpages bearbeiten {#edit-landing-page-settings}

Sie können Ihren Domänennamen und Ihre Ausweichseite bearbeiten, das Vorausfüllen von Formularen aktivieren oder deaktivieren, Missbrauch Ihrer Landingpage verhindern und vieles mehr. So geht es.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Klicken Sie unter **Admin** auf **Landingpages**.

   ![](assets/image2014-9-10-9-3a47-3a40.png)

1. Klicken Sie im Abschnitt **Landingpages** auf **Bearbeiten**.

   ![](assets/image2014-9-10-9-3a47-3a12.png)

1. Geben Sie Ihre Domäne und Seiteninformationen ein.

   | Begriff | Definition |
   |---|---|
   | Domänenname für Landingpages | Das ist Ihr CNAME. Ein CNAME ist der erste Teil der URL, die Sie Personen für Landingpages angeben. Beispiel: In `http://go.yourCompany.com` ist das Wort &quot;go&quot;der CNAME. Man kann mehrere haben, aber die meisten Leute verwenden nur das eine. |
   | Fallback-Seite | Hier muss man gehen, wenn die Landingpage nicht existiert oder nicht da ist. Erfahren Sie mehr über [Ausweichseiten](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | Homepage | Geben Sie Ihre Unternehmens-Site-URL ein. |

   ![](assets/three.png)

1. Markieren Sie das Kontrollkästchen **Formularvorausfüllung**, damit Formulare Informationen für bekannte (Cookie-)Personen vorab ausfüllen können. Deaktivieren, um zu blockieren.

   ![](assets/four.png)

1. Wenn Sie verhindern möchten, dass böswillige Seiten Ihren Inhalt scheinbar hosten, aktivieren Sie das Kontrollkästchen **Marketo-Seiten nicht in externe Webseiten** einbetten lassen.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Wenn das Tag &quot;`<script>`&quot;am Ende des Tags &quot;`<head>`&quot;im Code angezeigt werden soll, markieren Sie das Kontrollkästchen &quot;**Skript zum Vorausfüllen am Ende der Überschrift**&quot;einfügen. Lassen Sie das Kontrollkästchen deaktiviert, wenn es am Anfang erscheinen soll.
   >
   >Markieren Sie **Entfernen Sie die standardmäßigen Favicon-Links**, um zu verhindern, dass Marketo Favicon-Links in den Code einfügt.

1. Klicken Sie nach der Auswahl auf **Speichern.**

   ![](assets/six.png)

   Gute Arbeit! Ihre Landingpages haben jetzt die richtigen Informationen und sollten Beginn sofort arbeiten.
