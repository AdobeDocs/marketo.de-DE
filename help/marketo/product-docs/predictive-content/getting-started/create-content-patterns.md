---
unique-page-id: 11385579
description: Erstellen von Inhaltsmustern - Marketo-Dokumente - Produktdokumentation
title: Inhaltsmutter erstellen
exl-id: 963529fb-1b30-486c-b97d-3ff697f91258
feature: Predictive Content
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 2%

---

# Inhaltsmutter erstellen {#create-content-patterns}

Wenn Sie Inhaltsmuster festlegen, wird der Inhalt automatisch erkannt, wenn ein Web-Besucher auf die für das Inhaltsmuster relevante HTML-Web-Seite klickt. Er wird verwendet, um HTML-Seiten (Blog-Beiträge, Pressemitteilungen, Nachrichtenartikel) als Inhaltselemente zur Seite „Alle Inhalte“ hinzuzufügen. Wenn die automatische Erkennung auf Inhaltsmustern basiert, werden HTML-Seiten, die mit dem definierten URL-Muster zusammenhängen, erkannt und verfolgt, wenn ein Web-Besucher eine Seite anzeigt oder auf einen Link klickt. Dieser Teil des Inhalts (URL, Seitenname und Metadaten, einschließlich Bild-URL und Beschreibung) wird der Seite „Alle Inhalte“ hinzugefügt, um prädiktive Inhalte vorzubereiten. Für die automatische Erkennung anderer Inhalte, z. B. PDFs und eingebettete Videos, müssen Sie [Inhaltssuche aktivieren](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md).

1. Navigieren Sie **[!UICONTROL Inhaltseinstellungen]**.

   ![](assets/settings-dropdown-hand-2.png)

1. Klicken Sie auf **[!UICONTROL URL-Muster]**.

   ![](assets/click-url-patterns-hand.png)

1. Klicken Sie auf das **+**, um eine Zeile zu öffnen, in der Sie Ihre Informationen eingeben können.

   ![](assets/content-settings-create-patterns-hand.png)

1. Fügen Sie die URL-Erweiterung der Domain hinzu, in der sich die Webseite befindet. Wählen Sie die Kategorie aus (z[!UICONTROL &#x200B; B. &#x200B;], [!UICONTROL Artikel], [!UICONTROL Datenblatt], [!UICONTROL Pressemitteilung]).

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >Die Elemente in der Dropdown-Liste auf der rechten Seite spiegeln die Kategorien wider, die Sie beim Erstellen [ Kategorien festgelegt ](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md).

1. Klicken Sie auf **+**, um einen weiteren Pfad hinzuzufügen.

   ![](assets/url-patterns-add2.png)

1. Fügen Sie die Erweiterung und die Kategorie für den zusätzlichen Pfad hinzu und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/url-patterns-save.png)

## Regeln für Inhaltsmuster {#content-pattern-rules}

* Sie können einen Platzhalter überall in einem Ausdruck verwenden (Beispiel: _domain.com/&#42;_, _domain.com/&#42;blog&#42;_)

* Es wird empfohlen, /&#42; am Ende eines Ausdrucks zu verwenden, um die Mustererkennung fortzusetzen (Beispiel: _domain.com/blog/&#42;_ erkennt alle Beiträge im Blog-Ordner)
* Bei Inhaltsmustern wird nicht zwischen Groß- und Kleinschreibung unterschieden (Beispiel: _domain.com/Blog/&#42;_ erkennt alle HTML-Seiten auf _domain.com/Blog_ und _domain.com/blog_)

* URL-Parameter werden nicht erkannt (dadurch werden mehrere Elemente mit derselben Inhalts-URL, aber unterschiedlichen Parametern vermieden)

## Beispiele {#examples}

Für _domain.com_:

<table> 
 <tbody> 
  <tr> 
   <th>URL-Muster</th> 
   <th>Ergebnis</th> 
  </tr> 
  <tr> 
   <td>Blog/*</td> 
   <td><p>Ermittelt alle Inhalte, die dem Muster domain.com/blog/ entsprechen:</p><p>domain.com/blog/5-top-tricks</p><p>domain.com/blog/2017/new-year-solutions</p><p>domain.com/Blog/3-best-recipes</p></td> 
  </tr> 
  <tr> 
   <td>Artikel/2017/*</td> 
   <td><p>Ermittelt alle Inhalte, die dem Muster domain.com/article/2017/ entsprechen:</p><p>domain.com/article/2017/5-top-tricks</p></td> 
  </tr> 
  <tr> 
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="--"></td> 
   <td><p>Ermittelt alle URLs, die das Wort „Datenblätter“ enthalten:</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>Pressemitteilung</td> 
   <td><p>Es wird nur eine exakte Übereinstimmung mit der HTML-Seite erkannt:</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>Wenn der URL-Ausdruck leer ist, erkennt das URL-Muster nur die Startseite:</p><p>domain.com</p></td> 
  </tr> 
 </tbody> 
</table>
