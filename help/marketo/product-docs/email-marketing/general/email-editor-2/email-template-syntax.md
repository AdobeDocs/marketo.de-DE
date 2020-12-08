---
unique-page-id: 11371040
description: Syntax der E-Mail-Vorlage - Marketing-Dokumente - Produktdokumentation
title: Syntax der E-Mail-Vorlage
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '2397'
ht-degree: 0%

---


# Syntax der E-Mail-Vorlage {#email-template-syntax}

In Marketos neuem E-Mail 2.0-Erlebnis bestehen E-Mail-Vorlagen aus einer beliebigen Kombination von Elementen, Variablen, Modulen oder Containern. Jede wird definiert, indem Sie Ihrem HTML eine Marketo-spezifische Syntax hinzufügen. Alte E-Mail-Vorlagen (v1.0) werden im E-Mail-Editor 2.0 unterstützt. Sie enthalten jedoch nicht alle Funktionen des neuen Editors.

Die Syntax von Marketo-E-Mails funktioniert nur in Vorlagen und einzelnen E-Mails. es funktioniert **nicht** , wenn es in Snippets oder Rich Text Tokens eingebettet ist.

>[!NOTE]
>
>Die Marketing-Unterstützung ist nicht so eingerichtet, dass sie bei CSS/HTML unterstützt wird. Wenn Sie mit CSS/HTML nicht vertraut sind, wenden Sie sich bitte an Ihren Entwickler.

>[!CAUTION]
>
>Bei Klassenwerten mit Marketo-Syntax (z. B. mktoModule, mktoContainer, mktoText) wird zwischen Groß- und Kleinschreibung unterschieden. Benutzerdefinierte Attributnamen (d. h. mktoimgwidth, mktoname) sind nicht vorhanden.

## Elemente {#elements}

Elemente sind Inhaltsbereiche, die Sie in Ihrer E-Mail-Vorlage als bearbeitbar definieren. Die Bearbeitung eines Elements ist für seinen Typ und seine Angebot einzigartig und stellt eine einfache Möglichkeit dar, mit Inhalten zu arbeiten. Folgende Elemente können in eine E-Mail-Vorlage einbezogen werden:

* Rich Text
* Bilder
* Snippets
* Videos

## Rich Text {#rich-text}

Wenn Sie eine Region als Rich Text definieren, können Benutzer ihre Inhalte [mit dem Rich Text Editor](../../../../product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)von Marketo bearbeiten. Es gibt zwei Möglichkeiten, ein Rich-Text-Element in einer E-Mail-Vorlage zu definieren: mktEditable und mktoText. Beachten Sie, dass ein Rich-Text-Element immer aus dem E-Mail-Editor in ein Snippet konvertiert werden kann.

### Option 1 - mktEditable {#option-mkteditable}

Da der E-Mail-Editor 2.0 abwärtskompatibel ist, können einige alte E-Mail-Vorlagen Rich-Text-Elemente angeben, indem class=&quot;mktEditable&quot; für jedes HTML-Element hinzugefügt wird. Dies wird weiterhin unterstützt, und die ID des Elements wird als Anzeigename im E-Mail-Editor verwendet.

Erforderliche Attribute

* **class**: &quot;mktEditable&quot;.
* **id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.

Optionale Attribute

* **mktoName** : Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Standardwert

Der Inhalt im HTML-Element (sofern vorhanden) mit class=&quot;mktEditable&quot; wird als Standardwert für das Rich Text-Element verwendet.

Beispiel:

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### Option 2 - mktoText {#option-mktotext}

Es wird empfohlen, Rich Text-Elemente mit der Syntax class=&quot;mktoText&quot; anzugeben. Dadurch wird sichergestellt, dass immer ein passender Anzeigename für das Element vorhanden ist.

Erforderliche Attribute

* **class**: &quot;mktoText&quot;
* **id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName** : Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Standardwert

Der Inhalt im HTML-Element (sofern vorhanden) mit class=&quot;mktoText&quot; wird als Standardwert für das Rich Text-Element verwendet.

