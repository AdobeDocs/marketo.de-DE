---
unique-page-id: 7515401
description: Erstellen einer geführten Landingpage-Vorlage - Marketo Docs - Produktdokumentation
title: Erstellen einer Vorlage für eine geführte Landingpage
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1254'
ht-degree: 2%

---

# Erstellen einer Vorlage für eine geführte Landingpage {#create-a-guided-landing-page-template}

Geführte Landingpage-Vorlagen haben eine spezielle Syntax. Verwenden Sie diese Syntax, um festzulegen, was angepasst werden kann und wo der Inhalt auf jeder aus Ihrer Vorlage erstellten Landingpage landet. Nur die Regionen oder Variablen, die Sie als bearbeitbar angeben, stehen im Landingpage-Editor &quot;Geführt&quot;zur Anpassung zur Verfügung.

>[!TIP]
>
>Verwenden Sie gute Namenskonventionen, und Ihr Marketing-Team wird sich in Sie verlieben.

Es gibt zwei Möglichkeiten, zu deklarieren, dass etwas auf Ihrer Seite bearbeitbar sein sollte:

* Deklarieren Sie ein Objekt als &quot;Element&quot;. Der Ersteller der Landingpage kann Bilder, Texte oder Marketo-Assets zu den angegebenen Bereichen hinzufügen.
* Deklarieren Sie eine Zeichenfolge als &quot;Variable&quot;. Der Ersteller der Landingpage kann diese Variable durch einen String-, Farb- oder booleschen Status aus einem true/false-Hebel ersetzen.

## Bearbeitbare Elemente {#editable-elements}

Elemente werden deklariert, indem ein normales DOM-Element zur Vorlage hinzugefügt und das Element dann mit einem Marketo-spezifischen Klassennamen dekoriert wird.

## Text {#text}

Wenn Sie eine Region als Rich-Text definieren, können Benutzer den Inhalt bearbeiten [Verwenden des Rich-Text-Editors von Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md).

Erforderliche Attribute:\
**class**: &quot;mktoText&quot;\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
Der Inhalt eines Elements mit der Klasse mktoText (sofern verfügbar) wird als Standardwert für den bearbeitbaren Bereich verwendet.

Beispiel:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div>`

## Bild {#image}

Sie haben zwei Optionen zum Definieren bearbeitbarer Bildelemente. Sie können entweder eine `<div>`, der einen Container angibt, in den das Bild eingefügt wird, oder einen `<img>` -Tag.

## Option 1: Verwenden eines `<div>` {#option-use-a-div}

Erforderliche Attribute:

class: &quot;mktoImg&quot;\
id: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
mktoName : String. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
mktoImgClass: String. Der Wert hier wird dem class -Attribut der `<img>` -Element innerhalb des div.

Beispiel:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image"></div>`

## Option 2: Verwenden Sie eine `<img>` {#option-use-a-img}

Erforderliche Attribute:\
class: &quot;mktoImg&quot;\
id: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
mktoName : String. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
src: String-URL. Dies wird als Standardwert für das Bild verwendet.

Beispiel:

`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

>[!NOTE]
>
>Bei Verwendung von `<img>` -Version enthält die gerenderte HTML einen generierten Div-Wrapper um die `<img>` -Tag. Sie wird auf class festgelegt.&quot;mktoImg.mktoGen&quot; und werden angezeigt:inline-block.

## Formular {#form}

Beispiel: Erforderliche Attribute:\
**class**: &quot;mktoForm&quot;\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

`<div class="mktoForm" id="exampleForm" mktoName="Example Form"></div>`

## Ausschnitt {#snippet}

Erforderliche Attribute:\
**class**: &quot;mktoSnippet&quot;\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div>`

## Schaltfläche &quot;Freigeben&quot; {#share-button}

Erforderliche Attribute:\
**class**: &quot;mktoShareButton&quot;\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div>`

## Video {#video}

>[!NOTE]
>
>Bei Verwendung des Videoelements in einer Landingpage unterstützt Marketo nur Videos aus YouTube. Wenn Sie einen anderen Dienst verwenden, empfehlen wir, ein Rich-Text-Feld zu verwenden und den Einbettungscode des Videos einzufügen.

Erforderliche Attribute:
**class**: &quot;mktoVideo&quot;
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div>`

