---
solution: Marketo Engage
product: marketo
title: Anpassbare Fragmente
description: Erfahren Sie, wie Sie Fragmente anpassen, indem Sie einige der zugehörigen Felder als bearbeitbar festlegen.
level: Beginner, Intermediate
feature: Email Designer
role: User
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
source-git-commit: cc6c04ca8a72f6efb0bec93cba084fe2993f53f0
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 64%

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
<!--
## Add editable fields in HTML components and expression fragments {#expression}

To make portions of an HTML component or an expression fragment editable, you must use a specific syntax in the expression editor. This involves declaring a _variable_ with a default value that users can override after adding the fragment to their content.

For example, suppose you want to create a fragment to add to your emails, and allow users to customize a specific color used in different locations, such as frames or buttons' background colors. When creating your fragment, you need to declare a variable with a _unique ID_ (e.g., "color"), and call it at the desired locations in the fragment content where you want to apply this color. When adding the fragment to their content, users will be able to customize the color used wherever the variable is referenced.

For HTML components, only specific elements can become editable fields. Expand the section below for more information.

+++Editable elements in HTML components:

The elements below can become editable fields in an HTML component:

* A portion of text
* A full URL for link or image (doesn't work with portion of a URL)
* Entire CSS property (doesn't work with partial property)

For example, in the code below, each element highlighted in red can become a property:

![](assets/fragment-html.png){width="500" zoomable="yes"}

+++
-->
>[!MORELIKETHIS]
>
>[Fragmente](/help/marketo/product-docs/email-marketing/email-designer/fragments.md){target="_blank"}
