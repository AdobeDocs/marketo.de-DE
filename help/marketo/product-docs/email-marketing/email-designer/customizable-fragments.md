---
solution: Marketo Engage
product: marketo
title: Anpassbare Fragmente
description: Erfahren Sie, wie Sie Fragmente anpassen können, indem Sie einige Felder bearbeitbar machen. Erstellen Sie flexible wiederverwendbare Fragmente in der E-Mail-Designer.
level: Beginner, Intermediate
feature: Email Designer
role: User
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
TQID: https://experienceleague.adobe.com/SCmyn9QUECmvQgVltKknlvLuvL15Tz3LYorBFYB1hqI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 8ba2ac1fa056e96aac50abbde16042e522779ab3
workflow-type: tm+mt
source-wordcount: 1410
ht-degree: 12%

---

# Anpassbare Fragmente {#customizable-fragments}

Wenn Fragmente in einer E-Mail oder E-Mail-Vorlage verwendet werden, sind sie aufgrund der Vererbung standardmäßig gesperrt, d. h. alle Änderungen, die an einem Fragment vorgenommen werden, werden automatisch an alle Assets weitergegeben, in denen es verwendet wird. Mit anpassbaren Fragmenten können bestimmte Felder innerhalb eines Fragments als bearbeitbar definiert werden, wenn das Fragment zu einer E-Mail oder E-Mail-Vorlage hinzugefügt wird. Wenn Sie beispielsweise über ein Fragment mit einem Banner, etwas Text und einer Schaltfläche verfügen, können Sie bestimmte Felder, z. B. die Bild- oder Schaltflächen-Ziel-URL, als bearbeitbar festlegen.

Mit anpassbaren Fragmenten können Sie Inhalte verwalten und personalisieren, ohne völlig neue Inhaltsbausteine zu erstellen oder die Fragmentvererbung zu unterbrechen. Änderungen, die auf Fragmentebene vorgenommen werden, werden weiterhin weitergegeben und ermöglichen die Anpassung auf E-Mail- oder E-Mail-Vorlagenebene.

Sowohl visuelle Fragmente als auch Ausdrucksfragmente können als anpassbar markiert werden.

## Hinzufügen bearbeitbarer Felder in visuellen Fragmenten {#visual}

Gehen Sie wie folgt vor, um Teile eines visuellen Fragments als bearbeitbar festzulegen:

