---
unique-page-id: 2953419
description: Verwenden des Rich Text Editor - Marketing Docs - Produktdokumentation
title: Verwenden des Rich-Text-Editors
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 0%

---


# Verwenden des Rich-Text-Editors {#using-the-rich-text-editor}

Der Rich-Text-Editor (RTE) wird überall in Marketing angezeigt und steht jederzeit zur Verfügung, wenn Sie Inhalte hinzufügen oder bearbeiten möchten. Sie sehen eine Version davon auf Landingpages, Programmen, E-Mails, Formularen und Snippets. Klicken Sie einfach auf **Entwurf bearbeiten** und es erscheint ein Popup, um Ihnen zu helfen.

## Editoreinstellungen {#editor-settings}

Die Einstellung für das Stammblock-Element definiert, welche Tags Ihren Inhalt umschließen. Standardmäßig verwendet das Element E-Mail-Stammblock <p> Tags. Sie haben die Möglichkeit, dies zu ändern, indem Sie die folgenden Schritte ausführen.

>[!TIP]
>
>Sie haben zwar die Möglichkeit, Ihr Stammblock-Element auszuwählen, es wird jedoch empfohlen, die Standardeinstellungen für eine optimale Benutzererfahrung zu verwenden.

1. Klicken Sie auf **Admin**.

   ![](assets/one.png)

1. Klicken Sie auf **E-Mail**.

   ![](assets/two.png)

1. Klicken Sie auf **Texteditoreinstellungen bearbeiten**.

   ![](assets/three.png)

1. Wählen Sie in der Dropdownliste **E-Mail/Snippet-Editor** die Option <div> oder Keine und klicken Sie auf **Speichern**. <div> in diesem Beispiel verwendet.

   ![](assets/four.png)

   Wenn Sie <div class="&ldquo;mktEditable&rdquo;"></div> in einer E-Mail-Vorlage sehen Sie das folgende Verhalten der HTML-Quelle, wenn Sie den Abschnitt öffnen und im Editor &quot;Text geht hierher&quot; eingeben:

<table> 
 <tbody> 
  <tr> 
   <th>&lt;p&gt;</th> 
   <th>&lt;div&gt;</th> 
   <th>Keines</th> 
  </tr> 
  <tr> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>&lt;p&gt;Text kommt hier&lt;/p&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>&lt;div&gt;Text kommt hier&lt;/div&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>Text kommt hier<br>&lt;/div&gt;</p></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Sie können auch das Stammblock-Element des Landingpage-Editors ändern, indem Sie die gleichen Schritte ausführen, aber in Schritt 4 auf die Dropdownliste **Landingpage-Editor** statt E-Mail/Snippet-Editor klicken.

>[!NOTE]
>
>Das Stammblock-Element ist immer <p> für Rich-Text-Programm-Token.

## Funktionen {#features}

Hier finden Sie die Funktionen, die Sie in einer RTE finden.

