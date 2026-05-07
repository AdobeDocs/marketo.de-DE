---
unique-page-id: 11371040
description: Informationen zur Syntax von E-Mail-Vorlagen im E-Mail-Editor 2.0. Verwenden Sie die richtige Syntax für Module und bearbeitbare Abschnitte in Vorlagen.
title: Syntax von E-Mail-Vorlagen
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '2464'
ht-degree: 83%

---

# Syntax von E-Mail-Vorlagen {#email-template-syntax}

Im neuen E-Mail-Erlebnis 2.0 von Marketo bestehen E-Mail-Vorlagen aus einer beliebigen Kombination von Elementen, Variablen, Modulen oder Containern. Jede Vorlage wird definiert, indem Sie Marketo-spezifischen Syntax zu Ihrer HTML hinzufügen. Alte E-Mail-Vorlagen (v1.0) werden im E-Mail-Editor 2.0 unterstützt, verfügen jedoch nicht über alle Funktionen des neuen Editors.

Die Marketo-E-Mail-Syntax funktioniert nur in Vorlagen und einzelnen E-Mails. Sie funktioniert **nicht**, wenn sie in Ausschnitte oder Rich-Text-Token eingebettet ist.

>[!NOTE]
>
>Der Marketo-Support unterstützt Sie nicht hinsichtlich CSS/HTML. Wenn Sie nicht mit CSS/HTML vertraut sind, wenden Sie sich bitte an Ihre Entwicklerin bzw. Ihren Entwickler.

>[!CAUTION]
>
>Bei Klassenwerten, die die Marketo-Syntax enthalten (d. h. „mktoModule“, „mktoContainer“, „mktoText“), wird zwischen Groß- und Kleinschreibung unterschieden. Bei benutzerdefinierten Attributnamen (d. h. „mktoimgwidth“, „mktoname“) ist dies nicht der Fall.

## Elemente {#elements}

Elemente sind Inhaltsbereiche, die Sie in Ihrer E-Mail-Vorlage als bearbeitbar definieren. Die Bearbeitung eines Elements ist abhängig vom Typ und bietet eine einfache Möglichkeit, mit Inhalten zu arbeiten. Die möglichen Elemente, die in eine E-Mail-Vorlage aufgenommen werden können, sind:

* Rich Text
* Bilder
* Ausschnitte
* Videos

## Rich Text {#rich-text}

Wenn Sie einen Bereich als Rich Text definieren, können Benutzende seinen Inhalt [mit dem Rich-Text-Editor von Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md) bearbeiten. Es gibt zwei Möglichkeiten, ein Rich-Text-Element innerhalb einer E-Mail-Vorlage zu definieren: „mktEditable“ und „mktoText“. Beachten Sie, dass ein Rich-Text-Element mit dem E-Mail-Editor jederzeit in einen Ausschnitt konvertiert werden kann.

### Option 1: mktEditable {#option-mkteditable}

Da der E-Mail-Editor 2.0 abwärtskompatibel ist, können in einigen alten E-Mail-Vorlagen Rich-Text-Elemente angegeben werden, indem „class=&quot;mktEditable&quot;“ zu einem beliebigen HTML-Element hinzugefügt wird. Dies wird weiterhin unterstützt und die ID des Elements wird als Anzeigename im E-Mail-Editor verwendet.

Erforderliche Attribute

* **class**: &quot;mktEditable&quot;.
* **id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich „-“ und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.

Optionale Attribute

* **mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Standardwert

Der Inhalt innerhalb des HTML-Elements (falls bereitgestellt) mit „class=&quot;mktEditable&quot;“ wird als Standardwert für das Rich-Text-Element verwendet.

Beispiel:

