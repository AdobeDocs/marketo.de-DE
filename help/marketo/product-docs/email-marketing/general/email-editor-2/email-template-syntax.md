---
unique-page-id: 11371040
description: Syntax von E-Mail-Vorlagen - Marketo-Dokumente - Produktdokumentation
title: E-Mail-Vorlagensyntax
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: a9f880bd32d533613020d0472c0e1bee07ab388c
workflow-type: tm+mt
source-wordcount: '2449'
ht-degree: 1%

---

# E-Mail-Vorlagensyntax {#email-template-syntax}

In Marketos neuer E-Mail-2.0-Version bestehen E-Mail-Vorlagen aus einer beliebigen Kombination von Elementen, Variablen, Modulen oder Containern. Jeder wird durch Hinzufügen einer Marketo-spezifischen Syntax zu Ihrem HTML definiert. Alte E-Mail-Vorlagen (v1.0) werden in E-Mail-Editor 2.0 unterstützt, enthalten jedoch nicht alle Funktionen des neuen Editors.

Die Marketo-E-Mail-Syntax funktioniert nur in Vorlagen und einzelnen E **Mails. Sie funktioniert nicht** wenn sie in Snippets oder Rich-Text-Token eingebettet ist.

>[!NOTE]
>
>Der Marketo-Support ist nicht für die Unterstützung von CSS/HTML eingerichtet. Wenn Sie nicht mit CSS/HTML vertraut sind, wenden Sie sich bitte an Ihren Entwickler.

>[!CAUTION]
>
>Bei Klassenwerten, die die Marketo-Syntax enthalten (d. h. mktoModule, mktoContainer, mktoText) wird zwischen Groß- und Kleinschreibung unterschieden. Benutzerdefinierte Attributnamen (d. h. mktoimgwidth, mktoname) werden nicht unterstützt.

## Elementen {#elements}

Elemente sind Inhaltsbereiche, die Sie in Ihrer E-Mail-Vorlage als bearbeitbar definieren. Das Bearbeitungserlebnis eines Elements ist einzigartig in seinem Typ und bietet eine einfache Möglichkeit, mit Inhalten zu arbeiten. Zu den möglichen Elementen, die in eine E-Mail-Vorlage aufgenommen werden können, gehören:

* RTF
* Bilder
* Snippets
* Videos

## RTF {#rich-text}

Wenn Sie eine Region als Rich-Text definieren, können Benutzende ihren Inhalt bearbeiten [mit dem Rich-Text-Editor von Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). Es gibt zwei Möglichkeiten, ein Rich-Text-Element innerhalb einer E-Mail-Vorlage zu definieren: mktEditable und mktoText. Ein Rich-Text-Element kann immer aus dem E-Mail-Editor in ein Snippet konvertiert werden.

### Option 1: mktEditable {#option-mkteditable}

Da E-Mail-Editor 2.0 abwärtskompatibel ist, können einige alte E-Mail-Vorlagen Rich-Textelemente angeben, indem class=„mktEditable“ zu einem beliebigen HTML-Element hinzugefügt wird. Dies wird weiterhin unterstützt und die ID des Elements wird als Anzeigename im E-Mail-Editor verwendet.

Erforderliche Attribute

* **class**: „mktEditable“.
* **id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.

Optionale Attribute

* **mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Standardwert

Der Inhalt innerhalb des HTML-Elements (falls bereitgestellt) mit class=„mktEditable“ wird als Standardwert für das Rich-Text-Element verwendet.

Beispiel:

`<div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

### Option 2: mktoText {#option-mktotext}

Es wird empfohlen, Rich-Text-Elemente mit der Syntax class=„motoText“ anzugeben. Dadurch wird sichergestellt, dass immer ein geeigneter Anzeigename für das Element vorhanden ist.

Erforderliche Attribute

* **class**: „mktoText“
* **id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Standardwert

Der Inhalt innerhalb des HTML-Elements (falls bereitgestellt) mit class=„mktoText“ wird als Standardwert für das Rich-Text-Element verwendet.

Beispiel:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

## Bilder {#images}

Zum Definieren bearbeitbarer Bildelemente stehen zwei Optionen zur Verfügung. Sie können entweder ein `<div>`, das einen Container angibt, in den das `<img>` eingefügt wird, oder ein `<img>` Tag verwenden. Wenn der Endbenutzer einfach ein Bild auswählen soll, das die Bild-URL zurückgibt (im Gegensatz zum DOM), lesen Sie den Abschnitt „Bildvariablen“ unten. Mit den folgenden beiden Optionen wird ein HTML-`<img>` eingefügt.

### Option 1: Verwenden eines `<div>` {#option-use-a-div}

Erforderliche Attribute

* **class:** „mktoImg“.
* **id:** ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName :** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **mktoImgClass:** String. Der Wert hier wird zum Klassenattribut des `<img>` Elements im div hinzugefügt.
* **mktoImgSrc:** wird als Standardwert für das Bild verwendet, das in diesem div platziert wird. Ein Platzhalter wird verwendet, wenn dieser weggelassen wird.
* **mktoImgLink:** Geben Sie an, dass das `<img>` von einem `<a>`-Tag mit dieser Ziel-URL umgeben sein soll. Der Benutzer kann dies im E-Mail-Editor ändern.
* **mktoImgLinkTarget:** Geben Sie an, dass das `<a>`-Tag des mktoImgLink-Attributs dieses Ziel verwenden soll. Hat keine Auswirkung, wenn nicht auch mktoImgLink verwendet wird.
* **mktoImgWidth:** Wird als Breite auf dem umschlossenen `<img>` verwendet.
* **mktoImgHeight:** Wird als Höhe auf dem umschlossenen `<img>` verwendet.
* **mktoLockImgSize:** Wird zum Entsperren der height-Eigenschaft und width des `<img>`-Elements verwendet, sodass der Endbenutzer sie ändern kann (standardmäßig „true“, wenn sie weggelassen wird).
* **mktoLockImgStyle:** Wird zum Sperren der style-Eigenschaft des `<img>`-Elements verwendet (der Standardwert lautet false).

Standardwert (optional)

**`<img>`**: Wird als `<img>` Element verwendet, in dem das Bild platziert werden soll. Dies ist nützlich, wenn Sie dem Bild Inline-Stile hinzufügen möchten. Denken Sie daran, die umgebenden `<a> </a>`-Tags einzuschließen, damit Ihre Formatierung nicht entfernt wird, wenn der Benutzer einen Link hinzufügt!

Beispiel:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div>`

### Option 2: Verwenden eines \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>Diese Option erlaubt es Endbenutzern nicht, einen Link zu ihrem Bild hinzuzufügen. Verwenden Sie Option 1, wenn dies für Ihre Vorlage wichtig ist.

Erforderliche Attribute

* **class:** „mktoImg“.
* **id:** ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.  Standardwert (optional)
* **src:** wird als Standardwert für das Bild verwendet. Ein Platzhalter wird verwendet, wenn dieser weggelassen wird.
* **mktoLockImgSize:** Wird zum Entsperren der height-Eigenschaft und width des `<img>`-Elements verwendet, sodass der Endbenutzer sie ändern kann (standardmäßig „true“, wenn sie weggelassen wird).
* **mktoLockImgStyle:** Wird zum Sperren der style-Eigenschaft des `<img>`-Elements verwendet (der Standardwert lautet false).