| Symbol | Name | Funktionsweise |
|---|---|---|
| ![—](assets/image2015-7-9-10-3a23-3a24.png) | Schriftfamilie | Wählen Sie Ihren Stil - wir haben jede Menge! |
| ![—](assets/image2015-7-9-10-3a22-3a11.png) | Schriftgröße | Wie groß willst du es? 25 Auswahlmöglichkeiten, von 8 px bis 90 px. |
| ![—](assets/image2015-7-9-10-3a59-3a4.png) | Stile | Wählen Sie &quot;Absatz&quot;oder &quot;sechs Überschriftenstile&quot;(für Landingpages). |
| ![—](assets/image2015-7-9-10-3a20-3a1.png) | Zeilenabstand | Nimm deinen Abstand zwischen den Zeilen. |
| ![—](assets/image2015-7-9-10-3a25-3a52.png) | Textfarbe | Schwarz, Rot oder was immer Sie wollen. |
| ![—](assets/image2015-7-9-10-3a24-3a38.png) | Hintergrundfarbe | Hervorhebung. |
| ![—](assets/image2015-7-9-10-3a28-3a4.png) | Fett | **Dunkler und dicker**. |
| ![—](assets/image2015-7-9-10-3a29-3a1.png) | Kursiv | *Gezinkt, für Hervorhebung oder* Zitate. |
| ![—](assets/image2015-7-9-10-3a30-3a56.png) | Unterstreichen | Legt eine Zeile unter den Text. |
| ![—](assets/image2015-7-9-10-3a31-3a57.png) | Ausrichtung | Verwenden Sie dieses Dropdownmenü, um Ihren Text und Ihre Bilder zu gestalten. Zentrieren Sie sie, wählen Sie die linke oder rechte Ausrichtung oder legen Sie mit voller Ausrichtung eine Kante an eine Kante fest. |  | ![—](assets/image2015-7-9-10-3a32-3a47.png) | Liste | Wählen Sie Aufzählungszeichen oder Zahlen aus der Dropdownliste. Aufzählungszeichen eignen sich gut für Listen und Zahlen mit Stufen. |
| ![—](assets/image2015-7-9-10-3a38-3a0.png) | Einzug | Wählen Sie mehr oder weniger Einzug. Verwenden Sie diese Option für Absätze oder Text, der hervorgehoben werden soll. |
| ![—](assets/image2015-7-9-10-3a38-3a58.png) | Link einfügen/bearbeiten | einen Link zu einer Website oder anderen Inhalten einfügen; einfach Änderungen daran vorzunehmen. |
| ![—](assets/image2015-7-9-10-3a39-3a42.png) | Bild einfügen/bearbeiten | Ein Bild sagt mehr als tausend Worte. Legen Sie eins ein. Klicken Sie auf das Kamerasymbol, um Ihr Design Studio zu durchsuchen. Sie können Bilder nebeneinander ablegen. |
| ![—](assets/image2015-7-9-10-3a40-3a36.png) | Token einfügen | Ein leistungsstarkes Tool, ideal für die Personalisierung von E-Mails und die Datenverfolgung. Achten Sie darauf, einen Standardwert einzugeben. |
| ![—](assets/image2015-7-9-10-3a41-3a21.png) | Rückgängig | Ups! Lass uns einen Schritt zurückgehen und es noch einmal versuchen. |
| ![—](assets/image2015-7-9-10-3a42-3a13.png) | Wiederholen | Wenn es wirklich in Ordnung ist, so wie es ist, kehren Sie zum Original zurück. |
| ![—](assets/image2015-7-9-10-3a43-3a29.png) | Verzeichnis | Baue deine eigene, so wie diese. Über ein Dropdown-Menü können Sie es konfigurieren. |
| ![—](assets/image2015-7-9-10-3a45-3a1.png) | Anker einfügen | Legen Sie Anker ab! |
| ![—](assets/image2015-7-9-10-3a45-3a48.png) | Horizontale Linie | Viele Verwendungen - Ideal zum Teilen von Abschnitten. |
| ![—](assets/image2015-10-6-12-3a12-3a17.png) | HTML bearbeiten | Blendet den HTML-Quelleditor ein, damit Sie Ihren Code anpassen können. |
| ![—](assets/image2015-7-9-10-3a47-3a36.png) | Tiefgestellt | Hängende Buchstaben (wie in O`<sub>2</sub>`). |
| ![—](assets/image2015-7-9-10-3a48-3a35.png) | Hochgestellt | Du hast die Macht! (2`<sup>6</sup>`). |
| ![—](assets/image2015-7-9-10-3a49-3a31.png) | Durchstreichen | `<s>Put a line through text, like this</s>`. |
| ![—](assets/image2015-7-9-10-3a50-3a11.png) | Sonderzeichen | Willst du über Euro reden? Mathe? Sie haben 243 Auswahlmöglichkeiten. |
| ![—](assets/image2015-7-9-10-3a52-3a26.png) | Suchen und Ersetzen | Suchen und ändern Sie Dinge viel schneller, als nach jeder Instanz selbst zu suchen. |
| ![—](assets/image2015-7-9-10-3a53-3a37.png) | Formatierung löschen | Bringen Sie Dinge wieder in den Standard. |
| ![—](assets/image2015-7-9-10-3a55-3a2.png) | Abbrechen | Drücken Sie die Taste, um zu sagen: &quot;Macht nichts.&quot; |
| ![—](assets/image2015-7-9-10-3a56-3a2.png) | Speichern | Drücken Sie die Taste, um zu sagen: &quot;OK, ich mag es.&quot; |

>[!TIP]
>
>Sie bearbeiten HTML und Text auf separaten Bildschirmen. Klicken Sie auf der Registerkarte **Text** aus HTML **kopieren und** Speichern **, damit Ihr Text mit Ihrem HTML übereinstimmt.**

>[!NOTE]
>
>Sie sind nicht auf die Schriftarten in der Dropdown-Liste beschränkt. Sie können eine nicht aufgeführte verwenden, indem Sie auf den HTML-Code zugreifen. Alle Webschriftarten werden in Marketo unterstützt, aber Webschriftarten funktionieren nicht in allen E-Mail-Clients.

## Landingpages {#landing-pages}

Die Einstellung für das Stammblock-Element definiert, welche Tags Ihren Inhalt umschließen. Standardmäßig verwendet das Stammblock-Element der Landingpage <div> Tags. Sie haben die Möglichkeit, dies zu ändern, indem Sie die folgenden Schritte ausführen.

>[!TIP]
>
>Sie haben zwar die Möglichkeit, Ihr Stammblock-Element auszuwählen, es wird jedoch empfohlen, die Standardeinstellungen für eine optimale Benutzererfahrung zu verwenden.

1. Klicken Sie auf **Admin**.

   ![](assets/one.png)

1. Klicken Sie auf **E-Mail**.

   ![](assets/two.png)

1. Klicken Sie auf **Texteditoreinstellungen bearbeiten**.

   ![](assets/three.png)

1. Wählen Sie in der Dropdownliste **Landingpage-Editor** die Option <p> oder Keine und klicken Sie auf **Speichern**. <p> in diesem Beispiel verwendet.

   ![](assets/five.png)

   Und das ist es!