`<div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

### Option 2: mktoText {#option-mktotext}

Es wird empfohlen, Rich-Text-Elemente mit der Syntax class=„motoText“ anzugeben. Dadurch wird sichergestellt, dass immer ein geeigneter Anzeigename für das Element vorhanden ist.

Erforderliche Attribute

* **class**: &quot;mktoText&quot;.
* **id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich „-“ und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Standardwert

Der Inhalt innerhalb des HTML-Elements (falls bereitgestellt) mit „class=&quot;mktoText&quot;“ wird als Standardwert für das Rich-Text-Element verwendet.

Beispiel:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

## Bilder {#images}

Zum Definieren bearbeitbarer Bildelemente stehen zwei Optionen zur Verfügung. Sie können entweder ein `<div>`-Tag verwenden, das einen Container angibt, in den `<img>` eingefügt wird, oder ein `<img>`-Tag. Wenn die Endbenutzerin bzw. der Endbenutzer einfach ein Bild auswählen soll, das die Bild-URL zurückgibt (im Gegensatz zum DOM), lesen Sie den Abschnitt „Bildvariablen“ unten. Mit den folgenden beiden Optionen wird ein `<img>`-HTML-Element eingefügt.

### Option 1: Verwenden von `<div>` {#option-use-a-div}

Erforderliche Attribute

* **class:** &quot;mktoImg&quot;.
* **id:** ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich „-“ und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **mktoImgClass:** Zeichenfolge. Der Wert hier wird zum Klassenattribut des `<img>`-Elements im „div“ hinzugefügt.
* **mktoImgSrc:** Wird als Standardwert für das Bild verwendet, das in diesem „div“ platziert wird. Ein Platzhalter wird verwendet, wenn dies weggelassen wird.
* **mktoImgLink:** Gibt an, dass `<img>` von einem `<a>`-Tag mit dieser Ziel-URL umgeben sein soll. Die Benutzerin bzw. der Benutzer kann dies im E-Mail-Editor ändern.
* **mktoImgLinkTarget:** Gibt an, dass das `<a>`-Tag des mktoImgLink-Attributs dieses Ziel verwenden soll. Hat keine Auswirkung, wenn nicht auch „mktoImgLink“ verwendet wird.
* **mktoImgWidth:** Wird als Breite auf dem umschlossenen `<img>` verwendet.
* **mktoImgHeight:** Wird als Höhe auf dem umschlossenen `<img>` verwendet.
* **mktoLockImgSize:** Wird zum Entsperren der Höhen- und Breiteneigenschaft des `<img>`-Elements verwendet, sodass die Endbenutzerin bzw. der Endbenutzer sie ändern kann (standardmäßig „wahr“, wenn weggelassen).
* **mktoLockImgStyle:** Wird zum Sperren der Stileigenschaft des `<img>`-Elements verwendet (standardmäßig „falsch“).

Standardwert (optional)

**`<img>`**: Wird als `<img>`-Element verwendet, in dem das Bild platziert werden soll. Dies ist nützlich, wenn Sie dem Bild Inline-Stile hinzufügen möchten. Denken Sie daran, die umgebenden `<a> </a>`-Tags einzuschließen, damit Ihre Formatierung nicht entfernt wird, wenn die Benutzerin bzw. der Benutzer einen Link hinzufügt.

Beispiel:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.adobe.com"> <a><img style="border:10px solid red;"></a> </div>`

### Option 2: Verwenden von \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>Diese Option erlaubt es Endbenutzenden nicht, einen Link zu ihrem Bild hinzuzufügen. Verwenden Sie Option 1, wenn dies für Ihre Vorlage wichtig ist.

Erforderliche Attribute

* **class:** &quot;mktoImg&quot;.
* **id:** ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich „-“ und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.  Standardwert (optional)
* **src:** Wird als Standardwert für das Bild verwendet. Ein Platzhalter wird verwendet, wenn dies weggelassen wird.
* **mktoLockImgSize:** Wird zum Entsperren der Höhen- und Breiteneigenschaft des `<img>`-Elements verwendet, sodass die Endbenutzerin bzw. der Endbenutzer sie ändern kann (standardmäßig „wahr“, wenn weggelassen).
* **mktoLockImgStyle:** Wird zum Sperren der Stileigenschaft des `<img>`-Elements verwendet (standardmäßig „falsch“).

