---
unique-page-id: 10095554
description: Einbetten eines Formulars in eine Webkampagne - Marketo Docs - Produktdokumentation
title: Einbetten eines Formulars in eine Webkampagne
exl-id: 41e60ae6-9a40-444f-8a55-47fc6ef6c5fb
feature: Web Personalization
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 1%

---

# Einbetten eines Formulars in eine Webkampagne {#embed-a-form-into-a-web-campaign}

Erfahren Sie, wie Sie ein Marketo-Formular in eine Webkampagne einbetten können (Dialogfeld, In Zone oder Widget).

1. Klicken Sie mit der rechten Maustaste auf ein bestätigtes Formular. Auswählen **Einbettungscode**.

   ![](assets/image2015-12-16-10-3a58-3a39.png)

1. Kopieren Sie den Code.

   ![](assets/image2015-12-16-11-3a16-3a24.png)

1. Gehen Sie in Web-Personalisierung zu **Web-Kampagnen**.

   ![](assets/web-campaigns-hand-7.jpg)

1. Klicks **Neue Kampagne erstellen**.

   ![](assets/create-new-web-campaign-hand-1.jpg)

1. Klicken Sie im Rich-Text-Editor auf das HTML-Symbol.

   ![](assets/five-1.png)

1. Fügen Sie den Einbettungscode des Formulars in den HTML Source Editor ein. Klicks **Aktualisieren**.

   ![](assets/six-1.png)

1. Das Formular wird nicht in der Editor-Ansicht angezeigt, Sie können es jedoch in der Vorschau anzeigen, um zu sehen, wie es in einer Kampagne dargestellt wird.

1. Klicks **Launch** , um die Kampagne zu starten.

   >[!NOTE]
   >
   >Alle Änderungen an den Formularfeldern müssen in den Marketingaktivitäten von Marketo unter &quot;Bearbeitungsentwurf des Formulars&quot;vorgenommen werden.

## Drei Methoden zum Hinzufügen eines Hintergrundbilds zu einem Formular {#three-ways-to-add-a-background-image-to-a-form}

Um ein Hintergrundbild zu Ihrem Formular hinzuzufügen, haben Sie folgende Möglichkeiten:

* CSS eines Formulardesigns bearbeiten
* Ändern der Dialogfeld- oder Widget-Farben in Set Campaign
* CSS-Code zum Skript hinzufügen

Informationen zum Bearbeiten der CSS eines Formulardesigns finden Sie unter [diesem Artikel](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md).

So ändern Sie die Dialogfeld- oder Widget-Farben in Set Campaign:

1. Wählen Sie im Rich-Text-Editor einen Dialogfeldkampagnentyp und einen Dialogfeldstil, eine Kopfzeilenfarbe und eine Hintergrundfarbe aus, um die Hintergrundfarben des Formulars anzupassen. Klicken Sie auf **Speichern**.

   ![](assets/image2015-12-29-18-3a28-3a31.png)

1. Hier ist ein Beispiel dafür, wie ein moderner Trim Dialog Style mit einer hellvioletten Kopfzeile und Hintergrundfarbe aussieht.

   ![](assets/image2015-12-29-18-3a27-3a31.png)

So fügen Sie dem Skript CSS-Code hinzu:

1. Klicken Sie im Rich-Text-Editor auf das HTML-Symbol.

   ![](assets/image2015-12-29-17-3a56-3a13.png)

1. Fügen Sie den Einbettungscode des Formulars mit dem Stil-Hintergrundcode in den HTML Source Editor ein. Klicks **Aktualisieren**.

   ![](assets/image2015-12-29-18-3a1-3a15.png)

1. Klicks **Vorschau** Sie können sehen, wie es in einer Kampagne dargestellt wird (das Formular wird nicht in der Editor-Ansicht angezeigt). Hier ist ein Beispiel dafür, wie der oben aufgeführte Formular-Code in einer Kampagne mit einem Hintergrundbild wiedergegeben wird.

   ![](assets/image2015-12-29-18-3a20-3a35.png)

>[!MORELIKETHIS]
>
>* [CSS eines Formulardesigns bearbeiten](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md)
>* [Dankesnachricht ohne Folgenachrichten-Landingpage anzeigen](https://developers.marketo.com/blog/show-thank-you-message-without-a-follow-up-landing-page/)
>* [Formulare 2.0](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/forms-api-reference)
