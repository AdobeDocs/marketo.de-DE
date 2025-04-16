---
unique-page-id: 2950555
description: Facebook-Rich-Post-Einstellungen bearbeiten - Marketo-Dokumente - Produktdokumentation
title: Rich-Post-Einstellungen für Facebook bearbeiten
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
hide: true
hidefromtoc: true
feature: Integrations
source-git-commit: 7a8f5146126d6e8a4902be9337eef4d51e108cf0
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

# Rich-Post-Einstellungen für Facebook bearbeiten {#edit-facebook-rich-post-settings}

Passen Sie Beiträge an, wenn Personen Sie auf Facebook teilen.

>[!AVAILABILITY]
>
>Nicht alle Marketo Engage-Benutzer haben diese Funktion erworben. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).

Marketo Mit _(Social_ Apps) können Ihre Leads Ihre Landingpages über ihre Verbindungen in sozialen Netzwerken wie Facebook, Twitter usw. teilen. Mit Facebook OpenGraph Tags (OG-Tags) können Sie festlegen, welche Informationen aus Ihrer Landingpage in Facebook-Posts enthalten sind.

## Rich-Post-Optionen auswählen {#select-rich-post-options}

Sie können die Arten von Seiteninformationen angeben, die in den Rich-Posts von Facebook verwendet werden sollen, die durch Freigaben auf Ihrer Landingpage generiert werden.

1. Wählen Sie **Facebook-Nachricht** im Editor für Ihr **YouTube**-Video oder Ihren Social-Media-Button aus.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Wählen Sie für Ihre Facebook-Nachricht eine der folgenden Optionen aus.

   * Statischen Inhalt hinzufügen: Wählen Sie diese Option aus, um den Titel, die Beschriftung und die Beschreibung manuell einzugeben.

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Dynamische Inhalte hinzufügen: Ihre Social-Media-App kann die `<TITLE>`-, `<CAPTION>`- und `<DESCRIPTION>`-Tags Ihrer Landingpage verwenden, um Ihren Rich-Post zu füllen.

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >Diese sollten bereits in der Quellseite der Seite vorhanden sein. Um mehr Kontrolle zu haben, können Sie Ihrer Landingpage jedoch bestimmte Facebook-OG-Tags hinzufügen.

   * Keinen umfangreichen Inhalt hinzufügen: Beschränkt die Facebook-Posts von Ihrer Landingpage auf die Hauptnachricht und den Link.

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## Hinzufügen von Facebook-OG-Tags zu einer Landingpage {#add-facebook-og-tags-to-a-landing-page}

Um die Seitenelemente zu steuern, die in den Facebook-Freigaben von Ihrer Landingpage aus enthalten sein werden, können Sie Ihrer Landingpage Facebook-OG-Tags (Open Graph) für Titel, Beschriftung und Beschreibung hinzufügen.

1. Öffnen Sie die Landingpage, die Ihr **YouTube-Video** Social-Media-Button enthält.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   Die **Landingpage Designer** wird in einem neuen Fenster geöffnet.

1. Wählen Sie **Landingpage-Aktionen** > **Bearbeiten von Seiten-Meta-Tags** aus.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Fügen Sie die HTML hinzu, die og:title, og:caption und og:description definiert. Kopieren Sie diese Zeilen, fügen Sie sie ein und ersetzen Sie den Platzhaltertext:

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Achten Sie beim Hinzufügen der OG-Tags darauf, die richtige HTML-Syntax zu verwenden.