Beispiel:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## Bilder {#images}

Sie haben zwei Optionen zum Definieren bearbeitbarer Bildelemente. Sie können entweder eine `<div>`, die einen Container angibt, in den die Datei eingefügt `<img>` wird, oder ein `<img>` -Tag verwenden. Wenn Sie möchten, dass der Endbenutzer einfach ein Bild auswählt, das die Bild-URL zurückgibt (im Gegensatz zum DOM), lesen Sie bitte &quot;Bildvariablen&quot; im folgenden Abschnitt. Die folgenden beiden Optionen fügen ein HTML- `<img>` Element ein.

### Option 1: Verwenden eines \&lt;div\> {#option-use-a-div}

Erforderliche Attribute

* **class:** &quot;mktoImg&quot;.
* **id:** ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **mktoImgClass:** Zeichenfolge. Der Wert hier wird dem Klassenattribut des `<img>` Elements innerhalb des div hinzugefügt.
* **mktoImgSrc:** Wird als Standardwert für das Bild verwendet, das in diesem div platziert wird. Ein Platzhalter wird verwendet, wenn dies weggelassen wird.
* **mktoImgLink:** Geben Sie an, dass die URL von einem `<img>` `<a>` Tag mit dieser Ziel-URL umgeben sein soll. Der Benutzer kann dies im E-Mail-Editor ändern.
* **mktoImgLinkTarget:** Geben Sie an, dass das `<a>` Tag des Attributs mktoImgLink diese Zielgruppe verwenden soll. Hat keine Auswirkung, wenn mktoImgLink nicht auch verwendet wird.
* **mktoImgWidth:** Wird als Breite auf der eingeschlossenen Seite verwendet `<img>`.
* **mktoImgHeight:** Wird als Höhe auf der eingeschlossenen Seite verwendet `<img>`.
* **mktoLockImgSize:** Wird verwendet, um die Eigenschaft height und width des `<img>` Elements zu entsperren, sodass der Endbenutzer Änderungen vornehmen kann (Standard ist true, wenn keine Angabe gemacht wird).
* **mktoLockImgStyle:** Wird zum Sperren der Stileigenschaft des `<img>` Elements verwendet (Standard ist false).

Standardwert (optional)

**`<img>`**: Wird als `<img>` Element verwendet, in dem das Bild platziert wird. Nützlich, wenn Sie dem Bild einen Inline-Stil hinzufügen möchten. Denken Sie daran, umliegende `<a> </a>` Tags einzuschließen. Wenn der Benutzer also einen Link hinzufügt, wird Ihr Stil nicht entfernt!

Beispiel:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="http://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### Option 2: Verwenden eines \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>Diese Option erlaubt es Endbenutzern nicht, einen Link zu ihrem Bild hinzuzufügen. Verwenden Sie Option 1, wenn dies für Ihre Vorlage wichtig ist.

Erforderliche Attribute

* **class:** &quot;mktoImg&quot;.
* **id:** ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.  Standardwert (optional)
* **src:** Wird als Standardwert für das Bild verwendet. Ein Platzhalter wird verwendet, wenn dies weggelassen wird.
* **mktoLockImgSize:** Wird verwendet, um die Eigenschaft height und width des `<img>` Elements zu entsperren, sodass der Endbenutzer Änderungen vornehmen kann (Standard ist true, wenn keine Angabe gemacht wird).
* **mktoLockImgStyle:** Wird zum Sperren der Stileigenschaft des `<img>` Elements verwendet (Standard ist false).

Beispiel:
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## Snippets {#snippets}

Wenn Sie einen Bereich als Snippet definieren, können Endbenutzer wählen, welches [](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)Snippet sie in diesen Bereich einfügen möchten. Rich-Text-Elemente können zwar aus dem E-Mail-Editor in Snippets konvertiert werden, aber wenn Sie eine Region spezifisch als Snippet definieren, kann sie nicht in Rich-Text konvertiert werden. Sie können einen Snippet-Bereich mit einer `<div>` mit class=&quot;mktoSnippet&quot; angeben.

