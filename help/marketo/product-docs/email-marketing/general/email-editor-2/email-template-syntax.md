---
unique-page-id: 11371040
description: Syntax der E-Mail-Vorlage - Marketo-Dokumente - Produktdokumentation
title: Syntax der E-Mail-Vorlage
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: a9f880bd32d533613020d0472c0e1bee07ab388c
workflow-type: tm+mt
source-wordcount: '2449'
ht-degree: 1%

---

# Syntax der E-Mail-Vorlage {#email-template-syntax}

In Marketos neuem E-Mail 2.0-Erlebnis bestehen E-Mail-Vorlagen aus einer beliebigen Kombination von Elementen, Variablen, Modulen oder Containern. Jede wird definiert, indem Sie Ihrer HTML eine Marketo-spezifische Syntax hinzufügen. Alte (v1.0) E-Mail-Vorlagen werden in E-Mail-Editor 2.0 unterstützt. Sie enthalten jedoch nicht alle neuen Editor-Funktionen.

Die E-Mail-Syntax von Marketo funktioniert nur in Vorlagen und E-Mails. Sie funktioniert **nicht**, wenn sie in Snippets oder Rich-Text-Token eingebettet ist.

>[!NOTE]
>
>Der Marketo-Support ist nicht für CSS/HTML eingerichtet. Wenn Sie nicht mit CSS/HTML vertraut sind, wenden Sie sich an Ihren Entwickler.

>[!CAUTION]
>
>Bei Klassenwerten mit Marketo-Syntax (d. h. mktoModule, mktoContainer, mktoText) wird zwischen Groß- und Kleinschreibung unterschieden. Benutzerdefinierte Attributnamen (d. h. mktoimgwidth, mktoname) sind nicht vorhanden.

## Elementen {#elements}

Elemente sind Inhaltsbereiche, die Sie in Ihrer E-Mail-Vorlage als bearbeitbar definieren. Das Bearbeitungserlebnis eines Elements ist seinem Typ eindeutig und bietet eine einfache Möglichkeit, mit Inhalten zu arbeiten. Folgende Elemente können in eine E-Mail-Vorlage aufgenommen werden:

* RTF
* Bilder
* Snippets
* Videos

## RTF {#rich-text}

Wenn Sie einen Bereich als Rich-Text definieren, können Benutzer den Inhalt [mit dem Rich-Text-Editor von Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md) bearbeiten. Es gibt zwei Möglichkeiten, ein Rich-Text-Element innerhalb einer E-Mail-Vorlage zu definieren: mktEditable und mktoText. Beachten Sie, dass ein Rich-Text-Element im E-Mail-Editor immer in einen Ausschnitt konvertiert werden kann.

### Option 1: mktEditable {#option-mkteditable}

Da Email Editor 2.0 abwärtskompatibel ist, können einige alte E-Mail-Vorlagen Rich-Text-Elemente spezifizieren, indem class=&quot;mktEditable&quot; für beliebige HTML-Elemente hinzugefügt wird. Dies wird weiterhin unterstützt und die ID des Elements wird als Anzeigename im E-Mail-Editor verwendet.

Erforderliche Attribute

* **class**: &quot;mktEditable&quot;.
* **id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.

Optionale Attribute

* **mktoName** : Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Standardwert

Der Inhalt im HTML-Element (sofern vorhanden) mit class=&quot;mktEditable&quot; wird als Standardwert für das Rich-Text-Element verwendet.

Beispiel:

`<div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

### Option 2: mktoText {#option-mktotext}

Es wird empfohlen, Rich-Text-Elemente mithilfe der Syntax class=&quot;mktoText&quot; anzugeben. Dadurch wird sichergestellt, dass für das Element immer ein richtiger Anzeigename vorhanden ist.

Erforderliche Attribute

* **class**: &quot;mktoText&quot;
* **id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName** : Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Standardwert

Der Inhalt im HTML-Element (sofern vorhanden) mit class=&quot;mktoText&quot; wird als Standardwert für das Rich-Text-Element verwendet.

Beispiel:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

## Bilder {#images}

Sie haben zwei Optionen zum Definieren bearbeitbarer Bildelemente. Sie können entweder einen `<div>` verwenden, der einen Container angibt, in den der `<img>` eingefügt wird, oder einen `<img>` -Tag. Wenn Sie möchten, dass der Endbenutzer einfach ein Bild auswählt, das die Bild-URL zurückgibt (im Gegensatz zum DOM), lesen Sie bitte &quot;Bildvariablen&quot;im folgenden Abschnitt. Mit den folgenden beiden Optionen wird ein HTML `<img>` -Element eingefügt.

### Option 1 - Verwenden eines `<div>` {#option-use-a-div}

Erforderliche Attribute

* **class:** &quot;mktoImg&quot;.
* **id:** ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName :** Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **mktoImgClass:** String. Der Wert hier wird dem Klassenattribut des Elements `<img>` innerhalb des div hinzugefügt.
* **mktoImgSrc:** Wird als Standardwert für das Bild verwendet, das in diesem div platziert wird. Ein Platzhalter wird verwendet, wenn dies weggelassen wird.
* **mktoImgLink:** Geben Sie an, dass die `<img>` von einem `<a>` -Tag mit dieser Ziel-URL umgeben sein sollte. Der Benutzer kann dies im E-Mail-Editor ändern.
* **mktoImgLinkTarget:** Geben Sie an, dass das Tag `<a>` aus dem Attribut mktoImgLink dieses Ziel verwenden soll. Hat keine Auswirkung, wenn mktoImgLink nicht auch verwendet wird.
* **mktoImgWidth:** Wird als Breite auf dem eingeschlossenen `<img>` verwendet.
* **mktoImgHeight:** Wird als Höhe auf dem eingeschlossenen `<img>` verwendet.
* **mktoLockImgSize:** Wird verwendet, um die Höhe und Breite des Elements `<img>` zu entsperren, sodass der Endbenutzer ändern kann (der Standardwert ist &quot;true&quot;, wenn nicht angegeben).
* **mktoLockImgStyle:** Wird zum Sperren der Stileigenschaft des Elements `<img>` verwendet (der Standard lautet &quot;false&quot;).

Standardwert (optional)

**`<img>`**: Wird als `<img>`-Element verwendet, in dem das Bild platziert wird. Nützlich, wenn Sie dem Bild Inline-Stile hinzufügen möchten. Denken Sie daran, umliegende `<a> </a>` -Tags einzuschließen. Wenn der Benutzer also einen Link hinzufügt, wird Ihr Stil nicht entfernt!

Beispiel:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div>`

### Option 2: Verwenden eines \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>Diese Option ermöglicht es Endbenutzern nicht, einen Link zu ihrem Bild hinzuzufügen. Verwenden Sie Option 1, wenn dies für Ihre Vorlage wichtig ist.

Erforderliche Attribute

* **class:** &quot;mktoImg&quot;.
* **id:** ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName:** String. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.  Standardwert (optional)
* **src:** Wird als Standardwert für das Bild verwendet. Ein Platzhalter wird verwendet, wenn dies weggelassen wird.
* **mktoLockImgSize:** Wird verwendet, um die Höhe und Breite des Elements `<img>` zu entsperren, sodass der Endbenutzer ändern kann (der Standardwert ist &quot;true&quot;, wenn nicht angegeben).
* **mktoLockImgStyle:** Wird zum Sperren der Stileigenschaft des Elements `<img>` verwendet (der Standard lautet &quot;false&quot;).

