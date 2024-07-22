---
unique-page-id: 11385579
description: Erstellen von Inhaltsmustern - Marketo-Dokumente - Produktdokumentation
title: Inhaltsmutter erstellen
exl-id: 963529fb-1b30-486c-b97d-3ff697f91258
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 2%

---

# Inhaltsmutter erstellen {#create-content-patterns}

Wenn Sie Inhaltsmuster festlegen, werden Inhalte automatisch erkannt, wenn ein Webbesucher auf die für das Inhaltsmuster relevante HTML-Web-Seite klickt. Sie wird verwendet, um HTML-Seiten (Blog-Beiträge, Pressemitteilungen, News-Artikel) als Inhaltselemente zur Seite &quot;Alle Inhalte&quot;hinzuzufügen. Wenn die automatische Erkennung auf Inhaltsmustern basiert, erkennt und verfolgt sie HTML-Seiten, die mit dem definierten URL-Muster in Zusammenhang stehen, wenn ein Webbesucher einen Link zur Seite anzeigt oder darauf klickt. Dieses Inhaltselement (URL, Seitenname und Metadaten, einschließlich Bild-URL und Beschreibung) wird der Seite &quot;Alle Inhalte&quot;hinzugefügt, um prädiktive Inhalte vorzubereiten. Für die automatische Erkennung anderer Inhalte wie PDF und eingebettetes Video müssen Sie [die Inhaltserkennung aktivieren](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md).

1. Navigieren Sie zu **Inhaltseinstellungen**.

   ![](assets/settings-dropdown-hand-2.png)

1. Klicken Sie auf **URL-Muster**.

   ![](assets/click-url-patterns-hand.png)

1. Klicken Sie auf **+** , um eine Zeile zu öffnen, in der Sie Ihre Informationen eingeben können.

   ![](assets/content-settings-create-patterns-hand.png)

1. Fügen Sie die URL-Erweiterung der Domäne hinzu, in der die Webseite vorhanden ist. Wählen Sie die Kategorie aus (z. B. Blog, Artikel, Datenblatt, Pressemitteilung).

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >Elemente in der Dropdown-Liste auf der rechten Seite spiegeln die Kategorien wider, die Sie bei der [Erstellung der Kategorien](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md) eingerichtet haben.

1. Klicken Sie auf **+** , um einen weiteren Pfad hinzuzufügen.

   ![](assets/url-patterns-add2.png)

1. Fügen Sie die Erweiterung und Kategorie für den zusätzlichen Pfad hinzu und klicken Sie auf **Speichern**.

   ![](assets/url-patterns-save.png)

## Inhaltsmuster-Regeln {#content-pattern-rules}

* Sie können einen Platzhalter überall in einem Ausdruck verwenden (Beispiel: _domain.com/&#42;_, _domain.com/&#42;blog&#42;_)

* Es wird empfohlen, /&#42; am Ende eines Ausdrucks zu verwenden, um die Mustererkennung fortzusetzen (Beispiel: _domain.com/blog/&#42;_ findet alle Beiträge im Blog-Ordner).
* Bei Inhaltsmustern wird nicht zwischen Groß- und Kleinschreibung unterschieden (Beispiel: _domain.com/Blog/&#42;_ erkennt alle HTML-Seiten auf _domain.com/Blog_ und _domain.com/blog_)

* URL-Parameter werden nicht erkannt (dies verhindert, dass mehrere Elemente mit derselben Inhalts-URL, aber verschiedenen Parametern gefunden werden)

## Beispiele {#examples}

Für _domain.com_:

<table> 
 <tbody> 
  <tr> 
   <th>URL-Muster</th> 
   <th>Ergebnis</th> 
  </tr> 
  <tr> 
   <td>blog/*</td> 
   <td><p>Ermittelt alle Inhalte, die dem Muster domain.com/blog/ entsprechen:</p><p>domain.com/blog/5-top-tricks</p><p>domain.com/blog/2017/new-year-solutions</p><p>domain.com/Blog/3-best-recipes</p></td> 
  </tr> 
  <tr> 
   <td>Artikel 217/2017*</td> 
   <td><p>Ermittelt alle Inhalte, die dem Muster domain.com/article/2017/ entsprechen:</p><p>domain.com/article/2017/5-top-tricks</p></td> 
  </tr> 
  <tr> 
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="--"></td> 
   <td><p>Ermittelt alle URLs, die das Wort "datasheets:"enthalten.</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>Pressemitteilung</td> 
   <td><p>Es wird nur eine exakte HTML-Seite mit einer Übereinstimmung gefunden:</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>Wenn der URL-Ausdruck leer ist, erkennt das URL-Muster nur die Startseite:</p><p>domain.com</p></td> 
  </tr> 
 </tbody> 
</table>
