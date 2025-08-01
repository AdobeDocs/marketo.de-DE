---
unique-page-id: 2953419
description: Verwenden des Rich-Text-Editors - Marketo-Dokumente - Produktdokumentation
title: Verwenden des Rich-Text-Editors
exl-id: 9b2d6d41-f947-4859-aad9-a10c15eb013a
feature: Email Editor
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 1%

---

# Verwenden des Rich-Text-Editors {#using-the-rich-text-editor}

Der Rich-Text-Editor (RTE) wird überall in Marketo angezeigt und ist immer verfügbar, wenn Sie Inhalte hinzufügen oder bearbeiten möchten. Eine Version davon wird auf Landingpages, Programmen, E-Mails, Formularen und Snippets angezeigt. Klicken Sie einfach **[!UICONTROL Entwurf bearbeiten]** und es wird angezeigt, um Ihnen zu helfen.

## Editor-Einstellungen {#editor-settings}

Die Einstellung „Stammblockelement“ definiert, welche Tags Ihren Inhalt umschließen. Standardmäßig verwendet das E-Mail-Stammblockelement `<p>` Tags. Sie haben die Möglichkeit, dies zu ändern, indem Sie die folgenden Schritte ausführen.

>[!TIP]
>
>Sie haben zwar die Möglichkeit, Ihr Stammblockelement auszuwählen, wir empfehlen jedoch immer die Verwendung von Standardeinstellungen, um das Benutzererlebnis zu verbessern.

1. Klicken Sie auf **[!UICONTROL Admin]**.

   ![](assets/one.png)

1. Klicken Sie auf **[!UICONTROL E-Mail]**.

   ![](assets/two.png)

1. Klicken Sie **[!UICONTROL Einstellungen für Texteditor bearbeiten]**.

   ![](assets/three.png)

1. Wählen Sie in der Dropdown **[!UICONTROL Dropdown]/[!UICONTROL Snippet-Editor]** die Option `<div>` oder [!UICONTROL Ohne] und klicken Sie auf **[!UICONTROL Speichern]**. `<div>` wird in diesem Beispiel verwendet.

   ![](assets/four.png)

   Wenn Sie in einer E-Mail-Vorlage `<div class=“mktEditable”></div>` haben, sehen Sie das folgende Verhalten von HTML Source, wenn Sie den Abschnitt öffnen und im Editor „Text geht hierhin“ eingeben:

<table>
 <tbody>
  <tr>
   <th>&lt;p&gt;</th>
   <th>&lt;div&gt;</th>
   <th>Keine</th>
  </tr>
  <tr>
   <td><p>&lt;div class=„mktEditable“&gt;<br>&lt;p&gt;Text hier&lt;/p&gt;<br>&lt;/div&gt;</p></td>
   <td><p>&lt;div class=„mktEditable“&gt;<br>&lt;div&gt;Text hier&lt;/div&gt;<br>&lt;/div&gt;</p></td>
   <td><p>&lt;div class=„mktEditable“&gt;<br>Text hier <br>&lt;/div&gt;</p></td>
  </tr>
 </tbody>
</table>

>[!TIP]
>
>Sie können auch das Stammblockelement des Landingpage-Editors ändern, indem Sie die gleichen Schritte ausführen, aber auf die Dropdown-Liste **[!UICONTROL Landingpage-Editor]** in Schritt 4 anstelle von [!UICONTROL E-Mail]/[!UICONTROL Snippet-Editor] klicken.

>[!NOTE]
>
>Das -Stammblockelement wird immer für Rich-Text-Programm-Token `<p>`.

## Funktionen {#features}

Im Folgenden finden Sie die Funktionen, die Sie in einem RTE finden.