Beispiel:
`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

## Snippets {#snippets}

Wenn Sie eine Region als Snippet definieren, können Endbenutzer wählen, welches genehmigte [Snippet](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md) eingefügt werden soll. Rich-Text-Elemente können zwar im E-Mail-Editor in Snippets konvertiert werden, aber wenn Sie eine Region spezifisch als Snippet definieren, kann sie nicht in Rich-Text konvertiert werden. Sie können einen Snippet-Bereich mit einem `<div>` mit class=&quot;mktoSnippet&quot; angeben.

Erforderliche Attribute

* **id:** ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName:** String. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Standardwert (optional)

**mktoDefaultSnippetId**: Die numerische ID des Marketo-Snippets, die standardmäßig angezeigt werden soll (funktioniert nur, wenn ein Snippet mit dieser ID vorhanden und in diesem Arbeitsbereich genehmigt ist).

Beispiel:

`<div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div>`

## Video {#video}

Wenn Sie eine Region als Video definieren, können Endbenutzer entweder eine YouTube- oder eine Vimeo-URL einfügen, die als Miniaturbild (mit der Schaltfläche &quot;Abspielen&quot;) in die E-Mail eingefügt wird. Sie können einen Videobereich mit einem `<div>` mit class=&quot;mktoVideo&quot; angeben.

Erforderliche Attribute

* **id:** ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName:** String. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **mktoImgClass:** String. Der Wert hier wird zum Klassenattribut der Videominiatur `<img>` innerhalb des div hinzugefügt.

Beispiel:

`<div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div>`

## Variablen {#variables}

Variablen sind wie Token. Definieren Sie sie zunächst im Abschnitt `<head>` Ihrer E-Mail-Vorlage mithilfe von `<meta>` -Tags und verwenden Sie sie dann beliebig oft in der Vorlage. Da sie in der Vorlage definiert sind, kann der Endbenutzer seine Werte entsprechend seinen Regeln ändern. Beachten Sie, dass Sie eine Variable im Umfang als lokal oder global definieren können. Wenn Sie eine Variable in einem &quot;Modul&quot;verwenden (siehe unten) und ein Endbenutzer dieses Modul dupliziert, verfügen lokale Variablen über unabhängige Werte, während globale Variablen für beide Module gelten.

## String {#string}

Wenn Sie eine Variable als Zeichenfolge angeben, kann der Endbenutzer Text in einem Textfeld im E-Mail-Editor eingeben. Sie geben eine String-Variable mit `<meta>` und class=&quot;mktoString&quot; an.

Erforderliche Attribute

* **id:** Referenzierung der Variablen in Ihrer E-Mail-Vorlage.
* **mktoName:** String. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **allowHTML:** Boolean. Steuert, ob der Variablenwert durch HTML maskiert ist. Der Standardwert ist &quot;False&quot;, wenn weggelassen.
* **default**: Standardwert für den String. Leer, wenn weggelassen.
* **mktoModuleScope**: Boolesch. Steuert bei Verwendung in einem Modul, ob die Variable lokal (true) oder global (false) ist. Der Standardwert ist &quot;False&quot;, wenn weggelassen.

Beispieldeklaration:

`<meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me">`

Beispielverwendung:

`${textHeader}`

## Liste {#list}

Wenn Sie eine Variable als Liste angeben, kann der Endbenutzer aus einem Satz von Werten wählen, die Sie im E-Mail-Editor definieren. Sie geben eine List-Variable mit `<meta>` und class=&quot;mktoList&quot; an.

Erforderliche Attribute

* **id**: Referenzierung der Variablen in Ihrer E-Mail-Vorlage.
* **mktoName:** String. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.
* **Werte:** Kommagetrennte Liste von Werten. Muss mindestens eine Zeichenfolge enthalten.

Optionale Attribute

* **default:** Standardwert des Dropdown-Menüs &quot;Auswählen&quot;. Wenn dieser Wert weggelassen wird, wird der erste Wert aus dem Attribut &quot;Werte&quot;verwendet.
* **mktoModuleScope**: Boolesch. Steuert bei Verwendung in einem Modul, ob die Variable lokal (true) oder global (false) ist. Der Standardwert ist &quot;False&quot;, wenn weggelassen.

Beispieldeklaration:

`<meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman">`

Beispielverwendung:

`${textFontFamily}`

## Zahl {#number}

Wenn Sie eine Variable als Zahl angeben, kann der Endbenutzer eine Zahl im E-Mail-Editor eingeben. Sie geben eine Number -Variable mit `<meta>` und class=&quot;mktoNumber&quot; an.

