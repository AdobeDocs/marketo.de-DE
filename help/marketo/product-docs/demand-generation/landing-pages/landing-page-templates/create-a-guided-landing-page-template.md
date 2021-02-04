---
unique-page-id: 7515401
description: Erstellen einer Vorlage für die Landingpage mit Guided - Marketing Docs - Produktdokumentation
title: Erstellen einer Vorlage für eine Landingpage mit Guided
translation-type: tm+mt
source-git-commit: 2969e6f94f5fd781e2167ae2aa8680bb8d134754
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 0%

---


# Erstellen einer Vorlage für eine geführte Landingpage {#create-a-guided-landing-page-template}

>[!NOTE]
>
>Lese müde? [Sehen Sie sich dieses coole ](https://youtu.be/3O7e4GdZKsM) Video mit schrittweisen Anleitungen an.

Vorlagen für Landingpages mit Guided haben eine spezielle Syntax. Verwenden Sie diese Syntax, um anzugeben, was anpassbar ist und wo der Inhalt auf jeder Landingpage landet, die aus Ihrer Vorlage erstellt wurde. Nur die als bearbeitbar angegebenen Regionen oder Variablen können im Editor für geführte Landingpages angepasst werden.

>[!TIP]
>
>Verwenden Sie gute Benennungskonventionen, und Ihr Marketing-Team wird sich in Sie verlieben.

Es gibt zwei Möglichkeiten, zu erklären, dass etwas auf Ihrer Seite bearbeitbar sein sollte:

* Deklarieren Sie ein Objekt als &quot;Element&quot;. Der Ersteller der Landingpage kann Bilder, Texte oder Markets zu den angegebenen Bereichen hinzufügen.
* Deklarieren Sie eine Zeichenfolge als &quot;Variable&quot;. Der Ersteller der Landingpage kann diese Variable durch einen String-, Farb- oder booleschen Status aus einem true/false-Hebel ersetzen.

## Bearbeitbare Elemente {#editable-elements}

Elemente werden deklariert, indem der Vorlage ein normales DOM-Element hinzugefügt und anschließend das Element mit einem Marketo-spezifischen Klassennamen dekoriert wird.

## Text {#text}

Wenn Sie einen Bereich als Rich Text definieren, können Benutzer den Inhalt [mit dem Rich Text Editor von Marketo bearbeiten.](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)

Erforderliche Attribute:\
**class**: &quot;mktoText&quot;\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
Der Inhalt eines Elements mit der Klasse mktoText (sofern vorhanden) wird als Standardwert für den bearbeitbaren Bereich verwendet.

Beispiel:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div></pre>`

### Bild {#image}

Sie haben zwei Optionen zum Definieren bearbeitbarer Bildelemente. Sie können entweder ein `<div>` verwenden, das einen Container angibt, in den das Bild eingefügt wird, oder ein `<img>`-Tag.

## Option 1: Verwenden Sie eine `<div>` {#option-use-a-div}

Erforderliche Attribute:

class: &quot;mktoImg&quot;\
id: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
mktoName: Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
mktoImgClass: Zeichenfolge. Der Wert hier wird dem Klassenattribut des Elements `<img>` innerhalb des div hinzugefügt.

Beispiel:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image"></div></pre>`

## Option 2: Verwenden Sie eine `<img>` {#option-use-a-img}

Erforderliche Attribute:\
class: &quot;mktoImg&quot;\
id: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
mktoName: Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
src: String-URL. Dies wird als Standardwert für das Bild verwendet.

Beispiel:

`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

>[!NOTE]
>
>Bei Verwendung der `<img>`-Version enthält der gerenderte HTML-Code einen generierten div-Wrapper um das `<img>`-Tag. Es wird auf class festgelegt.&quot;mktoImg.mktoGen,&quot; und wird angezeigt:inline-block.

## Formular {#form}

Beispiel: Erforderliche Attribute:\
**class**: &quot;mktoForm&quot;\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

`<pre data-theme="Confluence"><div class="mktoForm" id="exampleForm" mktoName="Example Form"></div></pre>`

## Ausschnitt {#snippet}

Erforderliche Attribute:\
**class**: &quot;mktoSnippet&quot;\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div></pre>`

## Freigabebeschaltfläche {#share-button}

Erforderliche Attribute:\
**class**: &quot;mktoShareButton&quot;\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<pre data-theme="Confluence"><div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div></pre>`

## Video {#video}

>[!NOTE]
>
>Wenn Sie das Videoelement in einer Landingpage verwenden, unterstützt Marketo nur Videos von YouTube. Wenn Sie einen anderen Dienst verwenden, sollten Sie ein Rich-Text-Feld verwenden und den Einbettungscode des Videos einfügen.

Erforderliche Attribute:
**class**: &quot;mktoVideo&quot;
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<pre data-theme="Confluence"><div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div></pre>`

## Umfrage {#poll}

Erforderliche Attribute:\
**class**: &quot;mktoPoll&quot;\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<pre data-theme="Confluence"><div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div></pre>`

## Verweis {#referral}

Erforderliche Attribute:\
**class**: &quot;mktoReferral&quot;\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<pre data-theme="Confluence"><div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div></pre>`

## Preisausschreiben {#sweepstakes}

Erforderliche Attribute:\
**class**: &quot;mktoSweepstakes&quot;\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Beispiel:

`<pre data-theme="Confluence"><div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div></pre>`

## Bearbeitbare Variablen {#editable-variables}

Alle Variablentypen werden verwendet, indem auf den Wert ihres id-Attributs verwiesen wird, das in eine ${ }-Zeichensequenz eingeschlossen ist. Sie können überall im Dokument verwendet werden, außer innerhalb anderer Variablendeklarationen.

Beispiel:

`<pre data-theme="Confluence">${var1}</pre>`

**Erklärung:**

Variablen werden als Meta-Tags innerhalb des Elements `<head>` der Vorlage deklariert. Es stehen drei Variablentypen zur Verfügung: Zeichenfolge, Farbe und Boolescher Wert.

## Zeichenfolge {#string}

Erforderliche Attribute:\
**class** : &quot;mktoString&quot;,\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
**Standard**: Zeichenfolgenwert für das Attribut. Leer, wenn keine angegeben ist.\
**allowHtml**: &quot;true&quot;oder &quot;false&quot;. Steuert, ob der Wert gedruckt wird, ohne dass HTML-Escape-Zeichen verwendet werden. Der Standardwert lautet &quot;false&quot;(falsch), wenn das Kontrollkästchen deaktiviert ist.

Grundlegendes Beispiel:

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable"></pre>`

Beispiel mit allen Attributen:

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true"></pre>`

## Farbe {#color}

Erforderliche Attribute:\
**class** : &quot;mktoColor&quot;,\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
**Standard**: Ein 7-stelliger HEX-Zeichenfarbcode. z. B.: &quot;#336699&quot;

Grundlegendes Beispiel:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color1" mktoName="My Color Variable"></pre>`

Beispiel mit allen Attributen:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

## Boolean {#boolean}

Erforderliche Attribute:\
**class** : &quot;mktoBoolean&quot;,\
**id**: ID-Zeichenfolge. Enthält nur Buchstaben, Zahlen, Bindestrich (-) und Unterstrich (_). Leerzeichen sind nicht zulässig. Muss eindeutig sein.\
**mktoName** : Zeichenfolge. Dies ist der Anzeigename, der im Landingpage-Editor angezeigt wird. Es empfiehlt sich, einen beschreibenden Namen zu verwenden.

Optional:\
**Standard**: Boolescher String. &quot;true&quot;oder &quot;false&quot;steuert, wenn der Wert in der EIN- oder AUS-Position Beginn. &quot;false&quot;, wenn nicht angegeben.\
**false_value**: Zeichenfolge. Der Wert, der für die Variable eingefügt werden soll, wenn sie sich in der Stellung OFF befindet. &quot;false&quot;, wenn nicht angegeben.\
**true_value**: Zeichenfolge. Der Wert, der für die Variable eingefügt werden soll, wenn sie sich an der Position ON befindet. &quot;true&quot;, wenn nicht angegeben.\
**false_value_name**: Zeichenfolge. Der Anzeigename, der im Landingpages-Editor angezeigt wird, wenn sich der Wert an der Stellung &quot;OFF&quot;befindet. &quot;AUS&quot;, wenn nicht angegeben.\
**true_value_name**: Zeichenfolge. Der Anzeigename, der im Landingpages-Editor angezeigt wird, wenn sich der Wert an der Position &quot;EIN&quot;befindet. &quot;ON&quot;, falls nicht angegeben.

Grundlegendes Beispiel:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable"></pre>`

Beispiel mit allen Attributen:

Dieses Beispiel zeigt einen häufigen Anwendungsfall, bei dem eine boolesche Variable die Sichtbarkeit eines CSS-Elements steuert, indem der Wert der css-Anzeigeeigenschaft auf &quot;block&quot;oder &quot;none&quot;eingestellt wird, um ein Element mit CSS ein-/auszublenden. Der Landingpages-Editor verwendet den Anzeigenamen &quot;Anzeigen/Ausblenden&quot;anstelle von &quot;AUS/EIN&quot;.

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style></pre>`

>[!NOTE]
>
>Programm-Token (my.token) können auch überall in Guided- oder Free-Form-Landingpages verwendet werden.