| Symbol | Name | Funktion |
|---|---|---|
| ![—](assets/image2015-7-9-10-3a23-3a24.png) | [!UICONTROL Schriftfamilie] | Wählen Sie Ihren Stil - wir haben jede Menge! |
| ![—](assets/image2015-7-9-10-3a22-3a11.png) | [!UICONTROL Schriftgröße] | Wie groß wollen Sie es? 25 Wahlmöglichkeiten, von 8 bis 90 Pixel. |
| ![—](assets/image2015-7-9-10-3a59-3a4.png) | [!UICONTROL Stile] | Wählen Sie Absatz oder sechs Überschriftenstile (für Landingpages). |
| ![—](assets/image2015-7-9-10-3a20-3a1.png) | [!UICONTROL Zeilenabstand] | Pick deinen Abstand zwischen den Linien. |
| ![—](assets/image2015-7-9-10-3a25-3a52.png) | [!UICONTROL Textfarbe] | Schwarz, Rot oder was immer Sie wollen. |
| ![—](assets/image2015-7-9-10-3a24-3a38.png) | [!UICONTROL Hintergrundfarbe] | Zur Hervorhebung markieren. |
| ![—](assets/image2015-7-9-10-3a28-3a4.png) | [!UICONTROL Fett] | **Dunkler und dicker**. |
| ![—](assets/image2015-7-9-10-3a29-3a1.png) | [!UICONTROL Kursiv] | *Abgewinkelt, für Hervorhebung oder*. |
| ![—](assets/image2015-7-9-10-3a30-3a56.png) | [!UICONTROL Unterstreichen] | Setzt eine Zeile unter den Text. |
| ![—](assets/image2015-7-9-10-3a31-3a57.png) | [!UICONTROL Ausrichtung] | Verwenden Sie dieses Dropdown-Menü, um Ihren Text und Ihre Bilder anzuordnen. Zentrieren Sie sie, wählen Sie die linke oder rechte Ausrichtung aus oder verteilen Sie sie mit der vollständigen Ausrichtung von Kante zu Kante. |  | ![—](assets/image2015-7-9-10-3a32-3a47.png) | Liste | Wählen Sie Aufzählungszeichen oder Zahlen aus dem Dropdown-Menü aus. Aufzählungszeichen eignen sich gut für Listen und Zahlen mit Schritten. |
| ![—](assets/image2015-7-9-10-3a38-3a0.png) | [!UICONTROL Einzug] | Wählen Sie mehr oder weniger Einzug. Verwenden Sie für Absätze oder Text, den Sie hervorheben möchten. |
| ![—](assets/image2015-7-9-10-3a38-3a58.png) | [!UICONTROL Link einfügen/bearbeiten] | Fügen Sie einen Link zu einer Website oder anderen Inhalten ein. Nehmen Sie einfach Änderungen daran vor. |
| ![—](assets/image2015-7-9-10-3a39-3a42.png) | [!UICONTROL Bild einfügen/bearbeiten] | Ein Bild sagt mehr als tausend Worte. Komm rein. Klicken Sie auf das Kamerasymbol, um Ihr Design Studio zu durchsuchen. Sie können Bilder nebeneinander ablegen. |
| ![—](assets/image2015-7-9-10-3a40-3a36.png) | [!UICONTROL Token einfügen] | Ein leistungsstarkes Tool, ideal für E-Mail-Personalisierung und Daten-Tracking. Stellen Sie sicher, dass Sie einen Standardwert eingeben. |
| ![—](assets/image2015-7-9-10-3a41-3a21.png) | [!UICONTROL Rückgängig] | Entschuldigung! Gehen wir einen Schritt zurück und versuchen es erneut. |
| ![—](assets/image2015-7-9-10-3a42-3a13.png) | [!UICONTROL Wiederholen] | Wenn es wirklich in Ordnung ist, wie es ist, kehren Sie zum Original zurück. |
| ![—](assets/image2015-7-9-10-3a43-3a29.png) | [!UICONTROL Tabelle] | Eigene bauen, wie diese hier. Ein Dropdown-Menü ermöglicht die Konfiguration. |
| ![—](assets/image2015-7-9-10-3a45-3a1.png) | [!UICONTROL Anker einfügen] | Anker fallen lassen! |
| ![—](assets/image2015-7-9-10-3a45-3a48.png) | [!UICONTROL Horizontale Linie] | Viele Anwendungen - Ideal für Teilungsabschnitte. |
| ![—](assets/image2015-10-6-12-3a12-3a17.png) | [!UICONTROL HTML bearbeiten] | Öffnet den HTML Source Editor, damit Sie Ihren Code anpassen können. |
| ![—](assets/image2015-7-9-10-3a47-3a36.png) | [!UICONTROL Tiefgestellt] | Tief hängende Buchstaben (wie in O`<sub>2</sub>`). |
| ![—](assets/image2015-7-9-10-3a48-3a35.png) | [!UICONTROL Hochgestellt] | Du hast die Macht! (2`<sup>6</sup>`) |
| ![—](assets/image2015-7-9-10-3a49-3a31.png) | [!UICONTROL Durchgestrichen] | `<s>Put a line through text, like this</s>`. |
| ![—](assets/image2015-7-9-10-3a50-3a11.png) | [!UICONTROL Sonderzeichen] | Möchten Sie über Euros sprechen? Mathematik? Sie haben 243 Möglichkeiten. |
| ![—](assets/image2015-7-9-10-3a52-3a26.png) | [!UICONTROL Suchen und Ersetzen] | Suchen und ändern Sie Dinge viel schneller, als selbst nach jeder Instanz zu suchen. |
| ![—](assets/image2015-7-9-10-3a53-3a37.png) | [!UICONTROL Formatierung löschen] | Bringen Sie die Dinge zum Standard zurück. |
| ![—](assets/image2015-7-9-10-3a55-3a2.png) | [!UICONTROL Abbrechen] | Drücke den Knopf, um zu sagen: „Macht nichts.“ |
| ![—](assets/image2015-7-9-10-3a56-3a2.png) | [!UICONTROL Speichern] | Drücken Sie den Knopf um zu sagen, „OK, ich mag es.“ |