Erforderliche Attribute

* **id**: Referenzierung der Variablen in Ihrer E-Mail-Vorlage.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.
* **default:** Standardmäßiger numerischer Wert für die Variable.

Optionale Attribute

* **min:** Zulässiger Mindestwert.
* **max:** Max. zulässige Werte.
* **Einheiten:** Einheiten, die beim Anzeigen im E-Mail-Editor an den Zahlenwert (z. B. px, pt, em usw.) sowie im resultierenden Code angehängt werden sollen.
* **Schritt:** Wie viele Einheiten die Zahlenvariable um (0,1, 1, 10 usw.) erhöhen/verringern soll. Wenn nicht angegeben, wird standardmäßig 1 verwendet.
* **mktoModuleScope**: Boolesch. Steuert bei Verwendung in einem Modul, ob die Variable lokal (true) oder global (false) ist. Der Standardwert ist &quot;False&quot;, wenn weggelassen.

Beispieldeklaration:

`<meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> `

Beispielverwendung:

`${textFontSize}`

## Farbe {#color}

Wenn Sie eine Variable als Farbe angeben, kann der Endbenutzer einen hexadezimalen Farbwert eingeben oder eine Farbe aus der Farbauswahl im E-Mail-Editor auswählen. Sie legen eine Farbvariable mit `<meta>` mit class=&quot;mktoColor&quot; fest.

Erforderliche Attribute

* **id**: Referenzierung der Variablen in Ihrer E-Mail-Vorlage.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **default:** Standardwert für die Farbe. 6-stelliger Hexadezimalfarbcode. Beispiel: #ffffff.
* **mktoModuleScope**: Boolesch. Steuert bei Verwendung in einem Modul, ob die Variable lokal (true) oder global (false) ist. Der Standardwert ist &quot;False&quot;, wenn weggelassen.

Beispieldeklaration:

`<meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF">`

Beispielverwendung:

`${textColor}`

## Boolesch {#boolean}

Wenn Sie eine Variable als Boolesch angeben, kann der Endbenutzer die Option im E-Mail-Editor aktivieren/deaktivieren. Sie geben eine boolesche Variable mit `<meta>` und class=&quot;mktoBoolean&quot; an.

Erforderliche Attribute

* **id**: Referenzierung der Variablen in Ihrer E-Mail-Vorlage.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **default:** Boolescher Wert, der den Standardstatus des Umschalters bestimmt. False , wenn weggelassen.
* **false_value:** Wert, der eingefügt werden soll, wenn sich der Umschalter in der Stellung &quot;AUS&quot;befindet. False , wenn weggelassen.
* **true_value:** Wert, der eingefügt werden soll, wenn sich der Umschalter an der Position &quot;EIN&quot;befindet. True , wenn weggelassen.
* **false_value_name:** Benutzeroberfläche, die beim Umschalten angezeigt wird, wenn sie sich in Aus-Position befindet. False , wenn weggelassen.
* **true_value_name:** Benutzeroberfläche, die beim Umschalten angezeigt wird, wenn sie sich an der Ein-Position befindet. True , wenn weggelassen.
* **mktoModuleScope**: Boolesch. Steuert bei Verwendung in einem Modul, ob die Variable lokal (true) oder global (false) ist. Der Standardwert ist &quot;False&quot;, wenn weggelassen.

Beispieldeklaration:

`<meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES">`

Beispielverwendung:

`${showFooter}`

## HTML-Block {#html-block}

Wenn Sie eine Variable als HTML-Block angeben, kann der Endbenutzer im E-Mail-Editor eine wörtliche HTML eingeben. Sie geben eine HTML Block-Variable mit `<meta>` und class=&quot;mktoHTML&quot; an.

Erforderliche Attribute