Beispiel:
`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

## Ausschnitte {#snippets}

Wenn Sie einen Bereich als Snippet definieren, können Endbenutzer auswählen, welches genehmigte [Snippet](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md) in diesen Bereich eingefügt werden soll. Rich-Text-Elemente können zwar mit dem E-Mail-Editor in Ausschnitte konvertiert werden, wenn Sie jedoch einen Bereich speziell als Ausschnitt definieren, kann er nicht in Rich-Text konvertiert werden. Sie können einen Ausschnittbereich mithilfe eines `<div>` mit „class=&quot;mktoSnippet&quot;“ angeben.

Erforderliche Attribute

* **id:** ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich „-“ und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Standardwert (optional)

**mktoDefaultSnippetId**: Die numerische ID des Marketo-Ausschnitts, die standardmäßig angezeigt werden soll (funktioniert nur, wenn ein Ausschnitt mit dieser ID vorhanden und in diesem Arbeitsbereich genehmigt ist).

Beispiel:

`<div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div>`

## Video {#video}

Wenn Sie einen Bereich als Video definieren, können Endbenutzende entweder eine YouTube- oder Vimeo-URL einfügen, die als Miniaturbild (mit der Schaltfläche „Abspielen“) in die E-Mail eingefügt wird. Sie können eine Videoregion mithilfe eines `<div>` mit „class=&quot;mktoVideo&quot;“ angeben.

Erforderliche Attribute

* **id:** ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich „-“ und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **mktoImgClass:** Zeichenfolge. Der Wert hier wird zum Klassenattribut der Videominiatur `<img>` im „div“ hinzugefügt.

Beispiel:

`<div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div>`

## Variablen {#variables}

Variablen sind wie Token. Sie definieren sie zunächst mithilfe von `<meta>`-Tags im Abschnitt `<head>` Ihrer E-Mail-Vorlage und können sie dann in Ihrer Vorlage beliebig oft verwenden. Da sie in der Vorlage definiert sind, können Endbenutzende ihre Werte entsprechend ihren Regeln ändern. Beachten Sie, dass Sie eine Variable als lokal oder global definieren können. Wenn Sie eine Variable in einem „Modul“ verwenden (siehe unten) und eine Endbenutzerin bzw. ein Endbenutzer dieses Modul dupliziert, haben lokale Variablen unabhängige Werte, während globale Variablen für beide Module gelten.

## String {#string}

Wenn Sie eine Variable als Zeichenfolge definieren, kann die Endbenutzerin bzw. der Endbenutzer Text in ein Textfeld im E-Mail-Editor eingeben. Sie definieren eine Zeichenfolgenvariable mithilfe von `<meta>` mit „class=&quot;mktoString&quot;“.

Erforderliche Attribute

* **id:** Wie Sie in Ihrer E-Mail-Vorlage auf die Variable verweisen.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **allowHTML:** Boolescher Wert. Steuert, ob der Wert der Variablen mit einer HTML-Escape-Sequenz versehen ist. Ist standardmäßig „falsch“, wenn weggelassen.
* **default**: Standardwert für die Zeichenfolge. Leer, wenn weggelassen.
* **mktoModuleScope:** Boolescher Wert. Steuert, ob die Variable lokal (wahr) oder global (falsch) ist, wenn sie in einem Modul verwendet wird. Ist standardmäßig „falsch“, wenn weggelassen.

Beispieldeklaration:

`<meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me">`

Beispielverwendung:

`${textHeader}`

## Liste {#list}

Wenn Sie eine Variable als Liste definieren, kann die Endbenutzerin bzw. der Endbenutzer im E-Mail-Editor aus einem Satz an von Ihnen definierten Werten auswählen. Sie definieren eine Listenvariable mithilfe von `<meta>` mit „class=&quot;mktoList&quot;“.

Erforderliche Attribute

* **id:** Wie Sie in Ihrer E-Mail-Vorlage auf die Variable verweisen.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.
* **values** Eine kommagetrennte Liste an Werten. Muss mindestens eine Zeichenfolge enthalten.

Optionale Attribute

* **default:** Standardwert der Auswahl-Dropdown-Liste. Wenn weggelassen, wird der erste Wert aus dem Attribut „values“ verwendet.
* **mktoModuleScope:** Boolescher Wert. Steuert, ob die Variable lokal (wahr) oder global (falsch) ist, wenn sie in einem Modul verwendet wird. Ist standardmäßig „falsch“, wenn weggelassen.

Beispieldeklaration:

`<meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman">`

Beispielverwendung:

`${textFontFamily}`

## Zahl {#number}