>[!TIP]
>
>Sie bearbeiten Ihre HTML und den Text auf separaten Bildschirmen. HTML Klicken Sie auf der Registerkarte **[!UICONTROL Text]** auf **[!UICONTROL Text]** und dann auf **[!UICONTROL Speichern]**, damit der Text Ihrer HTML entspricht.

>[!NOTE]
>
>Sie sind nicht auf die Schriftarten in der Dropdown-Liste beschränkt. Sie können eine nicht aufgeführte verwenden, indem Sie auf den HTML-Code zugreifen. Alle Web-Schriftarten werden in Marketo unterstützt, aber Web-Schriftarten funktionieren nicht universell in allen E-Mail-Clients.

## Landingpages {#landing-pages}

Die Einstellung „Stammblockelement“ definiert, welche Tags Ihren Inhalt umschließen. Standardmäßig verwendet das Stammblockelement der Landingpage `<div>` Tags. Sie haben die Möglichkeit, dies zu ändern, indem Sie die folgenden Schritte ausführen.

>[!TIP]
>
>Sie haben zwar die Möglichkeit, Ihr Stammblockelement auszuwählen, wir empfehlen jedoch immer die Verwendung von Standardeinstellungen, um das Benutzererlebnis zu verbessern.

1. Klicken Sie auf **[!UICONTROL Admin]**.

   ![](assets/one.png)

1. Klicken Sie auf **[!UICONTROL E-Mail]**.

   ![](assets/two.png)

1. Klicken Sie **[!UICONTROL Einstellungen für Texteditor bearbeiten]**.

   ![](assets/three.png)

1. Wählen Sie **[!UICONTROL Dropdown-Menü]** Landingpage-Editor“ `<p>` oder [!UICONTROL Keine] aus und klicken Sie auf **[!UICONTROL Speichern]**. `<p>` wird in diesem Beispiel verwendet.

   ![](assets/five.png)

   Und das war&#39;s!
