---
unique-page-id: 11385020
description: Aktivieren prädiktiver Inhalte in E-Mails - Marketo-Dokumente - Produktdokumentation
title: Aktivieren prädiktiver Inhalte in E-Mails
exl-id: 7eaefee1-23e8-47ee-afff-adcf49096aa7
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Aktivieren prädiktiver Inhalte in E-Mails {#enable-predictive-content-in-emails}

Erstellen Sie ein oder mehrere Bilder in Ihrer E-Mail-Prognose und passen Sie das Erlebnis für jeden Empfänger an.

>[!NOTE]
>
>Es wird empfohlen, mehr als fünf Inhaltselemente pro Kategorie und Quelle (E-Mail, Rich-Media, Balken) zu aktivieren, bevor Predictive Content getestet und verwendet wird. Mehr Inhalte geben Ihnen ein besseres Prognoseergebnis.

>[!PREREQUISITES]
>
>Vor der Aktivierung des prädiktiven Inhalts müssen Sie:
>
>* **Predictive Content vorbereiten**
>
>   * [Predictive Content für E-Mails bearbeiten](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target="_blank"} oder
>   * [Predictive Content für Rich Media bearbeiten](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target="_blank"} oder
>   * [Prädiktive Inhalte für die Empfehlungsleiste bearbeiten](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target="_blank"}
>
>* [Genehmigen eines Titels für prädiktive Inhalte](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target="_blank"}

## Hinzufügen prädiktiver Inhalte mit dem Email 2.0 Editor {#adding-predictive-content-using-the-email-editor}

1. Klicks **Marketingaktivitäten**.

   ![](assets/one.png)

1. E-Mail auswählen und auf **Entwurf bearbeiten**.

   ![](assets/two.png)

1. Klicken Sie auf das Bild, das Sie prädiktiv machen möchten. Wenn das Zahnradsymbol angezeigt wird, klicken Sie darauf und wählen Sie **ContentAI aktivieren** (ContentAI ist der frühere Name für Predictive Content).

   ![](assets/three.png)

1. Um eine oder mehrere Kategorien auszuwählen, klicken Sie auf die **Kategorien** Dropdown-Liste, Auswahl(n) und klicken Sie auf **Anwenden**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Die Auswahl bestimmter Kategorien oder die Änderung des prädiktiven Layouts ist optional.

1. Ihr Bild ist jetzt prädiktiv. Wiederholen Sie die Schritte 3 und 4 für weitere Bilder (falls gewünscht).

   ![](assets/five.png)

1. Um eine Vorschau Ihrer E-Mail anzuzeigen, klicken Sie auf **Vorschau** in der oberen rechten Ecke.

   ![](assets/six.png)

1. Um verschiedene mögliche Bilder anzuzeigen, klicken Sie auf **Aktualisieren**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Das Bild ist nicht ausgewählt **_bis der Empfänger die E-Mail öffnet_**. Was Sie also in der Vorschau sehen, ist nur ein Beispiel und wird nicht unbedingt das Bild sein, das der Empfänger sieht.

1. Nachdem Sie die Vorschau Ihrer E-Mail abgeschlossen haben, klicken Sie auf die Schaltfläche **Vorschau von Aktionen** und wählen Sie **Genehmigen und schließen**. Wenn Sie noch Bearbeitungen durchführen müssen, klicken Sie auf **Entwurf bearbeiten** rechts.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Beim Senden eines Beispiels wird ein zufälliges Bild ausgewählt.

Nachdem Sie Ihre E-Mail validiert haben, wird sie mit Predictive Content ausgestattet und versandbereit!

>[!CAUTION]
>
>Sobald ein Empfänger die E-Mail öffnet, werden die prädiktiven Bilder gesperrt. Wenn der Inhalt später entfernt wird, sehen die Empfänger ein defektes Bild, in dem sich der Inhalt befand.

## Hinzufügen prädiktiver Inhalte bei Nichtverwendung des E-Mail 2.0-Editors {#adding-predictive-content-when-not-using-the-email-editor}

Wenn Sie kein [Email 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md){target="_blank"} Vorlage können Sie Ihrer E-Mail Predictive Content hinzufügen, indem Sie einfach ein Bild in Ihrer Vorlage als bearbeitbares Marketo-Bildelement taggen.

Informationen zum [Marketo-spezifische Syntax hier](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md#elements){target="_blank"}.

Im Folgenden finden Sie ein Beispiel dafür, wie der Code aussehen sollte (dies ist nur ein Beispiel, kopieren Sie den unten stehenden Code nicht genau).

**Beispiel**

```example
<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com">  
<a><img style="border:10px solid red;"></a>  
</div>
```