Wenn Sie eine Variable als Zahl definieren, kann die Endbenutzerin bzw. der Endbenutzer eine Zahl im E-Mail-Editor eingeben. Sie definieren eine Zahlenvariable mithilfe von `<meta>` mit „class=&quot;mktoNumber&quot;“.

Erforderliche Attribute

* **id:** Wie Sie in Ihrer E-Mail-Vorlage auf die Variable verweisen.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.
* **default:** Numerischer Standardwert für die Zeichenfolge.

Optionale Attribute

* **min:** Minimaler akzeptierter Wert.
* **max:** Maximaler akzeptierter Wert.
* **units:** Einheiten, die an den Zahlenwert angehängt werden (z. B.: px, pt, em usw.) , wenn sie im E-Mail-Editor sowie im resultierenden Code angezeigt wird.
* **step:** Um wie viele Einheiten die Zahlenvariable erhöht/verringert werden soll („0,1“, „1“, „10“ usw.). Wenn weggelassen, wird standardmäßig „1“ verwendet.
* **mktoModuleScope:** Boolescher Wert. Steuert, ob die Variable lokal (wahr) oder global (falsch) ist, wenn sie in einem Modul verwendet wird. Ist standardmäßig „falsch“, wenn weggelassen.

Beispieldeklaration:

`<meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1">`

Beispielverwendung:

`${textFontSize}`

## Farbe {#color}

Wenn Sie eine Variable als Farbe definieren, kann die Endbenutzerin bzw. der Endbenutzer einen hexadezimalen Farbwert eingeben oder eine Farbe aus dem Farbwähler im E-Mail-Editor auswählen. Sie definieren eine Farbvariable mithilfe von `<meta>` mit „class=&quot;mktoColor&quot;“.

Erforderliche Attribute

* **id:** Wie Sie in Ihrer E-Mail-Vorlage auf die Variable verweisen.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **default:** Standardwert für die Farbe. 6-stelliger Hex-Farb-Code. Beispiel: #ffffff.
* **mktoModuleScope:** Boolescher Wert. Steuert, ob die Variable lokal (wahr) oder global (falsch) ist, wenn sie in einem Modul verwendet wird. Ist standardmäßig „falsch“, wenn weggelassen.

Beispieldeklaration:

`<meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF">`

Beispielverwendung:

`${textColor}`

## Boolesch {#boolean}

Wenn Sie eine Variable als booleschen Wert definieren, können Endbenutzende die Option im E-Mail-Editor aktivieren/deaktivieren. Sie definieren eine boolesche Variable mithilfe von `<meta>` mit „class=&quot;mktoBoolean&quot;“.

Erforderliche Attribute

* **id:** Wie Sie in Ihrer E-Mail-Vorlage auf die Variable verweisen.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **default:** Boolescher Wert, der die Standardeinstellung des Umschalters bestimmt. Falsch, wenn weggelassen.
* **false_value:** Wert, der eingefügt werden soll, wenn der Umschalter deaktiviert ist. Falsch, wenn weggelassen.
* **true_value:** Wert, der eingefügt werden soll, wenn der Umschalter aktiviert ist. Wahr, wenn weggelassen.
* **false_value_name:** Benutzeroberfläche, die angezeigt wird, wenn der Umschalter deaktiviert ist. Falsch, wenn weggelassen.
* **true_value_name:** Benutzeroberfläche, die angezeigt wird, wenn der Umschalter aktiviert ist. Wahr, wenn weggelassen.
* **mktoModuleScope:** Boolescher Wert. Steuert, ob die Variable lokal (wahr) oder global (falsch) ist, wenn sie in einem Modul verwendet wird. Ist standardmäßig „falsch“, wenn weggelassen.

Beispieldeklaration:

`<meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES">`

Beispielverwendung:

`${showFooter}`

## HTML-Block {#html-block}

Wenn Sie eine Variable als HTML-Block definieren, kann die Endbenutzerin bzw. der Endbenutzer HTML wortwörtlich im E-Mail-Editor eingeben. Sie definieren eine HTML-Blockvariable mithilfe von `<meta>` mit „class=&quot;mktoHTML&quot;“.

Erforderliche Attribute

