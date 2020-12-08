---
unique-page-id: 11385579
description: Erstellen von Inhaltsmustern - Marketing-Dokumente - Produktdokumentation
title: Inhaltsmuster erstellen
translation-type: tm+mt
source-git-commit: f28ff1acb0090892bdb92b75ef90d489db7abf20
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---


# Inhaltsmuster erstellen {#create-content-patterns}

>[!NOTE]
>
>Je nach Kaufdatum kann Ihr Marketing-Abonnement entweder Marketing-to-Predictive-Inhalte oder Inhalte`<sup>AI</sup>`enthalten. Für Personen, die Predictive Content verwenden, aktiviert Marketing bis zum 30. April 2018 Content`<sup>AI</sup>` Analytics-Funktionen. Wenden Sie sich an Ihren Marketing-Kundenbetreuer, um ein Upgrade auf Marketing-Inhalte`<sup>AI</sup>`durchzuführen, damit diese Funktionen über das entsprechende Datum hinausgehen.

Wenn Sie Inhaltsmuster festlegen, werden Inhalte automatisch erkannt, wenn ein Besucher auf die HTML-Webseite klickt, die für das Inhaltsmuster relevant ist. Es wird verwendet, um HTML-Seiten (Blog-Beiträge, Pressemitteilungen, News-Artikel) als Inhaltselemente zur Seite &quot;Alle Inhalte&quot;hinzuzufügen. Wenn die automatische Erkennung auf Inhaltsmustern basiert, werden HTML-Seiten entdeckt und verfolgt, die mit dem definierten URL-Muster in Zusammenhang stehen, wenn ein Web-Besucher eine Ansicht durchführt oder auf einen Link zur Seite klickt. Dieses Inhaltselement (URL, Seitenname und Metadaten einschließlich Bild-URL und Beschreibung) wird der Seite &quot;Alle Inhalte&quot;hinzugefügt, um prädiktiven Inhalt vorzubereiten. Für die automatische Erkennung anderer Inhalte wie PDFs und eingebettetes Video müssen Sie die Inhaltssuche [aktivieren](enable-content-discovery.md).

1. Gehen Sie zu **Inhaltseinstellungen**.

   ![](assets/settings-dropdown-hand-2.png)

1. Klicken Sie auf **URL-Muster**.

   ![](assets/click-url-patterns-hand.png)

1. Klicken Sie auf **+ **um eine Zeile zu öffnen, in der Sie Ihre Daten eingeben können.

   ![](assets/content-settings-create-patterns-hand.png)

1. hinzufügen die URL-Erweiterung der Domäne, in der die Webseite vorhanden ist. Wählen Sie die Kategorie aus (z. B. Blog, Artikel, Datenblatt, Pressemitteilung).

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >Elemente in der Dropdown-Liste auf der rechten Seite spiegeln die Kategorien wider, die Sie beim [Erstellen von Kategorien](set-up-categories.md)eingerichtet haben.

1. Klicken Sie auf **+ **um einen weiteren Pfad hinzuzufügen.

   ![](assets/url-patterns-add2.png)

1. hinzufügen Sie die Erweiterung und die Kategorie für den zusätzlichen Pfad und klicken Sie auf **Speichern**.

   ![](assets/url-patterns-save.png)

## Inhaltsmuster-Regeln {#content-pattern-rules}

* Sie können eine Platzhalterkarte an einer beliebigen Stelle in einem Ausdruck verwenden (Beispiel: *domain.com/**, *domain.com/*blog**)

* Es wird empfohlen, /* am Ende eines Ausdrucks zu verwenden, um die Mustererkennung fortzusetzen (Beispiel: *domain.com/blog/** erkennt alle Beiträge im Blog-Ordner)
* Bei Inhaltsmustern wird nicht zwischen Groß- und Kleinschreibung unterschieden (Beispiel: *domain.com/Blog/** entdeckt alle HTML-Seiten auf *domain.com/Blog* und *domain.com/blog*)

* URL-Parameter werden nicht erkannt (dies verhindert, dass mehrere Elemente mit derselben Inhalts-URL, aber unterschiedlichen Parametern erkannt werden)

## Beispiele {#examples}

Für *domain.com*:

<table> 
 <tbody> 
  <tr> 
   <th>URL-Muster</th> 
   <th>Ergebnis</th> 
  </tr> 
  <tr> 
   <td>blog/*</td> 
   <td><p>Entdeckt alle Inhalte, die dem Muster domain.com/blog/ entsprechen:</p><p>domain.com/blog/5-top-tricks</p><p>domain.com/blog/2017/new-year-solutions</p><p>domain.com/Blog/3-best-recipes</p></td> 
  </tr> 
  <tr> 
   <td>Artikel/2017/*</td> 
   <td><p>Entdeckt alle Inhalte, die dem Muster domain.com/article/2017/ entsprechen:</p><p>domain.com/article/2017/5-top-tricks</p></td> 
  </tr> 
  <tr> 
   <td><img alt="--" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="--"></td> 
   <td><p>Entdeckt alle URLs, die das Wort "Datasheets:"enthalten.</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>Pressemitteilung</td> 
   <td><p>Es wird nur eine exakte Übereinstimmung mit der HTML-Seite gefunden:</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>Wenn der URL-Ausdruck leer ist, erkennt das URL-Muster nur die Startseite:</p><p>domain.com</p></td> 
  </tr> 
 </tbody> 
</table>

