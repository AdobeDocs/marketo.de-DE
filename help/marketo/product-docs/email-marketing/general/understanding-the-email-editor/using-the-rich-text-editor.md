---
unique-page-id: 2953419
description: Verwenden des Rich-Text-Editors - Marketo-Dokumente - Produktdokumentation
title: Rich-Text-Editor verwenden
exl-id: 9b2d6d41-f947-4859-aad9-a10c15eb013a
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 5%

---

# Rich-Text-Editor verwenden {#using-the-rich-text-editor}

Der Rich-Text-Editor (RTE) wird überall in Marketo angezeigt und ist verfügbar, wenn Sie Inhalte hinzufügen oder bearbeiten möchten. Sie sehen eine Version davon auf Landingpages, Programmen, E-Mails, Formularen und Snippets. Klicken Sie einfach auf **Entwurf bearbeiten**, und es wird angezeigt, um Sie zu bedienen.

## Editor-Einstellungen {#editor-settings}

Die Einstellung des Stammblock-Elements definiert, welche Tags Ihren Inhalt umschließen. Standardmäßig verwendet das Element des E-Mail-Stammblocks `<p>` -Tags. Sie können dies ändern, indem Sie die folgenden Schritte ausführen.

>[!TIP]
>
>Sie haben zwar die Möglichkeit, Ihr Stammblock-Element auszuwählen, doch empfehlen wir für ein bestes Benutzererlebnis immer die Verwendung von Standardeinstellungen.

1. Klicken Sie auf **Admin**.

   ![](assets/one.png)

1. Klicken Sie auf **E-Mail**.

   ![](assets/two.png)

1. Klicken Sie auf **Einstellungen für den Texteditor bearbeiten**.

   ![](assets/three.png)

1. Wählen Sie in der Dropdown-Liste **E-Mail-/Snippet-Editor** die Option `<div>` oder Keine aus und klicken Sie auf **Speichern**. In diesem Beispiel wird `<div>` verwendet.

   ![](assets/four.png)

   Wenn Sie `<div class=“mktEditable”></div>` in einer E-Mail-Vorlage haben, sehen Sie das folgende HTML Source-Verhalten, wenn Sie den Abschnitt öffnen und im Editor &quot;Text wird hier angezeigt&quot;eingeben:

<table> 
 <tbody> 
  <tr> 
   <th>&lt;p&gt;</th> 
   <th>&lt;div&gt;</th> 
   <th>Keine</th> 
  </tr> 
  <tr> 
   <td><p>&lt;div class="mktEditable"&gt;<br>&lt;p&gt;Text geht hierhin&lt;/p&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="mktEditable"&gt;<br>&lt;div&gt;Text wird hierhin verschoben&lt;/div&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="mktEditable"&gt;<br>Text wird hierhin verschoben<br>&lt;/div&gt;</p></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Sie können auch das Stammblock-Element des Landingpage-Editors ändern, indem Sie dieselben Schritte ausführen, aber in Schritt 4 auf die Dropdown-Liste **Landingpage-Editor** statt auf E-Mail-/Snippet-Editor klicken.

>[!NOTE]
>
>Das Stammblock-Element ist bei Rich-Text-Programm-Token immer `<p>`.

## Funktionen {#features}

Hier finden Sie die Funktionen, die Sie in einem RTE finden.