* **id**: Referenzierung der Variablen in Ihrer E-Mail-Vorlage.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **default:** HTML-kodierter Wert, der als Standardinhalt des Blocks dient.
* **mktoModuleScope**: Boolesch. Steuert bei Verwendung in einem Modul, ob die Variable lokal (true) oder global (false) ist. Der Standardwert ist &quot;False&quot;, wenn weggelassen.

Beispieldeklaration:

`<meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel">`

Beispielverwendung:

`${trackingPixel}`

## Bildvariable {#image-variable}

Wenn Sie eine Variable als Bild angeben, kann der Endbenutzer ein Bild aus der Bildauswahl im E-Mail-Editor auswählen. Die ausgewählte Bild-URL ist der Wert der -Variablen. Sie geben eine Bildvariable mit `<meta>` mit class=&quot;mktoImg&quot; an.

Erforderliche Attribute

* **id**: Referenzierung der Variablen in Ihrer E-Mail-Vorlage.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **default:** Standard-Bild-URL für das Element.
* **mktoModuleScope**: Boolesch. Steuert bei Verwendung in einem Modul, ob die Variable lokal (true) oder global (false) ist. Der Standardwert ist &quot;False&quot;, wenn weggelassen.

Beispieldeklaration:

`<meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg">`

Beispielverwendung:

`${heroBackgroundImage}`

## Module {#modules}

Module sind vorlagenbasierte Abschnitte, die auf Vorlagenebene definiert sind und Endbenutzern das Einfügen in ihre E-Mail ermöglichen. Da Sie diese Module vorkonfiguriert haben, können Sie sicherstellen, dass sie mit dem Rest Ihres E-Mail-Inhalts ordnungsgemäß interagieren (auf vollständig responsive Weise). Sie können nur ein Modul in einen Container einfügen.

>[!IMPORTANT]
>
>Wenn eine E-Mail aus einer E-Mail-Vorlage generiert wird, die definierte Modulkomponenten enthält, werden alle Änderungen an den Modulen der Vorlage **nicht** an diese E-Mail gesendet.

**Für Container des Typs `<table>`, `<tbody>`, `<thead>` oder `<tfoot>`:**

Wird mit `<tr>` mit class=&quot;mktoModule&quot; angegeben

**Für Container des Typs `<td>`:**

Wird mit `<table>` mit class=&quot;mktoModule&quot; angegeben

Erforderliche Attribute

* **id**: Referenzierung des Moduls in Ihrer E-Mail-Vorlage.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der in Email Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **mktoActive:** Bestimmt, ob dieses Modul in der Modulliste im E-Mail-Editor angezeigt wird. Der Standardwert ist &quot;true&quot;. Bei &quot;false&quot;kann das Modul von einem Endbenutzer nicht zu einer E-Mail hinzugefügt werden.
* **mktoAddByDefault:** Bestimmt, ob sich dieses Modul auf der Arbeitsfläche einer neuen E-Mail befindet, die diese Vorlage bei der Erstellung verwendet. Die Standardeinstellung ist &quot;true&quot;(wenn mktoActive &quot;false&quot;ist, wird dieser Wert ignoriert).

>[!NOTE]
>
>Bei Klassenwerten mit Marketo-Syntax (d. h. mktoModule, mktoContainer, mktoText) wird zwischen Groß- und Kleinschreibung unterschieden. Benutzerdefinierte Attributnamen (d. h. mktoimgwidth, mktoname) sind nicht vorhanden.

## Container {#containers}

Ein Container enthält Module und definiert, wo sie platziert werden können. Wenn Endbenutzer Module neu anordnen und in ihre E-Mail einfügen, steuert der Container, wohin sie gehen können.

**Wird entweder mit `<table>`, `<tbody>`, `<thead>`, `<tfoot>` oder `<td>` mit class=&quot;mktoContainer&quot;** angegeben.

Erforderliche Attribute

**id**: Referenzierung des Moduls in Ihrer E-Mail-Vorlage.

>[!CAUTION]
>
>Container können nur Module enthalten. Wenn noch etwas Anderes vorhanden ist, wird der Container als ungültig angesehen! Pro Vorlage ist nur ein Container zulässig.