Erforderliche Attribute

* **id:** ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Standardwert (optional)

**mktoDefaultSnippetId**: Die numerische ID des Marketo-Snippets, die standardmäßig angezeigt werden sollte (funktioniert nur, wenn ein Snippet mit dieser ID vorhanden ist und in diesem Arbeitsbereich genehmigt wird).

Beispiel:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## Video {#video}

Wenn Sie einen Bereich als Video definieren, können Endbenutzer entweder eine YouTube- oder eine Vimeo-URL einfügen, die als Miniaturbild (mit der Schaltfläche &quot;Abspielen&quot;) in der E-Mail angezeigt wird. Sie können einen Videobereich mit einer `<div>` mit class=&quot;mktoVideo&quot; angeben.

Erforderliche Attribute

* **id:** ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **mktoImgClass:** Zeichenfolge. Der Wert hier wird dem Klassenattribut der Videominiatur `<img>` innerhalb des div hinzugefügt.

Beispiel:

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## Variablen {#variables}

Variablen sind wie Token. Zuerst definieren Sie sie im Abschnitt Ihrer E-Mail-Vorlage mit `<head>` `<meta>` -Tags und verwenden Sie sie dann so oft, wie Sie es in der Vorlage wünschen. Da sie in der Vorlage definiert sind, kann der Endbenutzer seine Werte entsprechend den Regeln ändern. Beachten Sie, dass Sie eine Variable als lokal oder global im Gültigkeitsbereich definieren können. Wenn Sie eine Variable innerhalb eines Moduls (siehe unten) und ein Duplikat eines Endbenutzers verwenden, das diese Module enthält, verfügen die lokalen Variablen über unabhängige Werte, während die globalen Variablen für beide Module gelten.

## Zeichenfolge {#string}

Wenn Sie eine Variable als Zeichenfolge angeben, kann der Endbenutzer Text in einem Textfeld im E-Mail-Editor eingeben. Sie geben eine String-Variable `<meta>` mit class=&quot;mktoString&quot; an

Erforderliche Attribute

* **id:** Referenzieren der Variablen in Ihrer E-Mail-Vorlage.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **allowHTML:** Boolescher Wert. Steuert, ob der Variablenwert mit HTML-Escape-Zeichen versehen ist. Der Standardwert ist &quot;false&quot;, wenn kein Wert angegeben wird.
* **Standard**: Standardwert für die Zeichenfolge. Leer, wenn nicht angegeben.
* **mktoModuleScope**: Boolescher Wert. Steuert, ob die Variable lokal (true) oder global (false) ist, wenn sie in einem Modul verwendet wird. Der Standardwert ist &quot;false&quot;, wenn kein Wert angegeben wird.

Beispieldeklaration:

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

Beispielverwendung:

`<pre data-theme="Confluence">${textHeader}</pre>`

## Liste {#list}

Wenn Sie eine Variable als Liste angeben, kann der Endbenutzer aus einem Satz von Werten wählen, die Sie im E-Mail-Editor definieren. Sie geben eine Variable für die Liste `<meta>` mit class=&quot;mktoList&quot; an

Erforderliche Attribute

* **id**: Referenzieren der Variablen in Ihrer E-Mail-Vorlage.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.
* **Werte:** Kommagetrennte Liste von Werten. Muss mindestens eine Zeichenfolge enthalten.

Optionale Attribute

* **default:** Standardwert des Dropdownmenüs &quot;Auswählen&quot;. Wenn dieser Wert weggelassen wird, wird der erste Wert des Attributs &quot;Werte&quot;verwendet.
* **mktoModuleScope**: Boolescher Wert. Steuert, ob die Variable lokal (true) oder global (false) ist, wenn sie in einem Modul verwendet wird. Der Standardwert ist &quot;false&quot;, wenn kein Wert angegeben wird.

Beispieldeklaration:

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

Beispielverwendung:

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## Nummer {#number}