* **id:** Wie Sie in Ihrer E-Mail-Vorlage auf die Variable verweisen.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **Standard:** HTML-kodierter Wert, der als Standardinhalt des Blocks verwendet wird.
* **mktoModuleScope:** Boolescher Wert. Steuert, ob die Variable lokal (wahr) oder global (falsch) ist, wenn sie in einem Modul verwendet wird. Ist standardmäßig „falsch“, wenn weggelassen.

Beispieldeklaration:

`<meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel">`

Beispielverwendung:

`${trackingPixel}`

## Bildvariable {#image-variable}

Wenn Sie eine Variable als Bild definieren, können Endbenutzende ein Bild aus der Bildauswahl im E-Mail-Editor auswählen. Die URL des ausgewählten Bildes ist der Wert der Variablen. Sie definieren eine Bildvariable mithilfe von `<meta>` mit „class=&quot;mktoImg&quot;“.

Erforderliche Attribute

* **id:** Wie Sie in Ihrer E-Mail-Vorlage auf die Variable verweisen.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **default:** Standardmäßige Bild-URL für das Element.
* **mktoModuleScope:** Boolescher Wert. Steuert, ob die Variable lokal (wahr) oder global (falsch) ist, wenn sie in einem Modul verwendet wird. Ist standardmäßig „falsch“, wenn weggelassen.

Beispieldeklaration:

`<meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg">`

Beispielverwendung:

`${heroBackgroundImage}`

## Module {#modules}

Module sind vorlagenbasierte Abschnitte, die auf Vorlagenebene definiert werden. Sie werden Endbenutzenden angezeigt, damit diese sie in ihre E-Mails einfügen können. Da Sie diese Module bereits vorkonfiguriert haben, stellen Sie sicher, dass sie mit dem Rest Ihres E-Mail-Inhalts nahtlos (in vollständig responsiver Weise) interagieren. Sie können nur ein Modul in einem Container platzieren.

>[!IMPORTANT]
>
>Wenn eine E-Mail aus einer E-Mail-Vorlage generiert wird, die definierte Modulkomponenten enthält, werden **keine** an den Modulen der Vorlage vorgenommenen Änderungen an diese E-Mail übertragen.

**Für Container vom Typ `<table>`, `<tbody>`, `<thead>` oder `<tfoot>`:**

Wird mithilfe von `<tr>` mit „class=&quot;mktoModule&quot;“ definiert.

**Für Container vom Typ `<td>`:**

Wird mithilfe von `<table>` mit „class=&quot;mktoModule&quot;“ definiert.

Erforderliche Attribute

* **id:** Wie Sie in Ihrer E-Mail-Vorlage auf das Modul verweisen.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **mktoActive:** Bestimmt, ob dieses Modul in der Liste der Module im E-Mail-Editor angezeigt wird. Ist standardmäßig „wahr“. Wenn „falsch“, kann das Modul nicht von einer Enbenutzerin bzw. einem Endbenutzer zu einer E-Mail hinzugefügt werden.
* **mktoAddByDefault:** Bestimmt, ob sich dieses Modul auf der Arbeitsfläche einer neuen E-Mail befindet, die diese Vorlage bei der Erstellung verwendet. Ist standardmäßig „wahr“ (wenn „mktoActive“ „falsch“ ist, wird dieser Wert ignoriert).

>[!NOTE]
>
>Bei Klassenwerten, die die Marketo-Syntax enthalten (d. h. „mktoModule“, „mktoContainer“, „mktoText“), wird zwischen Groß- und Kleinschreibung unterschieden. Bei benutzerdefinierten Attributnamen (d. h. „mktoimgwidth“, „mktoname“) ist dies nicht der Fall.

## Container {#containers}

Ein Container enthält Module und definiert, wo sie platziert werden können. Wenn Endbenutzende Module neu anordnen und in ihre E-Mail einfügen, steuert der Container, wo Sie platziert werden können.

**Wird entweder mithilfe von `<table>`, `<tbody>`, `<thead>`, `<tfoot>` oder `<td>` mit „class=&quot;mktoContainer&quot;“ definiert**

Erforderliche Attribute

**id:** Wie Sie in Ihrer E-Mail-Vorlage auf das Modul verweisen.

>[!CAUTION]
>
>Container können nur Module enthalten. Wenn noch etwas vorhanden ist, wird der Container als ungültig erachtet. Pro Vorlage ist nur ein Container zulässig.
