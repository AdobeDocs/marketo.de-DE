---
title: Gestalten barrierefreier Inhalte
description: Erfahren Sie, wie Sie in Marketo Engage barrierefreie Inhalte für Ihre E-Mails entwerfen.
feature: Email Designer
role: User
level: Beginner, Intermediate
keywords: E-Mail, Design, Barrierefreiheit
source-git-commit: 753455b40ead039a56c595fa61ab9a95b7936382
workflow-type: tm+mt
source-wordcount: '1367'
ht-degree: 45%

---

# Gestalten barrierefreier Inhalte {#accessible-content}

Der [Europäische Rechtsakt zur Barrierefreiheit](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=CELEX:32019L0882){target="_blank"} ist eine Richtlinie, mit der der Binnenmarkt für barrierefreie Produkte und Dienstleistungen durch die Beseitigung von Hindernissen, die durch unterschiedliche nationale Vorschriften in den Mitgliedstaaten verursacht werden, verbessert werden soll.

Diese Verordnung besagt, dass alle digitalen Kommunikationen, einschließlich E-Mails, Newsletter, PDFs und herunterladbare Inhalte, zugänglich sein sollten. Beim Erstellen von Inhalten für Ihre Empfängerinnen und Empfänger müssen Sie daher bestimmte Richtlinien befolgen, z. B. die Verwendung barrierefreier Schriftarten und lesbarer Formate und die Bereitstellung von Alternativtext für Bilder.

Mit Marketo Engage Email Designer können Sie diese Anweisung auf Grundlage der Web Content Accessibility Guidelines (WCAG) 2.1, Level AA, problemlos einhalten. Die Best Practices für die Erstellung barrierefreier Inhalte mit Marketo Engage sind unten aufgeführt.

>[!NOTE]
>
>Auf dieser Seite geht es darum, Ihre Inhalte für alle Empfängerinnen und Empfänger zugänglich zu machen, damit Menschen mit Behinderungen Ihre in Marketo Engage entworfenen E-Mails lesen, verstehen und mit ihnen interagieren können.

## Sicherstellen der Lesbarkeit von Text {#text-readability}

Verwenden Sie die Registerkarte **[!UICONTROL Stile]** der Komponente **[!UICONTROL Text]**, um sicherzustellen, dass Ihr Text lesbar ist, z. B. mit einem ordnungsgemäßen Farbkontrast und einfachen Schriftarten.

<!--![](assets/accessible-text-styles.png){width="80%"}-->

Befolgen Sie bei Schriftarten und Text die folgenden Richtlinien:

**Schriftartenauswahl**

* Verwenden Sie serifenlose Schriftarten wie Arial, Verdana, Tahoma, Helvetica oder Open Sans.
* Vermeiden Sie serifenlose, kursive oder dekorative Schriftarten in Textinhalten.
* Achten Sie auf einen eingeschränkten Schriftsatz, um Konsistenz und Fallback zu gewährleisten (z. B.: `font-family: Arial, Helvetica, sans-serif;`).

**Schriftgrad**

* Achten Sie beim Textkörper auf einen Schriftgrad von mindestens 16 Pixel.
* Verwenden Sie eine angemessene Hierarchie für Überschriften.

**Farbkontrast**

* Wahren Sie zwischen Text und Hintergrund ein Kontrastverhältnis von mindestens 4,5 :1.
* Achten Sie bei großem Text (≥24 Pixel oder fett 18 Pixel) auf einen Kontrast von mindestens 3 :1.
* Vermeiden Sie hellgrauen oder pastellfarbenen Text auf weißem Hintergrund.
* Verlassen Sie sich nicht allein auf Farbe, um Bedeutung zu vermitteln. Verwenden von Unterstrichen, Symbolen usw.

**Barrierefreiheit von Text**

* Vermeiden Sie Text in Bildern.
* Verwenden Sie im Textkörper nicht ausschließlich Großbuchstaben.
* Stellen Sie sicher, dass Text auf bis zu 200 % gezoomt werden kann, ohne dass das Layout beschädigt wird.

## Sicherstellen der visuellen Barrierefreiheit {#visual-accessibility}

* Verwenden Sie für wichtige Informationen keine reinen Farbindikatoren.
* Verwenden Sie Textbeschriftungen oder Symbole für mehr Klarheit.
* Optimieren Sie Ihr Design für mobile und responsive Layouts und stellen Sie sicher, dass Schaltflächen groß sind und ausreichend Abstand aufweisen.
* Testen Sie regelmäßig für verschiedene Geräte und Bildschirmgrößen, um die Barrierefreiheit zu gewährleisten.