## Umfrage {#poll}

Erforderliche Attribute:\
**class**: &quot;mktoPoll&quot;\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div>`

## Empfehlung {#referral}

Erforderliche Attribute:\
**class**: &quot;mktoReferral&quot;\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div>`

## Gewinnspiele {#sweepstakes}

Erforderliche Attribute:\
**class**: &quot;mktoSweepstakes&quot;\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div>`

## Bearbeitbare Variablen {#editable-variables}

Alle Variablentypen werden verwendet, indem auf den Wert ihres id-Attributs verwiesen wird, das in eine ${ } -Zeichensequenz eingeschlossen ist. Sie können überall im Dokument verwendet werden, außer in anderen Variablendeklarationen.

Beispiel:

`${var1}`

**Erklärung:**

Variablen werden als Meta-Tags innerhalb der `<head>` -Element der Vorlage. Es stehen drei Variablentypen zur Verfügung: Zeichenfolge, Farbe und Boolesch.

## Zeichenfolge {#string}

Erforderliche Attribute:\
**class** : &quot;mktoString&quot;,\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
**default**: Zeichenfolgenwert für das Attribut. Leer, wenn keine angegeben ist.\
**allowHtml**: &quot;true&quot;oder &quot;false&quot;. Steuert, ob der Wert gedruckt wird, ohne dass HTML maskiert wird. Die Standardeinstellung ist &quot;false&quot;, wenn nicht festgelegt.

Grundlegendes Beispiel:

`<meta class="mktoString" id="var1" mktoName="My Variable">`

Beispiel mit allen Attributen:

`<meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true">`

## Farbe {#color}

Erforderliche Attribute:\
**class** : &quot;mktoColor&quot;,\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
**default**: Ein 7-stelliger HEX-Zeichenfarbcode. Beispiel: &quot;#336699&quot;

Grundlegendes Beispiel:

`<meta class="mktoColor" id="color1" mktoName="My Color Variable">`

Beispiel mit allen Attributen:

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

## Boolesch {#boolean}

Erforderliche Attribute:\
**class** : &quot;mktoBoolean&quot;,\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestriche &quot;-&quot;und Unterstriche &quot;_&quot;. Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
**default**: Boolesche Zeichenfolge. &quot;true&quot;oder &quot;false&quot;steuert, ob der Wert in der EIN- oder AUS-Position beginnt. &quot;false&quot;, wenn nicht angegeben.\
**false_value**: Zeichenfolge. Der Wert, der für die Variable eingefügt werden soll, wenn sie sich in der Stellung &quot;AUS&quot;befindet. &quot;false&quot;, wenn nicht angegeben.\
**true_value**: Zeichenfolge. Der Wert, der für die Variable eingefügt werden soll, wenn sie sich an der Position &quot;ON&quot;befindet. &quot;true&quot;, wenn nicht angegeben.\
**false_value_name**: Zeichenfolge. Der Anzeigename, der im Landingpage-Editor angezeigt wird, wenn sich der Wert in der Stellung &quot;AUS&quot;befindet. &quot;AUS&quot;, falls nicht angegeben.\
**true_value_name**: Zeichenfolge. Der Anzeigename, der im Landingpage-Editor angezeigt wird, wenn sich der Wert an der Position &quot;EIN&quot;befindet. &quot;ON&quot;, falls nicht angegeben.

Grundlegendes Beispiel:

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable">`

Beispiel mit allen Attributen:

Dieses Beispiel zeigt einen häufigen Anwendungsfall, bei dem eine boolesche Variable die Sichtbarkeit eines CSS-Elements steuert, indem sie den Wert der CSS-Anzeigeeigenschaft auf &quot;block&quot;oder &quot;none&quot;setzt, um ein Element anhand der ID mit CSS anzuzeigen/auszublenden. Der Landingpage-Editor verwendet den Anzeigenamen &quot;Einblenden/Ausblenden&quot;anstelle von &quot;AUS/ON&quot;.

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style>`

>[!NOTE]
>
>Programm-Token (my.token) können auch überall auf Landingpages mit Guided oder Free-Form verwendet werden.