Wenn Sie eine Variable als Zahl angeben, kann der Endbenutzer eine Zahl im E-Mail-Editor eingeben. Sie geben eine Number-Variable `<meta>` mit class=&quot;mktoNumber&quot; ein.

Erforderliche Attribute

* **id**: Referenzieren der Variablen in Ihrer E-Mail-Vorlage.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.
* **default:** Standardwert für die Variable.

Optionale Attribute

* **min:** Min. akzeptierter Wert.
* **max:** Max. zulässiger Wert.
* **Einheiten:** Am Zahlenwert anzuhängende Einheiten (z. B.: px, pt, em usw.) angezeigt, sowohl im E-Mail-Editor als auch im resultierenden Code.
* **step:** Wie viele Einheiten sollte die Zahlenvariable um (0.1, 1, 10 usw.) erhöhen/verringern? Wenn dieser Wert weggelassen wird, wird der Standardwert 1 verwendet.
* **mktoModuleScope**: Boolescher Wert. Steuert, ob die Variable lokal (true) oder global (false) ist, wenn sie in einem Modul verwendet wird. Der Standardwert ist &quot;false&quot;, wenn kein Wert angegeben wird.

Beispieldeklaration:

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

Beispielverwendung:

`<pre data-theme="Confluence">${textFontSize}</pre>`

## Farbe {#color}

Wenn Sie eine Variable als Farbe angeben, kann der Endbenutzer einen hexadezimalen Farbwert eingeben oder eine Farbe aus der Farbauswahl im E-Mail-Editor auswählen. Sie geben eine Color-Variable `<meta>` mit class=&quot;mktoColor&quot; an

Erforderliche Attribute

* **id**: Referenzieren der Variablen in Ihrer E-Mail-Vorlage.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **default:** Standardwert für die Farbe. 6-stelliger hexadezimaler Farbcode. Ex: #ffffff.
* **mktoModuleScope**: Boolescher Wert. Steuert, ob die Variable lokal (true) oder global (false) ist, wenn sie in einem Modul verwendet wird. Der Standardwert ist &quot;false&quot;, wenn kein Wert angegeben wird.

Beispieldeklaration:

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

Beispielverwendung:

`<pre data-theme="Confluence">${textColor}</pre>`

## Boolesch {#boolean}

Wenn Sie eine Variable als boolesche Variable angeben, kann der Endbenutzer die Option im E-Mail-Editor aktivieren/deaktivieren. Sie geben eine boolesche Variable `<meta>` mit class=&quot;mktoBoolean&quot; an

Erforderliche Attribute

* **id**: Referenzieren der Variablen in Ihrer E-Mail-Vorlage.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **default:** Boolescher Wert, der den Standardstatus des Umschalters bestimmt. False, wenn nicht angegeben.
* **false_value:** Der einzufügende Wert, wenn sich der Umschalter in AUS-Position befindet. False, wenn nicht angegeben.
* **true_value:** Der Wert, der eingefügt werden soll, wenn sich der Umschalter in ON-Position befindet. True, wenn ausgelassen.
* **false_value_name:** Die Benutzeroberfläche wird im Umschalter angezeigt, wenn sie sich in AUS-Position befindet. False, wenn nicht angegeben.
* **true_value_name:** Die Benutzeroberfläche wird im Umschalter angezeigt, wenn sie sich an der Position ON befindet. True, wenn ausgelassen.
* **mktoModuleScope**: Boolescher Wert. Steuert, ob die Variable lokal (true) oder global (false) ist, wenn sie in einem Modul verwendet wird. Der Standardwert ist &quot;false&quot;, wenn kein Wert angegeben wird.

Beispieldeklaration:

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

Beispielverwendung:

`<pre data-theme="Confluence">${showFooter}</pre>`

## HTML-Block {#html-block}

Wenn Sie eine Variable als HTML-Block angeben, kann der Endbenutzer wörtliche HTML aus dem E-Mail-Editor eingeben. Sie geben eine HTML-Block-Variable `<meta>` mit class=&quot;mktoHTML&quot; an

