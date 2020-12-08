---
unique-page-id: 2950555
description: Einstellungen für reichhaltige Beiträge bearbeiten - Marketing-Dokumente - Produktdokumentation
title: Einstellungen für Facebook-Rich-Beiträge bearbeiten
translation-type: tm+mt
source-git-commit: 44ed91b485b52173922c709de63a4353e16c5072
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---


# Einstellungen für Facebook-Rich-Beiträge bearbeiten {#edit-facebook-rich-post-settings}

Passen Sie Beiträge an, wenn Personen Sie auf Facebook [freigeben](http://docs.marketo.com/display/docs/social) .

>[!NOTE]
>
>**Verfügbarkeit**
>
>Nicht alle Kunden haben diese Funktion erworben. Weitere Informationen erhalten Sie von Ihrem Vertriebsmitarbeiter.

Mit Marketo- [Social-Apps](http://docs.marketo.com/display/docs/social) können Ihre Interessenten Ihre Landingpages mit ihren Verbindungen in sozialen Netzwerken wie Facebook, Twitter usw. teilen. Mit den Facebook OpenGraph-Tags (OG-Tags) können Sie angeben, welche Informationen aus Ihrer Landingpage in Facebook-Beiträgen enthalten sind.

## Rich-Post-Optionen auswählen {#select-rich-post-options}

Sie können die Arten von Seiteninformationen angeben, die in den Facebook-Rich-Posts verwendet werden sollen, die von Teilen Ihrer Landingpage generiert wurden.

1. Wählen Sie **Facebook-Nachricht** im Editor für Ihr **YouTube** -Video oder Ihre Social-Schaltfläche aus.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Wählen Sie aus den folgenden Optionen für Ihre Facebook-Nachricht aus.

   * hinzufügen statischen Inhalt: Wählen Sie diese Option, um den Titel, die Beschriftung und die Beschreibung manuell einzugeben.

      ![](assets/image2014-9-22-16-3a48-3a0.png)

   * hinzufügen dynamischer Inhalt: Ihre Social-App kann Ihren Rich-Post mit den Tags `<TITLE>`, `<CAPTION>`und `<DESCRIPTION>` Tags Ihrer Landingpage füllen.

      ![](assets/image2014-9-22-16-3a48-3a9.png)
   >[!NOTE]
   >
   >Diese sollten bereits in der Seitenquelle vorhanden sein, aber für mehr Kontrolle können Sie Ihrer Landingpage [bestimmte Facebook-OG-Tags](edit-facebook-rich-post-settings.md)hinzufügen.

   * Fügen Sie keinen Rich Content hinzu: Begrenzt die Facebook-Beiträge von Ihrer Landingpage auf die Hauptnachricht und den Link.

      ![](assets/image2014-9-22-16-3a48-3a18.png)



## hinzufügen von Facebook-OG-Tags zu einer Landingpage {#add-facebook-og-tags-to-a-landing-page}

Um die Seitenelemente zu steuern, die in den Facebook-Teilen Ihrer Landingpage enthalten sein werden, können Sie Ihrer Landingpage Facebook OG-Tags (Open Graph) für Titel, Beschriftung und Beschreibung hinzufügen.

1. Öffnen Sie die Landingpage, die Ihr **YouTube-Video** oder Ihre Social-Schaltfläche enthält.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   Der **Landingpages-Designer** wird in einem neuen Fenster geöffnet.

1. Wählen Sie &quot; **Landingpages-Aktionen** &quot;> &quot;Seitenmeta-Tags **bearbeiten*****.**.*

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. hinzufügen HTML, das og:title, og:caption und og:description definiert. Kopieren Sie die folgenden Zeilen und ersetzen Sie den Platzhaltertext:

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Achten Sie darauf, beim Hinzufügen der OG-Tags die richtige HTML-Syntax zu verwenden.
