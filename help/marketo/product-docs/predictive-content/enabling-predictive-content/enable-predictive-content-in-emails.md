---
unique-page-id: 11385020
description: Predictive Inhalte in E-Mails aktivieren - Marketing-Dokumente - Produktdokumentation
title: Predictive Inhalte in E-Mails aktivieren
translation-type: tm+mt
source-git-commit: 3c24395e55c756184615941327e15e050fa7d0ac
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# Predictive Inhalte in E-Mails aktivieren {#enable-predictive-content-in-emails}

Machen Sie ein oder mehrere Bilder in Ihrer E-Mail prädiktiv und passen Sie das Erlebnis für jeden Empfänger an.

>[!NOTE]
>
>Es wird empfohlen, mehr als fünf Inhaltselemente pro Kategorie und Quelle (E-Mail, Rich Media, Bar) zu aktivieren, bevor Sie Predictive Content testen und verwenden. Mehr Inhalte geben Ihnen ein besseres Vorhersageergebnis.

>[!PREREQUISITES]
>
>Vor der Aktivierung von Predictive Content. Sie müssen:
>
>* [Vorbereitung von prädiktiven Inhalten](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md)
>* [Genehmigen eines Titels für prädiktive Inhalte](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## Hinzufügen von prädiktiven Inhalten mit dem E-Mail 2.0-Editor {#adding-predictive-content-using-the-email-editor}

1. Klicken Sie auf **Marketing-Aktivitäten**.

   ![](assets/one.png)

1. Wählen Sie Ihre E-Mail aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/two.png)

1. Klicken Sie auf das Bild, das prädiktiv sein soll. Wenn das Zahnradsymbol angezeigt wird, klicken Sie darauf und wählen Sie **Inhalt aktivieren`AI`** aus (Inhalt`AI` ist der frühere Name für Predictive Content).

   ![](assets/three.png)

1. Um eine oder mehrere Kategorien auszuwählen, klicken Sie auf die Dropdownliste **Kategorien**, wählen Sie die gewünschten aus und klicken Sie auf **Übernehmen**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Die Auswahl bestimmter Kategorien oder das Ändern des prädiktiven Layouts ist optional.

1. Ihr Bild ist jetzt prädiktiv. Wiederholen Sie die Schritte 3 und 4 für weitere Bilder (falls gewünscht).

   ![](assets/five.png)

1. Klicken Sie zur Vorschau Ihrer E-Mail in der rechten oberen Ecke auf **Vorschau**.

   ![](assets/six.png)

1. Klicken Sie auf **Aktualisieren**, um verschiedene Ansichten zu erstellen.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Das Bild wird erst ausgewählt, wenn der Empfänger die E-Mail-Adresse **_öffnet._** Was Sie also in der Vorschau sehen, ist nur ein Beispiel und wird nicht unbedingt das Bild sein, das der Empfänger sieht.

1. Nachdem Sie die Vorschau Ihrer E-Mail abgeschlossen haben, klicken Sie auf die Dropdownliste **Vorschau Aktionen** und wählen Sie **Genehmigen und Schließen**. Wenn Sie noch Bearbeitungen vornehmen müssen, klicken Sie auf der rechten Seite auf **Entwurf bearbeiten**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Beim Senden eines Beispiels wird ein zufälliges Bild ausgewählt.

Nachdem Sie Ihre E-Mail genehmigt haben, wird sie mit Predictive Content ausgestattet und bereit zum Versenden!

>[!CAUTION]
>
>Sobald ein Empfänger die E-Mail öffnet, werden die Prognosebilder gesperrt. Wenn der Inhalt später entfernt wird, sehen Empfänger ein beschädigtes Bild, in dem der Inhalt enthalten war.

## Hinzufügen von prädiktiven Inhalten, wenn der Editor &quot;E-Mail 2.0&quot;nicht verwendet wird{#adding-predictive-content-when-not-using-the-email-editor}

Wenn Sie keine [E-Mail 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md)-Vorlage verwenden, können Sie Ihrer E-Mail Predictive Content hinzufügen, indem Sie ein Bild in Ihrer Vorlage einfach als Markieren zu bearbeitbares Bildelement markieren.

Erfahren Sie mehr über die [Marketo-spezifische Syntax hier](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md#elements).

Im Folgenden finden Sie ein Beispiel dafür, wie der Code aussehen sollte (dies ist nur ein Beispiel, kopieren Sie den Code unten nicht genau).

**Beispiel**

```example
<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="http://www.marketo.com">  
<a><img style="border:10px solid red;"></a>  
</div>
```