In Marketo Engage können Größe und Abstand der verschiedenen Elemente in Ihrem Inhalt mithilfe der Stilparameter und -attribute im Bereich E-Mail-Designer (Stile **[!UICONTROL weiter]** werden.

Sie können beispielsweise den Hintergrund aktualisieren oder die Ränder, den Abstand und die Ausrichtung ändern, um die visuelle Barrierefreiheit zu verbessern.

<!--![](assets/accessible-styles.png){width="80%"}-->

Mit Marketo Engage Email Designer können Sie das Design für verschiedene Geräte und Bildschirmgrößen in der Vorschau anzeigen und optimieren. Sie können jederzeit **[!UICONTROL Zur Live-Ansicht wechseln]** um zu überprüfen, wie Ihre Inhalte auf verschiedenen Gerätegrößen gerendert werden können.

<!--![](assets/accessible-live-view.png){width="80%"}-->

>[!CAUTION]
>
>Die Live-Ansicht ist eine allgemeine Vorschau, die vergleicht, wie der Inhalt über verschiedene Gerätegrößen hinweg gerendert werden könnte. Das endgültige Rendering kann je nach E-Mail-Client der Empfängerinnen und Empfänger variieren.

## Verwenden von Alternativtext für Bilder {#alt-text}

Verwenden Sie die **[!UICONTROL Bild]**-Komponente, um alternativen Text für Bilder bereitzustellen.

<!--![](assets/accessible-alt-text.png){width="90%"}-->

* Beschreiben Sie den Zweck des Bildes kurz und kontextbezogen.
* Vermeiden Sie redundante Ausdrücke wie „Abbildung von …“ und verwenden Sie leeren Alternativtext für dekorative Bilder.
* Geben Sie für Symbole mit Bedeutung aussagekräftige Labels an. Nutzen Sie für komplexe Bilder einen kurzen Alternativtext und an anderer Stelle eine längere Beschreibung.

## Verwenden von lesbarem Format {#readable-format}

Verwenden Sie die für E-Mail-Designer relevanten Struktur- und Inhaltskomponenten sowie die Optionen im Bereich **[!UICONTROL Stile]**, um Ihre Inhalte klar, logisch und präzise zu organisieren, sodass sie für alle zugänglich sind.

<!--![](assets/accessible-components.png){width="100%"}-->

* Nutzen Sie strukturierte, semantische HTML mit passenden Überschriften, Absätzen, Listen und Tabellen.
* Stellen Sie sicher, dass der Inhalt einem logischen Fluss von links nach rechts, von oben nach unten folgt.
* Verwenden Sie klare, knappe Formulierungen.
* Stellen Sie alternative Formate für PDF-Dateien und Infografiken bereit.
* Ändern Sie die Textgröße und den Textfluss und stellen Sie sicher, dass die Typografie in allen Formaten mit angemessenem Farbkontrast lesbar ist.

## Sicherstellen der Lesbarkeit von Inhalten {#readability}

Um lesbar zu sein, müssen Ihre Inhalte klar, gut strukturiert und für alle verwendbar sein, auch für Menschen mit visuellen, kognitiven oder Leseschwächen und solche, die Hilfstechnologien verwenden. Einige Punkte, die Sie beim Erstellen barrierefreier Inhalte beachten sollten:

* Halten Sie Sätze mit bis zu 20 Wörtern.
* Bearbeiten Sie Ihre Kopie, um sie direkt und kurz zu halten.
* Nutzen Sie eine aktive Stimme, um die Satzstruktur einfacher zu halten.
* Vermeiden Sie Slang, Jargon oder regionale Wörter, mit denen einige Leute möglicherweise nicht vertraut sind.

Zur Einschätzung der Lesbarkeit Ihrer E-Mails können Sie den beliebten [Flesch Reading Ease Test](https://support.microsoft.com/de-de/office/abrufen-der-lesbarkeit-und-ebenenstatistiken-ihres-dokuments-85b4969e-e80a-4777-8dd3-f7fc3c8b3fd2){target="_blank"} nutzen, der in Microsoft Word zu finden ist. Er berechnet auf einer Skala von 0–100, wie leicht Ihre Inhalte zu lesen sind.

## Testen Ihrer Inhalte {#test}

Um die Barrierefreiheit Ihrer Inhalte zu überprüfen, können Sie die von Marketo Engage bereitgestellten Testfunktionen verwenden. Sie wurden nicht speziell dafür konzipiert zu überprüfen, ob Ihre Inhalte vollständig barrierefrei sind, können aber einen ersten Prüfungsschritt darstellen.

* Vorschau Ihres Inhalts mithilfe von Testprofilen.

* Verwenden Sie die Option [E-Mail-Rendering](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md){target="_blank"}, die Litmus zur Simulation Ihrer Designs in wichtigen E-Mail-Clients (Apple Mail, Gmail, Outlook) nutzt, damit Sie sehen können, ob Text, Farben und Bilder Ihre Inhalte barrierefrei machen. <!--Litmus includes accessibility testing-->

* Führen Sie Testsendungen durch, um das Rendering Ihres Inhalts zu testen, bevor Sie ihn an Ihre echte Zielgruppe senden.

<!--![](assets/accessible-simulate.png){width="90%"}-->

Um konsistenter zu überprüfen, ob Ihre Inhalte zuverlässig barrierefrei sind, nutzen Sie externe Tools wie:

* [WebAim Contrast Checker](https://webaim.org/resources/contrastchecker/){target="_blank"} und [WAVE Web Accessibility Evaluation Tool](https://wave.webaim.org/){target="_blank"} zur Bewertung von Kontrast und Compliance;

* Hilfstechnologien wie Bildschirmlesehilfen (z. B. [NVDA](https://www.nvaccess.org/download/){target="_blank"} oder [VoiceOver](https://support.apple.com/de-de/guide/iphone/iph3e2e415f/ios){target="_blank"} auf iPhone), um E-Mails aus der Perspektive sehbehinderter Benutzender zu erleben.

## Verwenden des dunklen Modus {#dark-mode}

[Dunkelmodus](/help/marketo/product-docs/email-marketing/email-designer/dark-mode.md){target="_blank"} Verbessert die visuelle Barrierefreiheit für Benutzer mit Lichtempfindlichkeit oder Sehbehinderungen, um das Seherlebnis zu verbessern.

<!--![](assets/accessible-dark-mode.png){width="90%"}-->

Zu den Best Practices für die Gestaltung von Inhalten im Dunkelmodus gehören:

* Verwenden transparenter PNGs oder SVGs
* Festlegen geeigneter Meta-Tags und CSS
* Bereitstellung von barrierefreiem Fallback-Styling, wenn der Dunkelmodus nicht unterstützt wird.

Stellen Sie sicher, dass Ihre E-Mails im Dunkelmodus korrekt gerendert werden, indem Sie alle E-Mail-Inhalte und Benutzeroberflächenelemente sowohl im Hellen als auch im Dunklen Modus testen.

## Verwenden spezifischer Attribute für Barrierefreiheit {#attributes}

### Sprachattribute {#language}

Fügen Sie beim Gestalten von Designs die Attribute `lang` (Sprache) und `dir` (Textausrichtung) in den Content-Hauptteil ein. Diese Attribute helfen Hilfstechnologien (wie Bildschirmlesehilfen), Ihre Inhalte angemessen zu interpretieren und darzustellen.

* Das Attribut `lang` gibt die Sprache der E-Mail für Hilfstechnologien an und stellt sicher, dass Wörter korrekt ausgesprochen werden.

  +++Beispiele

  Beispiel für Englisch:

  ```
  <body lang="en">
  ```

  Beispiel für Französisch:

  ```
  <body lang="fr">
  ```

  +++

* Das Attribut `dir` gibt die Textausrichtung an. Die meisten Sprachen, einschließlich Englisch und Französisch, werden von links nach rechts (ltr) gelesen, während Sprachen wie Arabisch und Hebräisch von rechts nach links (rtl) gelesen werden.

  +++Beispiele

  Beispiel für Englisch (links nach rechts):

  ```html
  <body lang="en" dir="ltr">
  ```

  Beispiel für Arabisch (rechts nach links):

  ```html
  <body lang="ar" dir="rtl">
  ```

  +++

Bildschirmlesehilfen verwenden das Attribut `lang`, um die korrekten Ausspracheregeln anzuwenden, während die Textausrichtung dafür sorgt, dass Inhalte in Sprachen, die von links nach rechts bzw. von rechts nach links fließen, richtig dargestellt werden. Ohne diese Attribute kann es zu einer verwirrenden Leserichtung oder falscher Aussprache kommen. Verpacken Sie den Textkörper Ihrer E-Mail immer mit den entsprechenden `lang`- und `dir`.

>[!TIP]
>
>Wenn Ihre E-Mail mehrere Sprachen enthält, weisen Sie bestimmten Abschnitten (z. B. `<table>` oder `<td>`) die entsprechenden Sprachattribute zu, um sicherzustellen, dass jeder Teil korrekt gelesen wird.

### Tabellen {#tables}

In HTML-Inhalten werden Tabellen häufig für das Layout verwendet. Standardmäßig behandeln Bildschirmlesehilfen jede `<table>` als Datentabelle und geben Zeilen, Spalten und Struktur aus. Dies kann verwirrend sein, wenn die Tabelle nur zur Formatierung dient.

Fügen Sie Layout-Tabellen `role="presentation"` (oder `role="none"`) hinzu, um sicherzustellen, dass Hilfstechnologien ihre Struktur überspringen und sich nur auf den tatsächlichen Inhalt konzentrieren.

+++Beispiel - Layouttabelle (mit `role="presentation"`)

```html
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="100%"> 
  <tr> 
    <td align="center"> 
      <h1>Hello World</h1> 
      <p>Welcome to our newsletter</p> 
    </td> 
  </tr> 
</table>
```

Die Bildschirmlesehilfen lesen:
„Hallo Welt. Willkommen zu unserem Newsletter.“ _(Zeilen, Spalten oder Tabellen werden nicht erwähnt)_

+++

+++Beispiel - Datentabelle (ohne `role="presentation"`)

```html
<table border="1" cellpadding="5" cellspacing="0">
  <tr>
    <th scope="col">Name</th>
    <th scope="col">Score</th>
  </tr>
  <tr> 
    <td>Peter</td>
    <td>19</td>
  </tr>
  <tr>
    <td>Parker</td>
    <td>62</td>
  </tr>
</table>
```

Die Bildschirmlesehilfen lesen:
„Tabelle mit 2 Spalten und 3 Zeilen.“

„Name, Peter. Bewertung, 19.“

„Name, Parker. Bewertung, 62.“

+++

>[!TIP]
>
>Verwenden Sie `role="presentation"` ausschließlich für Layout-Tabellen. Behalten Sie bei Datentabellen die semantische `<table>`-Struktur bei, damit Bildschirmlesehilfen Header und Beziehungen korrekt ausgeben können.

### Text für Links {#links}

Bildschirmlesehilfen lesen Links mit ihrem Text vor. Wenn ein Link nur mit „Hier klicken“ oder „Weitere Informationen“ beschriftet ist, kennen Benutzende von Hilfstechnologien das Ziel nicht. Für Barrierefreiheit benötigen sie beschreibenden Text, der das Ziel oder die Aktion klar angibt.

Verwenden Sie die E-Mail-Designer , um einen Link zu Ihrem Inhalt hinzuzufügen und die Kennzeichnung zu bearbeiten, damit sie erkennbar (sichtbar) und beschreibend (klar zu Ihrem Zweck) ist. Vermeiden Sie vage Labels wie „hier“ oder „mehr“.

<!--![](assets/accessible-link.png){width="70%"}-->

+++Beispiel - Guter Link (beschreibend): 

```
<p>Learn more in the  
<a href="https://adobe.com/release-notes">August release notes</a>. 
</p>
```

Die Bildschirmlesehilfen lesen:
„Link, Versionshinweise August.“

+++

+++Beispiel - Ungültiger Link (nicht beschreibend)

```
<p>Learn more about our new features.  
  <a href="https://adobe.com/release-notes">Click here</a>. 
</p>
```

Die Bildschirmlesehilfen lesen:
„Link, hier klicken.“ *(bietet keinen Kontext außerhalb der Lesereihenfolge)*

+++

<!--for Landing Pages-->

<!--## Provide keyboard navigation and focus support {#keyboard}

Providing keyboard navigation and focus support allows people who cannot use a mouse to fully access and interact with content. It also improves overall usability by giving all users a clear and consistent way to move through information.

* Focus via keyboard
    * Ensure all interactive elements (such as buttons, checkboxes, links) have `tabindex="0"` so they are included in the natural tab order. 
    * Allow navigation using the Tab and arrow keys (↑ ↓ ← →), which should visibly highlight the focused element. 
* Custom focus styling 
    * Apply clear and distinguishable styles for focusing on actionable elements: 
        +++Example (CSS)

        ```
        [tabindex="0"] : focus { 
        outline: 2px solid #00AEEF;  /* Cyan border */ 
        background-color: #20CEFF;   /* Optional background */ 
        }
        ```
        
        +++

    * Ensure that focus indicators meet the WCAG 2.2 focus appearance standards, including: 
        * Minimum area: 2 CSS pixel thick outline.
        * Contrast ratio: ≥ 3:1 between focused and unfocused state. 

* Keyboard activation support 
    * Ensure checkboxes and buttons respond to the Enter and Space keys. 
    * Validate the interaction using the keyboard alone: 
        * Enter or Space should toggle checkboxes.
        * Enter or Space should trigger the buttons.-->
