---
unique-page-id: 7515401
description: Erstellen einer geführten Landingpage-Vorlage - Marketo-Dokumente - Produktdokumentation
title: Erstellen einer geführten Landingpage-Vorlage
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1265'
ht-degree: 1%

---

# Erstellen einer geführten Landingpage-Vorlage {#create-a-guided-landing-page-template}

Geführte Landingpage-Vorlagen haben eine spezielle Syntax. Verwenden Sie diese Syntax, um anzugeben, was angepasst werden kann und wo die Inhalte auf jeder Landingpage landen, die aus Ihrer Vorlage erstellt wurde. Nur die Regionen oder Variablen, die Sie als bearbeitbar angeben, stehen im „geführten“ Landingpage-Editor zur Anpassung zur Verfügung.

>[!TIP]
>
>Wenn Sie gute Benennungskonventionen verwenden, wird sich Ihr Marketing-Team in Sie verlieben.

Es gibt zwei Möglichkeiten, zu deklarieren, dass etwas auf Ihrer Seite bearbeitbar sein sollte:

* Deklarieren Sie ein -Objekt als „Element“. Der Ersteller der Landingpage kann Bilder, Text oder Marketo-Assets in diese angegebenen Bereiche hinzufügen.
* Deklarieren Sie eine Zeichenfolge als „Variable“. Der Ersteller der Landingpage kann diese Variable durch eine Zeichenfolge, eine Farbe oder einen booleschen Status mit einem „true“-/„false“-Hebel ersetzen.

## Bearbeitbare Elemente {#editable-elements}

-Elemente werden deklariert, indem ein normales DOM-Element zur Vorlage hinzugefügt und das Element dann mit einem Marketo-spezifischen Klassennamen versehen wird.

## Text {#text}

Wenn Sie eine Region als Rich-Text definieren, können Benutzende ihren Inhalt bearbeiten [mit dem Rich-Text-Editor von Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md).

Erforderliche Attribute:\
**class**: „mktoText“\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
Der Inhalt eines Elements mit der Klasse „motoText“ (falls angegeben) wird als Standardwert für den bearbeitbaren Bereich verwendet.

Beispiel:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div>`

## Bild {#image}

Zum Definieren bearbeitbarer Bildelemente stehen zwei Optionen zur Verfügung. Sie können entweder einen `<div>`, der einen Container angibt, in den das Bild eingefügt wird, oder ein `<img>`-Tag verwenden.

## Option 1: Verwenden eines `<div>` {#option-use-a-div}

Erforderliche Attribute:

class: „mktoImg“\
id: ID-String. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
motoName : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
mktoImgClass: Zeichenfolge. Der Wert hier wird zum Klassenattribut des `<img>` Elements im div hinzugefügt.

Beispiel:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image"></div>`

## Option 2: Verwenden eines `<img>` {#option-use-a-img}

Erforderliche Attribute:\
class: „mktoImg“\
id: ID-String. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
motoName : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
src: String-URL. Dies wird als Standardwert für das Bild verwendet.

Beispiel:

`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

>[!NOTE]
>
>Bei Verwendung der `<img>`-Version enthält die gerenderte HTML einen generierten div-Wrapper um das `<img>`-Tag. Er wird auf die Klasse eingestellt.“mktoImg.mktoGen“ festgelegt und wird als display:inline-block angezeigt.

## Formular {#form}

Beispiel: Erforderliche Attribute:\
**class**: „mktoForm“\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

`<div class="mktoForm" id="exampleForm" mktoName="Example Form"></div>`

## Ausschnitt {#snippet}

Erforderliche Attribute:\
**class**: „mktoSnippet“\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div>`

## Schaltfläche Freigeben {#share-button}

Erforderliche Attribute:\
**class**: „mktoShareButton“\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div>`

## Video {#video}

>[!NOTE]
>
>Wenn Sie das Videoelement in einer Landingpage verwenden, unterstützt Marketo nur Videos aus YouTube. Wenn Sie einen anderen Service verwenden, empfehlen wir die Verwendung eines Rich-Text-Felds und das Einfügen in den Einbettungs-Code des Videos.

Erforderliche Attribute:
**class**: „mktoVideo“
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div>`