Beispiel:
`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

## Snippets {#snippets}

Wenn Sie einen Bereich als Snippet definieren, können Endbenutzer auswählen, welcher genehmigte [Snippet](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md) in diesen Bereich eingefügt werden soll. Rich-Text-Elemente können zwar aus dem E-Mail-Editor in Snippets konvertiert werden, wenn Sie jedoch einen Bereich speziell als Snippet definieren, kann er nicht in Rich-Text konvertiert werden. Sie können einen Snippet-Bereich mithilfe eines `<div>` mit class=„mktoSnippet“ angeben.

Erforderliche Attribute

* **id:** ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Standardwert (optional)

**mktoDefaultSnippetId**: Die numerische ID des Marketo-Snippets, das standardmäßig angezeigt werden soll (funktioniert nur, wenn ein Snippet mit dieser ID vorhanden und in diesem Arbeitsbereich genehmigt ist).

Beispiel:

`<div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div>`

## Video {#video}

Wenn Sie eine Region als Video definieren, können Endbenutzer entweder eine YouTube- oder eine Vimeo-URL einfügen, die als Miniaturbild (mit der Schaltfläche „Abspielen„) in die E-Mail eingefügt wird. Sie können eine Videoregion mithilfe eines `<div>` mit class=„mktoVideo“ angeben

Erforderliche Attribute

* **id:** ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **mktoImgClass:** String. Der Wert hier wird zum Klassenattribut der Videominiatur `<img>` im div hinzugefügt.

Beispiel:

`<div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div>`

## Variablen {#variables}

Variablen sind wie Token. Definieren Sie sie zunächst mithilfe von `<meta>`-Tags im Abschnitt `<head>` Ihrer E-Mail-Vorlage und verwenden Sie sie dann in Ihrer Vorlage beliebig oft. Da sie in der Vorlage definiert sind, können Endbenutzer ihre Werte entsprechend ihren Regeln ändern. Beachten Sie, dass Sie eine Variable im Gültigkeitsbereich als lokal oder global definieren können. Wenn Sie eine Variable in einem „Modul“ verwenden (siehe unten) und ein Endbenutzer dieses Modul dupliziert, haben lokale Variablen unabhängige Werte, während globale Variablen für beide Module gelten.

## String {#string}

Wenn Sie eine Variable als Zeichenfolge angeben, kann der Endbenutzer Text in ein Textfeld im E-Mail-Editor eingeben. Sie geben eine Zeichenfolgenvariable mithilfe von `<meta>` mit class=„mktoString“ an

Erforderliche Attribute

* **id:** wie Sie in Ihrer E-Mail-Vorlage auf die Variable verweisen.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **allowHTML:** Boolean. Steuert, ob der Wert der Variablen mit HTML-Escape-Zeichen versehen wird. Die Standardeinstellung ist False, wenn ausgelassen.
* **default**: Standardwert für die Zeichenfolge. Leer, wenn weggelassen.
* **mktoModuleScope**: Boolean. Steuert, ob die Variable lokal (true) oder global (false) ist, wenn sie in einem Modul verwendet wird. Die Standardeinstellung ist False, wenn ausgelassen.

Beispieldeklaration:

`<meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me">`

Beispielverwendung:

`${textHeader}`

## Liste {#list}

Wenn Sie eine Variable als Liste angeben, kann der Endbenutzer aus einem Satz von Werten auswählen, die Sie im E-Mail-Editor definieren. Sie geben eine Listenvariable mithilfe von `<meta>` mit class=„mktoList“ an

Erforderliche Attribute

* **id**: So referenzieren Sie die Variable in Ihrer E-Mail-Vorlage.
* **mktoName:** Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.
* **values** Eine kommagetrennte Liste von Werten. Muss mindestens eine Zeichenfolge haben.

Optionale Attribute

* **default:** Standardwert des Dropdown-Menüs „Auswählen“. Wenn ausgelassen, wird der erste Wert aus dem Attribut „values“ verwendet.
* **mktoModuleScope**: Boolean. Steuert, ob die Variable lokal (true) oder global (false) ist, wenn sie in einem Modul verwendet wird. Die Standardeinstellung ist False, wenn ausgelassen.

Beispieldeklaration:

`<meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman">`

Beispielverwendung:

`${textFontFamily}`

## Zahl {#number}

Wenn Sie eine Variable als Zahl angeben, kann der Endbenutzer eine Zahl im E-Mail-Editor eingeben. Sie geben eine Number-Variable mithilfe von `<meta>` mit class=„mktoNumber“ an

Erforderliche Attribute

