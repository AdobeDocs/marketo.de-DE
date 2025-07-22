---
unique-page-id: 10095554
description: Einbetten eines Formulars in eine Web-Kampagne - Marketo-Dokumente - Produktdokumentation
title: Einbetten eines Formulars in eine Web-Kampagne
exl-id: 41e60ae6-9a40-444f-8a55-47fc6ef6c5fb
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 2%

---

# Einbetten eines Formulars in eine Web-Kampagne {#embed-a-form-into-a-web-campaign}

Erfahren Sie, wie Sie ein Marketo-Formular in eine Web-Kampagne einbetten können (Dialogfeld, In-Bereich oder Widget).

1. Rechtsklick auf ein genehmigtes Formular. Wählen Sie **[!UICONTROL Einbettungs-Code]** aus.

   ![](assets/image2015-12-16-10-3a58-3a39.png)

1. Kopieren Sie den Code.

   ![](assets/image2015-12-16-11-3a16-3a24.png)

1. Navigieren Sie [!DNL Web Personalization] zu **[!UICONTROL Web-Kampagnen]**.

   ![](assets/web-campaigns-hand-7.jpg)

1. Klicken Sie **[!UICONTROL Neue Kampagne erstellen]**.

   ![](assets/create-new-web-campaign-hand-1.jpg)

1. Klicken Sie im Rich-Text-Editor auf das HTML-Symbol.

   ![](assets/five-1.png)

1. Fügen Sie den Einbettungs-Code des Formulars in den [!UICONTROL HTML Source Editor] ein. Klicken Sie auf **[!UICONTROL Aktualisieren]**.

   ![](assets/six-1.png)

1. Das Formular wird nicht in der Editor-Ansicht angezeigt, Sie können es jedoch in der Vorschau anzeigen, um zu sehen, wie es in einer Kampagne gerendert wird.

1. Klicken Sie **[!UICONTROL Starten]**, um die Kampagne zu starten.

   >[!NOTE]
   >
   >Alle Änderungen an den Formularfeldern müssen innerhalb der Marketing-Aktivitäten von Marketo in „Formularentwurf bearbeiten“ vorgenommen werden.

## Drei Möglichkeiten zum Hinzufügen eines Hintergrundbilds zu einem Formular {#three-ways-to-add-a-background-image-to-a-form}

Um dem Formular ein Hintergrundbild hinzuzufügen, haben Sie folgende Möglichkeiten:

* Bearbeiten der CSS-Datei eines Formulardesigns
* Ändern der Farben von Dialogfeldern oder Widgets in Campaign Set
* Hinzufügen von CSS-Code zum Skript

Informationen zum Bearbeiten des CSS eines Formulardesigns finden Sie in [diesem Artikel](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md).

So ändern Sie die Farben des Dialogfelds oder Widgets in Campaign Set:

1. Wählen Sie im Rich-Text-Editor einen Dialogfeldkampagnentyp und einen Dialogfeldstil, eine Kopfzeilenfarbe und eine Hintergrundfarbe aus, um die Hintergrundfarben des Formulars anzupassen. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2015-12-29-18-3a28-3a31.png)

1. Im Folgenden finden Sie ein Beispiel dafür, wie ein moderner Trimm-Dialogfeldstil mit einer hellvioletten Kopfzeile und einer Hintergrundfarbe aussieht.

   ![](assets/image2015-12-29-18-3a27-3a31.png)

So fügen Sie dem Skript CSS-Code hinzu:

1. Klicken Sie im Rich-Text-Editor auf das HTML-Symbol.

   ![](assets/image2015-12-29-17-3a56-3a13.png)

1. Fügen Sie den Einbettungs-Code des Formulars mit dem Stil-Code im Hintergrund in den [!UICONTROL HTML Source Editor ein]. Klicken Sie auf **[!UICONTROL Aktualisieren]**.

   ![](assets/image2015-12-29-18-3a1-3a15.png)

1. Klicken Sie **[!UICONTROL Vorschau]**, um zu sehen, wie es in einer Kampagne gerendert wird (das Formular wird nicht in der Editor-Ansicht angezeigt). Im Folgenden finden Sie ein Beispiel dafür, wie der obige Formular-Code in einer Kampagne mit einem Hintergrundbild gerendert wird.

   ![](assets/image2015-12-29-18-3a20-3a35.png)

>[!MORELIKETHIS]
>
>* [Bearbeiten des CSS eines Formulardesigns](/help/marketo/product-docs/demand-generation/forms/form-design/edit-the-css-of-a-form-theme.md)
>* [Dankesnachricht ohne nachfolgende Landingpage anzeigen](https://developers.marketo.com/blog/show-thank-you-message-without-a-follow-up-landing-page/)
>* [Formulare 2.0](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/forms-api-reference)