## Umfrage {#poll}

Erforderliche Attribute:\
**class**: „mktoPoll“\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div>`

## Empfehlung {#referral}

Erforderliche Attribute:\
**class**: „mktoReferral“\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div>`

## Gewinnspiele {#sweepstakes}

Erforderliche Attribute:\
**class**: „mktoSweepstakes“\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div>`

## Bearbeitbare Variablen {#editable-variables}

Alle Variablentypen werden verwendet, indem auf den Wert ihres ID-Attributs verwiesen wird, das in eine ${ }-Zeichensequenz eingeschlossen ist. Sie können überall im Dokument verwendet werden, mit Ausnahme von innerhalb anderer Variablendeklarationen.

Beispiel:

`${var1}`

**Deklaration:**

Variablen werden als Meta-Tags im `<head>` der Vorlage deklariert. Es gibt drei Arten von Variablen, die verwendet werden können: Zeichenfolge, Farbe und Boolesch.

## String {#string}

Erforderliche Attribute:\
**class** : „mktoString“,\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
**default**: Zeichenfolgenwert für das Attribut. Leer, wenn keine angegeben.\
**allowHTML**: „true“ oder „false“. Steuert, ob der Wert gedruckt wird, ohne dass HTML-Escape-Zeichen verwendet werden. Die Standardeinstellung ist „false“, wenn nicht festgelegt.

Einfaches Beispiel:

`<meta class="mktoString" id="var1" mktoName="My Variable">`

Beispiel mit allen Attributen:

`<meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true">`

## Farbe {#color}

Erforderliche Attribute:\
**class** : „mktoColor“,\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
**Standard**: Ein 7-stelliger HEX-Zeichenfarbcode. Beispiel: &quot;#336699“

Einfaches Beispiel:

`<meta class="mktoColor" id="color1" mktoName="My Color Variable">`

Beispiel mit allen Attributen:

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

## Boolesch {#boolean}

Erforderliche Attribute:\
**class** : „mktoBoolean“,\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich &quot;-&quot; und Unterstrich „_“. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
**default**: Boolesche Zeichenfolge. „true“ oder „false“ steuert, ob der Wert in der ON- oder OFF-Position beginnt. „false“, wenn nicht angegeben.\
**false_value**: Zeichenfolge. Der Wert, der für die Variable eingefügt werden soll, wenn sie sich in der OFF-Position befindet. „false“, wenn nicht angegeben.\
**true_value**: Zeichenfolge. Der Wert, der für die Variable eingefügt werden soll, wenn sie sich an der Position „EIN“ befindet. „true“, wenn nicht angegeben.\
**false_value_name**: Zeichenfolge. Der Anzeigename, der im Landingpage-Editor angezeigt werden soll, wenn sich der Wert in der OFF-Position befindet. „OFF“, wenn nicht angegeben.\
**true_value_name**: Zeichenfolge. Der Anzeigename, der im Landingpage-Editor angezeigt werden soll, wenn der Wert auf „EIN“ steht. „EIN“, wenn nicht angegeben.

Einfaches Beispiel:

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable">`

Beispiel mit allen Attributen:

Dieses Beispiel zeigt einen gängigen Anwendungsfall, bei dem eine boolesche Variable die Sichtbarkeit eines CSS-Elements steuert, indem sie den Wert der CSS-Anzeigeeigenschaft entweder auf „block“ oder auf „none“ festlegt, um ein Element anhand der ID mit CSS ein-/auszublenden. Der Landingpage-Editor verwendet den Anzeigenamen Einblenden/Ausblenden anstelle von AUS/EIN.

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style>`

>[!NOTE]
>
>Programm-Token (my.token) können auch überall auf geführten oder Freiform-Landingpages verwendet werden.