* **id**: So referenzieren Sie die Variable in Ihrer E-Mail-Vorlage.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.
* **default:** numerischer Standardwert für die Variable.

Optionale Attribute

* **min:** Akzeptierter Mindestwert.
* **max:** Maximaler akzeptierter Wert.
* **units:** Einheiten, die an den Zahlenwert (z. B. px, pt, em usw.) angehängt werden sollen, wenn sie im E-Mail-Editor sowie im resultierenden Code angezeigt werden.
* **Schritt:** wie viele Einheiten die Zahlenvariable um (0,1, 1, 10 usw.) erhöhen/verringern soll. Wenn ausgelassen, wird standardmäßig 1 verwendet.
* **mktoModuleScope**: Boolean. Steuert, ob die Variable lokal (true) oder global (false) ist, wenn sie in einem Modul verwendet wird. Die Standardeinstellung ist False, wenn ausgelassen.

Beispieldeklaration:

`<meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> `

Beispielverwendung:

`${textFontSize}`

## Farbe {#color}

Wenn Sie eine Variable als Farbe angeben, kann der Endbenutzer einen hexadezimalen Farbwert eingeben oder eine Farbe aus der Farbauswahl im E-Mail-Editor auswählen. Sie geben eine Farbvariable mithilfe von `<meta>` mit class=„mktoColor“ an.

Erforderliche Attribute

* **id**: So referenzieren Sie die Variable in Ihrer E-Mail-Vorlage.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **default:** Standardwert für die Farbe. 6-stelliger HEX-Farbcode. Beispiel: #ffffff.
* **mktoModuleScope**: Boolean. Steuert, ob die Variable lokal (true) oder global (false) ist, wenn sie in einem Modul verwendet wird. Die Standardeinstellung ist False, wenn ausgelassen.

Beispieldeklaration:

`<meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF">`

Beispielverwendung:

`${textColor}`

## Boolesch {#boolean}

Wenn Sie eine Variable als Booleschen Wert angeben, können Endbenutzer die Option im E-Mail-Editor aktivieren/deaktivieren. Sie geben eine boolesche Variable mithilfe von `<meta>` mit class=„mktoBoolean“ an

Erforderliche Attribute

* **id**: So referenzieren Sie die Variable in Ihrer E-Mail-Vorlage.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **default:** boolescher Wert, der den Standardstatus des Umschalter bestimmt. False, wenn ausgelassen.
* **false_value:** Wert, der eingefügt werden soll, wenn der Umschalter in der OFF-Position ist. False, wenn ausgelassen.
* **true_value:** Wert, der eingefügt werden soll, wenn der Umschalter auf „EIN“ steht. True, wenn weggelassen.
* **false_value_name:** Benutzeroberfläche, die im Umschalter angezeigt wird, wenn sie sich in der OFF-Position befindet. False, wenn ausgelassen.
* **true_value_name:** Benutzeroberfläche, die im Umschalter angezeigt wird, wenn sich diese in der Position „EIN“ befindet. True, wenn weggelassen.
* **mktoModuleScope**: Boolean. Steuert, ob die Variable lokal (true) oder global (false) ist, wenn sie in einem Modul verwendet wird. Die Standardeinstellung ist False, wenn ausgelassen.

Beispieldeklaration:

`<meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES">`

Beispielverwendung:

`${showFooter}`

## HTML {#html-block}

Wenn Sie eine Variable als HTML-Block angeben, kann der Endbenutzer bzw. die Endbenutzerin wörtliches HTML aus dem E-Mail-Editor heraus eingeben. Sie geben eine HTML-Blockvariable mithilfe von `<meta>` mit class=„mktoHTML“ an

Erforderliche Attribute

* **id**: So referenzieren Sie die Variable in Ihrer E-Mail-Vorlage.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **default:** HTML-kodierter Wert, der als Standardinhalt des Blocks verwendet wird.
* **mktoModuleScope**: Boolean. Steuert, ob die Variable lokal (true) oder global (false) ist, wenn sie in einem Modul verwendet wird. Die Standardeinstellung ist False, wenn ausgelassen.

