---
unique-page-id: 2950555
description: Facebook Rich-Post-Einstellungen bearbeiten - Marketo-Dokumente - Produktdokumentation
title: Bearbeiten von Facebook Rich-Post-Einstellungen
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
feature: Integrations
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

# Bearbeiten von Facebook Rich-Post-Einstellungen {#edit-facebook-rich-post-settings}

Passen Sie Beiträge an, wenn Benutzer Sie in Facebook freigeben.

>[!AVAILABILITY]
>
>Nicht alle Marketo Engage-Benutzer haben diese Funktion erworben. Weitere Informationen erhalten Sie vom Adobe Account Team (Ihrem Kundenbetreuer).

Marketo [Social Apps](/help/marketo/product-docs/demand-generation/social/social-functions/add-a-social-button-on-a-landing-page.md) ermöglichen es Leads, Ihre Landingpages mit ihren Verbindungen in sozialen Netzwerken wie Facebook, Twitter usw. zu teilen. Mit facebook OpenGraph-Tags (OG-Tags) können Sie angeben, welche Informationen von Ihrer Landingpage in Facebook-Beiträgen enthalten sind.

## Rich-Post-Optionen auswählen {#select-rich-post-options}

Sie können die Arten von Seiteninformationen angeben, die in den Rich-Posts von Facebook verwendet werden sollen, die von Teilen aus Ihrer Landingpage generiert wurden.

1. Auswählen **Facebook-Nachricht** im Editor für **YouTube** Video- oder Social-Schaltfläche.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Wählen Sie eine der folgenden Optionen für Ihre Facebook-Nachricht aus.

   * Statischen Inhalt hinzufügen: Wählen Sie diese Option aus, um den Titel, die Beschriftung und die Beschreibung manuell einzugeben.

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Dynamischen Inhalt hinzufügen: Ihre Social-App kann die `<TITLE>`, `<CAPTION>`, und `<DESCRIPTION>` Tags zum Ausfüllen Ihres Rich-Posts.

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >Diese sollten bereits in der Seitenquelle vorhanden sein. Für mehr Kontrolle können Sie Ihrer Landingpage jedoch bestimmte Facebook OG-Tags hinzufügen.

   * Rich-Content nicht hinzufügen: Beschränkt die Facebook-Beiträge von Ihrer Landingpage auf die Hauptnachricht und den Link.

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## Hinzufügen von Facebook OG-Tags zu einer Landingpage {#add-facebook-og-tags-to-a-landing-page}

Um die Seitenelemente zu steuern, die in den Facebook-Freigaben von Ihrer Landingpage enthalten sein werden, können Sie Ihrer Landingpage Facebook OG (Open Graph)-Tags für Titel, Beschriftung und Beschreibung hinzufügen.

1. Öffnen Sie die Landingpage, die Ihre **YouTube-Video** oder &quot;Social&quot;.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   Die **Landingpage-Designer** in einem neuen Fenster geöffnet.

1. Auswählen **Landingpage-Aktionen** > **Bearbeiten von Seiten-Meta-Tags**.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Fügen Sie die HTML hinzu, die og:title, og:caption und og:description definiert. Kopieren Sie diese Zeilen und fügen Sie sie ein und ersetzen Sie den Platzhaltertext:

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Achten Sie beim Hinzufügen der OG-Tags auf die Verwendung der richtigen HTML-Syntax.