Erforderliche Attribute

* **id**: Referenzieren der Variablen in Ihrer E-Mail-Vorlage.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **default:** HTML-kodierter Wert, der als Standardinhalt des Blocks dient.
* **mktoModuleScope**: Boolescher Wert. Steuert, ob die Variable lokal (true) oder global (false) ist, wenn sie in einem Modul verwendet wird. Der Standardwert ist &quot;false&quot;, wenn kein Wert angegeben wird.

Beispieldeklaration:

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

Beispielverwendung:

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## Bildvariable {#image-variable}

Wenn Sie eine Variable als Bild angeben, kann der Endbenutzer ein Bild aus der Bildauswahl im E-Mail-Editor auswählen. Die ausgewählte Bild-URL ist der Wert der Variablen. Sie geben eine Image-Variable `<meta>` mit class=&quot;mktoImg&quot; an

Erforderliche Attribute

* **id**: Referenzieren der Variablen in Ihrer E-Mail-Vorlage.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **default:** Standardbild-URL für das Element.
* **mktoModuleScope**: Boolescher Wert. Steuert, ob die Variable lokal (true) oder global (false) ist, wenn sie in einem Modul verwendet wird. Der Standardwert ist &quot;false&quot;, wenn kein Wert angegeben wird.

Beispieldeklaration:

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="http://www.company.com/image.jpg"></pre>`

Beispielverwendung:

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## Module {#modules}

Module sind vorlagenbasierte Abschnitte, die auf Vorlagenebene definiert werden und die Endbenutzer zum Einfügen in ihre E-Mail-Nachricht aufrufen können. Da Sie diese Module bereits erstellt haben, können Sie sicherstellen, dass sie mit dem Rest Ihres E-Mail-Inhalts korrekt interagieren (in einer vollständig reaktionsfähigen Weise). Man kann nur ein Modul in einen Container setzen.

**Für Container des Typs `<table>`, `<tbody>`, `<thead>``<tfoot>`oder:**

Spezifiziert mit `<tr>` class=&quot;mktoModule&quot;

**Bei Containern des Typs `<td>`:**

Spezifiziert mit `<table>` class=&quot;mktoModule&quot;

Erforderliche Attribute

* **id**: Wie Sie auf das Modul in Ihrer E-Mail-Vorlage verweisen.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **mktoActive:** Bestimmt, ob dieses Modul in der Liste der Module im E-Mail-Editor angezeigt wird. Der Standardwert ist true. Wenn &quot;false&quot;, kann das Modul nicht von einem Endbenutzer einer E-Mail hinzugefügt werden.
* **mktoAddByDefault:** Stellt fest, ob sich dieses Modul bei der Erstellung in der Arbeitsfläche einer neuen E-Mail befindet, die diese Vorlage verwendet. Die Standardeinstellung ist true (wenn mktoActive auf false gesetzt ist, wird dieser Wert ignoriert).

>[!NOTE]
>
>**Erinnerung**
>
>Bei Klassenwerten mit Marketo-Syntax (z. B. mktoModule, mktoContainer, mktoText) wird zwischen Groß- und Kleinschreibung unterschieden. Benutzerdefinierte Attributnamen (d. h. mktoimgwidth, mktoname) sind nicht vorhanden.

## Container {#containers}

Ein Container enthält Module und definiert, wo sie platziert werden können. Wenn Endbenutzer Module neu anordnen und in ihre E-Mail einfügen, steuert der Container, wohin sie gehen können.

**Angabe mit `<table>`, `<tbody>`, `<thead>`, `<tfoot>` oder `<td>` mit class=&quot;mktoContainer&quot;**

Erforderliche Attribute

**id**: Wie Sie auf das Modul in Ihrer E-Mail-Vorlage verweisen.

>[!CAUTION]
>
>Container können nur Module enthalten - wenn noch etwas Anderes vorhanden ist, wird der Container als ungültig angesehen! Pro Vorlage ist nur ein Container zulässig.