Beispieldeklaration:

`<meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel">`

Beispielverwendung:

`${trackingPixel}`

## Bildvariable {#image-variable}

Wenn Sie eine Variable als Bild angeben, können Endbenutzer ein Bild aus der Bildauswahl im E-Mail-Editor auswählen. Die ausgewählte Bild-URL ist der Wert der Variablen. Sie geben eine Bildvariable mithilfe von `<meta>` mit class=„mktoImg“ an

Erforderliche Attribute

* **id**: So referenzieren Sie die Variable in Ihrer E-Mail-Vorlage.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **default:** Standardbild-URL für das Element.
* **mktoModuleScope**: Boolean. Steuert, ob die Variable lokal (true) oder global (false) ist, wenn sie in einem Modul verwendet wird. Die Standardeinstellung ist False, wenn ausgelassen.

Beispieldeklaration:

`<meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg">`

Beispielverwendung:

`${heroBackgroundImage}`

## Module {#modules}

Module sind vorlagenbasierte Abschnitte, die auf Vorlagenebene definiert werden und Endbenutzern angezeigt werden, damit sie sie in ihre E-Mail einfügen können. Da Sie diese Module bereits vorkonfiguriert haben, können Sie sicherstellen, dass sie mit dem Rest Ihres E-Mail-Inhalts elegant (in vollständig responsiver Weise) interagieren. Ein Modul kann nur in einem Container platziert werden.

>[!IMPORTANT]
>
>Wenn eine E-Mail aus einer E-Mail-Vorlage generiert wird, die definierte Modulkomponenten enthält, werden alle Änderungen, die an den Modulen der Vorlage vorgenommen **,** an diese E-Mail gesendet.

**Für Container vom Typ `<table>`, `<tbody>`, `<thead>` oder `<tfoot>`:**

Wird mithilfe von `<tr>` mit class=„mktoModule“ angegeben

**Für Container vom Typ `<td>`:**

Wird mithilfe von `<table>` mit class=„mktoModule“ angegeben

Erforderliche Attribute

* **id**: So referenzieren Sie das Modul in Ihrer E-Mail-Vorlage.
* **mktoName**: Zeichenfolge. Dies ist der Anzeigename, der im E-Mail-Editor 2.0 angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optionale Attribute

* **mktoActive:** Bestimmt, ob dieses Modul in der Liste der Module im E-Mail-Editor angezeigt wird. Die Standardeinstellung ist true. Bei „false“ kann das Modul nicht von einem Endbenutzer zu einer E-Mail hinzugefügt werden.
* **mktoAddByDefault:** Bestimmt, ob sich dieses Modul auf der Arbeitsfläche einer neuen E-Mail befindet, die diese Vorlage bei der Erstellung verwendet. Der Standardwert ist „true“ (wenn „mktoActive“ „false“ ist, wird dieser Wert ignoriert).

>[!NOTE]
>
>Bei Klassenwerten, die die Marketo-Syntax enthalten (d. h. mktoModule, mktoContainer, mktoText) wird zwischen Groß- und Kleinschreibung unterschieden. Benutzerdefinierte Attributnamen (d. h. mktoimgwidth, mktoname) werden nicht unterstützt.

## Container {#containers}

Ein Container enthält Module und definiert, wo sie platziert werden können. Wenn Endbenutzer Module neu anordnen und in ihre E-Mail einfügen, steuert der Container, wohin sie gehen können.

**Wird entweder mithilfe von `<table>`, `<tbody>`, `<thead>`, `<tfoot>` oder `<td>` mit class=„mktoContainer“ angegeben**

Erforderliche Attribute

**id**: So referenzieren Sie das Modul in Ihrer E-Mail-Vorlage.

>[!CAUTION]
>
>Container können nur Module enthalten. Wenn noch etwas vorhanden ist, wird der Container als ungültig erachtet! Pro Vorlage ist nur ein Container zulässig.
