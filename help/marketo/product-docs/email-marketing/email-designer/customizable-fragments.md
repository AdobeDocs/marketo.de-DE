---
solution: Marketo Engage
product: marketo
title: Anpassbare Fragmente
description: Erfahren Sie, wie Sie Fragmente anpassen, indem Sie einige der zugehörigen Felder als bearbeitbar festlegen.
level: Beginner, Intermediate
feature: Email Designer
role: User
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 71%

---

# Anpassbare Fragmente {#customizable-fragments}

Wenn Fragmente in einer E-Mail oder E-Mail-Vorlage verwendet werden, sind sie aufgrund der Vererbung standardmäßig gesperrt. Das bedeutet, dass alle an einem Fragment vorgenommenen Änderungen automatisch an alle Assets weitergegeben werden, in denen das Fragment verwendet wird. Mit anpassbaren Fragmenten können bestimmte Felder innerhalb eines Fragments als bearbeitbar definiert werden, wenn das Fragment zu einer E-Mail oder E-Mail-Vorlage hinzugefügt wird. Angenommen, Sie verfügen über ein Fragment mit einem Banner, etwas Text und einer Schaltfläche. Sie können bestimmte Felder wie das Bild oder die Ziel-URL der Schaltfläche als bearbeitbar festlegen. Auf diese Weise können Benutzer diese Elemente ändern, wenn sie das Fragment in ihre E-Mail-/E-Mail-Vorlage integrieren, und so ein maßgeschneidertes Erlebnis schaffen, ohne das ursprüngliche Fragment zu beeinflussen.

Durch die Nutzung anpassbarer Fragmente können Sie Ihre Inhalte effizient verwalten und personalisieren, ohne völlig neue Inhaltsbausteine erstellen oder die Vererbung vom ursprünglichen Fragment unterbrechen zu müssen. Dadurch wird sichergestellt, dass Änderungen, die auf Fragmentebene vorgenommen werden, weiterhin weitergegeben werden. Gleichzeitig wird die erforderliche Anpassung auf E-Mail-/E-Mail-Vorlagenebene ermöglicht.

Sowohl visuelle Fragmente als auch Ausdrucksfragmente können als anpassbar markiert werden. Detaillierte Anweisungen zum weiteren Vorgehen mit den einzelnen Fragmenttypen finden Sie in den folgenden Abschnitten.

## Hinzufügen bearbeitbarer Felder in visuellen Fragmenten {#visual}

Gehen Sie wie folgt vor, um Teile eines visuellen Fragments als bearbeitbar festzulegen:

>[!NOTE]
>
>Bearbeitbare Felder können zu **Bild**-, **Text**- und **Schaltflächenkomponenten** hinzugefügt werden. Für **HTML**-Komponenten werden bearbeitbare Felder ähnlich wie Ausdrucksfragmente mithilfe des Personalisierungseditors hinzugefügt. [Informationen dazu, wie Sie bearbeitbare Felder in HTML-Komponenten und Ausdrucksfragmenten hinzufügen](#expression)

1. Öffnen Sie den Bildschirm zur Inhaltsbearbeitung von Fragmenten.

1. Wählen Sie die Komponente in Ihrem Fragment aus, für die Sie bearbeitbare Felder konfigurieren möchten.

1. Der Bereich „Komponenteneigenschaften“ wird auf der rechten Seite geöffnet. Wählen Sie die Registerkarte **[!UICONTROL Bearbeitbare Felder]** aus und aktivieren Sie die Option **[!UICONTROL Bearbeitung aktivieren]**.

1. Alle Felder, die für die ausgewählte Komponente bearbeitet werden können, werden im Bereich aufgelistet. Welche Felder zur Bearbeitung verfügbar sind, hängt vom ausgewählten Komponententyp ab.

   Im folgenden Beispiel wird es ermöglicht, die URL der Schaltfläche „Hier klicken“ zu bearbeiten.

   ![](assets/fragment-param-enable.png){width="800" zoomable="yes"}

1. Klicken Sie **[!UICONTROL Übersicht]**, um alle bearbeitbaren Felder und ihre Standardwerte zu überprüfen.

   In diesem Beispiel wird das Feld für die Schaltflächen-URL mit dem in der Komponente definierten Standardwert angezeigt. Dieser Wert kann von Benutzenden angepasst werden, nachdem sie das Fragment zu ihrem Inhalt hinzugefügt haben.

   ![](assets/fragment-param-preview.png){width="800" zoomable="yes"}

1. Speichern Sie abschließend Ihre Änderungen.

Nachdem Sie das Fragment zu einer E-Mail hinzugefügt haben, können Benutzer alle bearbeitbaren Felder anpassen, die im Fragment konfiguriert sind.

## Hinzufügen bearbeitbarer Felder in HTML-Komponenten und Ausdrucksfragmenten {#expression}

Damit Teile einer HTML-Komponente oder eines Ausdrucksfragments bearbeitbar sind, müssen Sie im Ausdruckseditor eine bestimmte Syntax verwenden. Dazu gehört die Deklarierung einer _Variablen_ mit einem Standardwert, den Benutzende überschreiben können, nachdem sie das Fragment zu ihrem Inhalt hinzugefügt haben.

Angenommen, Sie möchten zum einen ein Fragment erstellen, das Ihren E-Mails hinzugefügt werden soll, und zum anderen den Benutzenden ermöglichen, eine bestimmte Farbe anzupassen, die an verschiedenen Stellen verwendet wird, z. B. die Hintergrundfarbe von Rahmen oder Schaltflächen. Beim Erstellen Ihres Fragments müssen Sie eine Variable mit einer _eindeutigen ID_ (z. B. „color„) deklarieren und sie an den gewünschten Stellen im Fragmentinhalt aufrufen, an denen Sie diese Farbe anwenden möchten. Beim Hinzufügen des Fragments zum Inhalt können Benutzende die Farbe anpassen, die dann überall dort verwendet wird, wo auf die Variable verwiesen wird.

Im Falle von HTML-Komponenten können nur bestimmte Elemente zu bearbeitbaren Feldern gemacht werden. Erweitern Sie den folgenden Abschnitt, um weitere Informationen zu erhalten:

+++Bearbeitbare Elemente in HTML-Komponenten:

Die folgenden Elemente können in einer HTML-Komponente zu bearbeitbaren Feldern gemacht werden:

* Textteile
* Eine vollständige URL für Links oder Bilder (funktioniert nicht mit einer Teil-URL)
* Eine vollständige CSS-Eigenschaft (funktioniert nicht mit einer Teileigenschaft)

Im folgenden Code kann beispielsweise jedes rot hervorgehobene Element zu einer Eigenschaft gemacht werden:

![](assets/fragment-html.png){width="500" zoomable="yes"}

+++

>[!MORELIKETHIS]
>
>[Fragmente](/help/marketo/product-docs/email-marketing/email-designer/fragments.md){target="_blank"}