>[!NOTE]
>
>Bearbeitbare Felder können zu **Bild**-, **Text**- und **Schaltflächenkomponenten** hinzugefügt werden. Für **HTML**-Komponenten werden bearbeitbare Felder ähnlich wie Ausdrucksfragmente mithilfe des Personalisierungseditors hinzugefügt. [Erfahren Sie, wie Sie bearbeitbare Felder in HTML-Komponenten und Ausdrucksfragmenten hinzufügen](#expression)

1. Öffnen Sie den Bildschirm zur Inhaltsbearbeitung von Fragmenten.

1. Wählen Sie die Komponente in Ihrem Fragment aus, für die Sie bearbeitbare Felder konfigurieren möchten.

1. Der Bereich der Komponenteneigenschaften wird auf der rechten Seite geöffnet. Wählen Sie die Registerkarte **[!UICONTROL Bearbeitbare Felder]** aus und aktivieren Sie die Option **[!UICONTROL Bearbeitung aktivieren]**.

1. Alle Felder, die für die ausgewählte Komponente bearbeitet werden können, werden im Bereich aufgelistet. Welche Felder zur Bearbeitung verfügbar sind, hängt vom ausgewählten Komponententyp ab.

   Im folgenden Beispiel ist die URL der Schaltfläche „Hier klicken“ als bearbeitbar konfiguriert.

   ![](assets/fragment-param-enable.png){width="800" zoomable="yes"}

1. Klicken Sie **[!UICONTROL Übersicht]**, um alle bearbeitbaren Felder und ihre Standardwerte zu überprüfen.

   In diesem Beispiel wird das Feld für die Schaltflächen-URL mit dem in der Komponente definierten Standardwert angezeigt. Benutzende können diesen Wert anpassen, nachdem sie das Fragment zu ihrem Inhalt hinzugefügt haben.

   ![](assets/fragment-param-preview.png){width="800" zoomable="yes"}

1. Speichern Sie abschließend Ihre Änderungen.

Nachdem Sie das Fragment zu einer E-Mail hinzugefügt haben, können Benutzer alle bearbeitbaren Felder anpassen, die im Fragment konfiguriert sind.

## Hinzufügen bearbeitbarer Felder zu HTML-Komponenten und Ausdrucksfragmenten {#expression}

Innerhalb einer HTML-Komponente können die folgenden Elementtypen bearbeitbar gemacht werden:

* Ein Teil des **Textinhalts** (z. B. eine Überschrift oder eine CTA-Kennzeichnung).
* Eine vollständige **URL**, die als Link-Ziel oder Bildquelle verwendet wird. Partielle URLs werden nicht unterstützt. Die Variable muss den gesamten URL-Wert darstellen.
* Ein vollständiger **CSS-Eigenschaftswert** (z. B. ein voller Farbwert, ein voller Abstand oder ein voller Breitenwert). Partielle CSS-Eigenschaftswerte werden nicht unterstützt.

Jeder parametrisierte CSS-Eigenschaftswert muss genau `{{{varName}}}` sein: keine Suffixe, kein zusätzlicher Text, keine mehreren Variablen und keine Verkettung innerhalb einer einzelnen Eigenschaft.

Um mehrseitige Eigenschaften wie den Abstand zu parametrisieren, gehen Sie wie folgt vor:

* jede Seite als separate Eigenschaft deklarieren _(empfohlen)_ oder
* Deklarieren Sie eine einzelne Variable, die den vollständigen Kurzschreibwert enthält.

## Funktionsweise von bearbeitbaren Feldern in HTML-Komponenten {#components}

Bearbeitbare Felder in einer HTML-Komponente werden erstellt, indem Inline-Variablen direkt im Quellcode der Komponente deklariert werden. Jede Variable hat eine eindeutige ID und einen Standardwert. Die Variable wird dann dort referenziert, wo der bearbeitbare Wert im Markup angezeigt werden soll.

Nach dem Speichern und Veröffentlichen des Fragments wird jede in der HTML-Komponente deklarierte Variable automatisch als bearbeitbarer Parameter angezeigt, wenn das Fragment zu einer E-Mail hinzugefügt wird.

Der E-Mail-Autor kann dann den Standardwert einer beliebigen Variablen aus der E-Mail-Designer überschreiben (z. B. eine Hintergrundfarbe ändern, eine CTA-URL austauschen oder eine Überschrift aktualisieren), ohne die zugrunde liegende HTML zu ändern.

## Syntaxverweis {#syntax}

Bearbeitbare Felder werden anhand von zwei Mustern definiert und referenziert:

### Deklarieren einer Variablen {#declaring}

Verwenden Sie die Inline-Deklaration, um eine Variable mit einer eindeutigen ID und einem Standardwert zu definieren:

```handlebars
{{#inline "variableID"}}default_value{{/inline}}
```

Ersetzen Sie `variableID` durch eine eindeutige Kennung für das bearbeitbare Feld. Die ID muss innerhalb der Komponente eindeutig sein und darf keine Leerzeichen enthalten.

Ersetzen Sie `default_value` durch den Wert, der verwendet werden soll, wenn der E-Mail-Autor ihn nicht überschreibt.

### Verweisen auf eine Variable {#referencing}

Verwenden Sie dreifache geschweifte Klammern, um auf die Variable an der Stelle zu verweisen, an der ihr Wert im Markup angezeigt werden soll:

```handlebars
{{{variableID}}}
```

Dieselbe Variablenkennung kann innerhalb der HTML beliebig oft referenziert werden. Alle Verweise werden auf den Wert aufgelöst, den der E-Mail-Autor festlegt (oder auf den Standardwert, wenn keine Überschreibung bereitgestellt wird).

### Optionale Parameter {#optional}

Die Inline-Deklaration unterstützt optionale Parameter, die die Darstellung oder Verarbeitung des bearbeitbaren Felds ändern:

| Aktion | Parameter | Beispiel |
|---|---|---|
| Deklarieren eines bearbeitbaren Felds mit einem **Standardwert**. Wenn das Fragment zu einer E-Mail hinzugefügt wird, wird dieser Standardwert verwendet, es sei denn, der Autor überschreibt ihn. | Hinzufügen des Standardwerts zwischen den Inline-Tags. | `{{#inline "editableFieldID"}}default_value{{/inline}}` |
| Definieren eines **Labels** für das bearbeitbare Feld. Dieser Titel wird in der E-Mail-Designer angezeigt, wenn der E-Mail-Autor die Felder des Fragments bearbeitet. | `name="title"` | `{{#inline "editableFieldID" name="title"}}default_value{{/inline}}` |
| Deklarieren Sie ein bearbeitbares Feld, das eine **Bildquelle“**. | `assetType="image"` | `{{#inline "editableFieldID" assetType="image"}}default_value{{/inline}}` |
| Deklarieren Sie ein bearbeitbares Feld, das eine **URL** enthält, die verfolgt werden muss. | `assetType="url"` | `{{#inline "editableFieldID" assetType="url"}}default_value{{/inline}}` |

## Hinzufügen bearbeitbarer Felder zu einer HTML-Komponente {#adding-editable-fields}

Gehen Sie wie folgt vor, um Teile einer HTML-Komponente in einem visuellen Fragment bearbeitbar zu machen:

1. Öffnen Sie das visuelle Fragment zur Bearbeitung in der E-Mail-Designer.
1. Fügen Sie eine **HTML-** zum Fragment im Bedienfeld „Komponenten“ hinzu oder wählen Sie eine bestehende HTML-Komponente aus.
1. Klicken Sie bei ausgewählter HTML-Komponente **Quellcode anzeigen**, um die HTML-Quellansicht im Personalisierungseditor zu öffnen.
1. Deklarieren Sie im Personalisierungseditor jede bearbeitbare Variable mithilfe der Inline-Deklarationssyntax. Platzieren Sie alle Variablendeklarationen zur besseren Lesbarkeit am Anfang der Komponente und weisen Sie jeder Variablen eine eindeutige ID zu.
1. Referenzieren Sie jede Variable im HTML-Markup mithilfe der `{{{variableID}}}`, wo immer der bearbeitbare Wert angezeigt werden soll. Dieselbe Variable kann mehrmals in derselben Komponente referenziert werden.
1. Speichern Sie die HTML-Komponente und speichern Sie dann das Fragment.
1. Veröffentlichen Sie das Fragment, um es für die Verwendung in E-Mails verfügbar zu machen.

## Fragment in einer E-Mail verwenden {#using-fragment}

Nachdem das Fragment veröffentlicht wurde, werden alle in den HTML-Komponenten deklarierten Variablen als bearbeitbare Parameter in der E-Mail-Designer angezeigt.

So passen Sie sie bei Verwendung des Fragments in einer E-Mail an:

1. Öffnen oder erstellen Sie eine E-Mail in der Marketo Engage Email Designer.
1. Fügen Sie das veröffentlichte Fragment zur E-Mail-Arbeitsfläche hinzu.
1. Wählen Sie das Fragment aus, um seinen Eigenschaftenbereich zu öffnen. Die Liste der bearbeitbaren Felder wird im Abschnitt **Bearbeitbare Felder** angezeigt, wobei jedes Feld durch seine Variable ID (oder durch die im Parameter `name` angegebene benutzerfreundliche Beschriftung) gekennzeichnet ist.
1. Aktualisieren Sie den Wert eines beliebigen bearbeitbaren Felds direkt im Bereich Eigenschaften . Die Änderung gilt nur für die aktuelle E-Mail. Das veröffentlichte Fragment und andere E-Mails, die darauf verweisen, sind davon nicht betroffen.
1. Speichern Sie die E-Mail.

Das Fragment wird mit den angepassten Werten gerendert, während weiterhin alle zukünftigen strukturellen Aktualisierungen am veröffentlichten Fragment übernommen werden.

### Beispiel: einfaches Fragment mit bearbeitbarem Text, Farbe und URL {#example}

Im folgenden Beispiel wird ein kleines Werbebanner mit vier bearbeitbaren Feldern erstellt:

* Eine Hintergrundfarbe
* Ein Überschrifttext
* Ein CTA-Label
* eine CTA-URL

Nach der Veröffentlichung des Fragments kann ein E-Mail-Autor diese Werte überschreiben, wenn er das Fragment zu einer E-Mail hinzufügt.

**Einfaches bearbeitbares Banner**

```html
<!-- Define editable variables -->
{{#inline "bgColor"}}#0057FF{{/inline}}
{{#inline "headlineText"}}Example Headline{{/inline}}
{{#inline "ctaText"}}Learn More{{/inline}}
{{#inline "ctaUrl" assetType="url"}}https://www.example.com{{/inline}}

<!-- Use the variables in the HTML -->
<table width="100%" cellpadding="0" cellspacing="0"
       style="background-color:{{{bgColor}}}; border-radius:8px;" >
  <tr>
    <td style="padding:30px; text-align:center; font-family:Arial,sans-serif;">
      <h2 style="color:#ffffff; font-size:24px; margin:0;">
        {{{headlineText}}}
      </h2>
      <a href="{{{ctaUrl}}}"
         style="display:inline-block; margin-top:16px; padding:12px 28px;
                background:#ffffff; color:{{{bgColor}}};
                font-weight:bold; border-radius:4px; text-decoration:none;">
        {{{ctaText}}}
      </a>
    </td>
  </tr>
</table>
```

In diesem Beispiel:

* `bgColor` wird zweimal referenziert: einmal für die Hintergrundfarbe der Tabelle und einmal für die Textfarbe von CTA. Beide Verweise werden auf denselben Wert aufgelöst, sodass eine einzelne Bearbeitung an beide Speicherorte übertragen wird.
* `ctaUrl` wird mit `assetType="url"` deklariert, was signalisiert, dass der Wert als getrackte URL verarbeitet werden soll.

## Best Practices {#best-practices}

* Schließen Sie Einheiten (`px`, `em`, `%`) in den Standardwert der Variablen ein, sodass die Variable einen vollständigen CSS-Wert darstellt. Dadurch wird eine Verkettung vermieden, die nicht unterstützt wird.
* CSS-Eigenschaften pro Seite (`padding-top`, `padding-right`, `padding-bottom`, `padding-left`) werden den Kurzbezeichnungen vorgezogen, wenn jede Seite unabhängig bearbeitet werden muss.
* Wenn eine URL getrackt werden muss, deklarieren Sie sie mit `assetType="url"`.
* Wenn ein bearbeitbares Feld eine Bildquelle enthält, deklarieren Sie es mit `assetType="image"`.
* Testen Sie das Fragment, indem Sie es zu einem E-Mail-Entwurf hinzufügen und überprüfen, ob alle bearbeitbaren Felder im Eigenschaftenbereich angezeigt werden und beim Überschreiben korrekt aufgelöst werden.

## Was Sie wissen sollten {#things-to-know}

* Bearbeitbare Felder in HTML-Komponenten unterstützen Volltextinhalte, vollständige URLs und vollständige CSS-Eigenschaftswerte. Partielle URLs und partielle CSS-Eigenschaftswerte können nicht parametrisiert werden.
* Ein einzelner CSS-Eigenschaftswert kann eine Variable nicht mit zusätzlichem statischem Text oder mit einer anderen Variablen kombinieren. Jeder parametrisierte Eigenschaftswert muss genau ein Variablenverweis sein.
* Variablen-IDs müssen innerhalb einer HTML-Komponente eindeutig sein und dürfen keine Leerzeichen enthalten.
* Vorkonfigurierte Systemlinks wie der Abmelde-Link und die Mirrorseiten-URL können nicht in bearbeitbare Felder umgewandelt werden.

<!--
## Add editable fields in HTML components and expression fragments {#expression}

To make portions of an HTML component or an expression fragment editable, you must use a specific syntax in the expression editor. This involves declaring a _variable_ with a default value that users can override after adding the fragment to their content.

For example, suppose you want to create a fragment to add to your emails, and allow users to customize a specific color used in different locations, such as frames or buttons' background colors. When creating your fragment, you need to declare a variable with a _unique ID_ (e.g., "color"), and call it at the desired locations in the fragment content where you want to apply this color. When adding the fragment to their content, users will be able to customize the color used wherever the variable is referenced.

For HTML components, only specific elements can become editable fields. Expand the section below for more information.

+++Editable elements in HTML components:

The elements below can become editable fields in an HTML component:

* A portion of text
* A full URL for link or image (doesn't work with portion of a URL)
* Entire CSS property (doesn't work with partial property)

For example, in the code below, each element highlighted in red can become a property:

![](assets/fragment-html.png){width="500" zoomable="yes"}

+++
-->

>[!MORELIKETHIS]
>
>[Fragmente](/help/marketo/product-docs/email-marketing/email-designer/fragments.md){target="_blank"}