| Symbol | Name | Funktion |
|---|---|---|
| ![—](assets/image2015-7-9-10-3a23-3a24.png) | Schriftart | Wählen Sie Ihren Stil - wir haben jede Menge! |
| ![—](assets/image2015-7-9-10-3a22-3a11.png) | Schriftgroesse | Wie groß willst du es? 25 Auswahlmöglichkeiten, von 8 px bis 90 px. |
| ![—](assets/image2015-7-9-10-3a59-3a4.png) | Stil | Wählen Sie Absatz oder sechs Überschriftenstile (für Landingpages). |
| ![—](assets/image2015-7-9-10-3a20-3a1.png) | Zeilenabstand | Pick deinen Abstand zwischen den Zeilen. |
| ![—](assets/image2015-7-9-10-3a25-3a52.png) | Textfarbe | Schwarz, Rot oder was immer Sie wollen. |
| ![—](assets/image2015-7-9-10-3a24-3a38.png) | Hintergrundfarbe | Hervorhebung der Hervorhebung. |
| ![—](assets/image2015-7-9-10-3a28-3a4.png) | Fett | **dunkler und dicker**. |
| ![—](assets/image2015-7-9-10-3a29-3a1.png) | Kursiv | *Vergeltet, für Hervorhebung oder Zitat* s. |
| ![—](assets/image2015-7-9-10-3a30-3a56.png) | Unterstreichen | Legt eine Zeile unter den Text. |
| ![—](assets/image2015-7-9-10-3a31-3a57.png) | Ausrichtung | Verwenden Sie dieses Dropdown-Menü, um Ihren Text und Ihre Bilder darzustellen. Zentrieren Sie sie, wählen Sie eine linke oder rechte Ausrichtung oder teilen Sie sie mit vollständiger Ausrichtung an den Rand. |  | ![—](assets/image2015-7-9-10-3a32-3a47.png) | Liste | Wählen Sie Aufzählungszeichen oder Zahlen aus der Dropdown-Liste aus. Aufzählungszeichen eignen sich gut für Listen und Zahlen mit Schritten. |
| ![—](assets/image2015-7-9-10-3a38-3a0.png) | Einrücken | Wählen Sie mehr oder weniger Einzug. Verwenden Sie für Absätze oder Text, den Sie hervorheben möchten. |
| ![—](assets/image2015-7-9-10-3a38-3a58.png) | Link einfügen/bearbeiten | Fügen Sie einen Link zu einer Website oder anderen Inhalten ein und nehmen Sie einfach Änderungen daran vor. |
| ![—](assets/image2015-7-9-10-3a39-3a42.png) | Bild einfügen/bearbeiten | Ein Bild sagt mehr als tausend Worte. Legen Sie eine ab. Klicken Sie auf das Kamerasymbol, um Ihr Design Studio zu durchsuchen. Sie können Bilder nebeneinander einfügen. |
| ![—](assets/image2015-7-9-10-3a40-3a36.png) | Token einfügen | Ein leistungsstarkes Tool, ideal für die Personalisierung von E-Mails und das Tracking von Daten. Geben Sie unbedingt einen Standardwert ein. |
| ![—](assets/image2015-7-9-10-3a41-3a21.png) | Rückgängig | Entschuldigung! Lass uns einen Schritt zurückgehen und es noch einmal versuchen. |
| ![—](assets/image2015-7-9-10-3a42-3a13.png) | Wiederholen | Wenn es wirklich in Ordnung ist, so wie es ist, kehren Sie zum Original zurück. |
| ![—](assets/image2015-7-9-10-3a43-3a29.png) | Tabelle | Erstellen Sie Ihre eigene, wie diese hier. Ein Dropdown-Menü ermöglicht die Konfiguration. |
| ![—](assets/image2015-7-9-10-3a45-3a1.png) | Anker einfügen | Drop anchor! |
| ![—](assets/image2015-7-9-10-3a45-3a48.png) | Horizontale Linie | Viele Verwendungen - Ideal für die Teilung von Abschnitten. |
| ![—](assets/image2015-10-6-12-3a12-3a17.png) | HTML bearbeiten | Öffnet den HTML Source Editor, damit Sie Ihren Code anpassen können. |
| ![—](assets/image2015-7-9-10-3a47-3a36.png) | Tiefgestellt | Kleinhängende Buchstaben (wie in O`<sub>2</sub>`). |
| ![—](assets/image2015-7-9-10-3a48-3a35.png) | Hochgestellt | Du hast die Macht! (2`<sup>6</sup>`). |
| ![—](assets/image2015-7-9-10-3a49-3a31.png) | Durchstreichen | `<s>Put a line through text, like this</s>`. |
| ![—](assets/image2015-7-9-10-3a50-3a11.png) | Sonderzeichen | Willst du über Euro reden? Mathematisch? Sie haben 243 Möglichkeiten. |
| ![—](assets/image2015-7-9-10-3a52-3a26.png) | Suchen und Ersetzen | Suchen und ändern Sie Dinge viel schneller als die Suche nach jeder Instanz selbst. |
| ![—](assets/image2015-7-9-10-3a53-3a37.png) | Formatierung löschen | Kehren Sie Dinge auf den Standard zurück. |
| ![—](assets/image2015-7-9-10-3a55-3a2.png) | Abbrechen | Drücken Sie den Knopf, um zu sagen: &quot;Macht nichts.&quot; |
| ![—](assets/image2015-7-9-10-3a56-3a2.png) | Speichern | Drücken Sie die Taste, um zu sagen: &quot;OK, ich mag es.&quot; |

>[!TIP]
>
>Sie bearbeiten HTML und Text auf separaten Bildschirmen. Stellen Sie sicher, dass Sie auf der Registerkarte **Text** auf **Von HTML kopieren und dann auf** Speichern **klicken, damit Ihr Text Ihrer HTML entspricht.**

>[!NOTE]
>
>Sie sind nicht auf die Schriftarten in der Dropdown-Liste beschränkt. Sie können eine nicht aufgeführte verwenden, indem Sie auf den HTML-Code zugreifen. Alle Webfonts werden in Marketo unterstützt, Webfonts funktionieren jedoch nicht in allen E-Mail-Clients allgemein.

## Landing Page {#landing-pages}

Die Einstellung des Stammblock-Elements definiert, welche Tags Ihren Inhalt umschließen. Standardmäßig verwendet das Stammblock-Element der Landingpage `<div>` -Tags. Sie können dies ändern, indem Sie die folgenden Schritte ausführen.

>[!TIP]
>
>Sie haben zwar die Möglichkeit, Ihr Stammblock-Element auszuwählen, doch empfehlen wir für ein bestes Benutzererlebnis immer die Verwendung von Standardeinstellungen.

1. Klicken Sie auf **Admin**.

   ![](assets/one.png)

1. Klicken Sie auf **E-Mail**.

   ![](assets/two.png)

1. Klicken Sie auf **Einstellungen für den Texteditor bearbeiten**.

   ![](assets/three.png)

1. Wählen Sie in der Dropdown-Liste **Landingpage-Editor** die Option `<p>` oder &quot;Keine&quot;aus und klicken Sie auf **Speichern**. In diesem Beispiel wird `<p>` verwendet.

   ![](assets/five.png)

   Und das ist es!
