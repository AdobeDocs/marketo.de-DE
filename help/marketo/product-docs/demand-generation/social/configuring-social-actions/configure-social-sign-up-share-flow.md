---
unique-page-id: 2950530
description: Konfigurieren des Flusses für die Anmeldung/Freigabe in Social Media - Marketo-Dokumente - Produktdokumentation
title: Konfigurieren des Flusses für die Anmeldung/Freigabe für Social Media
exl-id: 521187d1-2228-42e7-a87b-3b20a45adb03
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 1%

---

# Konfigurieren des Flusses für die Anmeldung/Freigabe für Social Media {#configure-social-sign-up-share-flow}

Wenn Sie eine Social-Media-App erstellen, können Sie die Auswahl und die Eingabeaufforderungen der Social-Media-Netzwerke konfigurieren, auf die ein Benutzer bei der Anmeldung trifft.

>[!IMPORTANT]
>
>Am 31. Juli 2024 haben wir mit der Einstellung dieser Funktion begonnen. Neue Assets können nicht mehr erstellt werden. Vorhandene Assets funktionieren bis zum 31. Januar 2025 weiterhin. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## Netzwerke für die Freigabe auswählen {#select-networks-for-sharing}

1. Navigieren Sie **Marketing-Aktivitäten**.

   ![](assets/ma-1.png)

1. Wählen Sie die App aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2014-9-22-13-3a57-3a43.png)

1. Klicken Sie im Social-App-Editor **Anmeldefluss** > **Soziale Netzwerke**.

   ![](assets/three.png)

1. Wählen Sie die Netzwerke aus, für die eine Person freigeben kann, oder heben Sie die Auswahl auf.

   ![](assets/four.png)

## Konfigurieren der Facebook-Nachricht {#configure-the-facebook-message}

1. Navigieren Sie **Anmeldefluss** > **Nachrichten freigeben**.

   ![](assets/five.png)

1. Konfigurieren Sie die Nachricht, die in Facebook-Beiträgen angezeigt wird.

   ![](assets/image2014-9-22-13-3a58-3a54.png)

   >[!NOTE]
   >
   >In einer Videofreigabe wird die Miniaturansicht automatisch generiert.

   Wenn Sie **Dynamischen Inhalt hinzufügen** wählen, werden die Werte der **OpenGraph**-Tags (og:title, og:caption und og:description) der Seite und die Miniaturansicht automatisch zu Facebook-Beiträgen hinzugefügt. Siehe den nächsten Schritt.

   Wenn Sie **Statischen Inhalt hinzufügen** wählen, geben Sie den Titel, die Beschriftung und die Beschreibung ein und laden Sie ein Bild hoch. Siehe die nächsten beiden Schritte.

1. Klicken Sie im Fenster Anzeigen und bearbeiten auf **Bearbeitungen anzeigen** und bearbeiten Sie die Freigabeaufforderung und -meldung, die in Facebook-Beiträgen angezeigt werden.

   >[!TIP]
   >
   >Weitere Informationen finden Sie unter [Facebook Rich-Post-Einstellungen bearbeiten](/help/marketo/product-docs/demand-generation/facebook/edit-facebook-rich-post-settings.md).

   ![](assets/image2014-9-22-13-3a59-3a57.png)

   >[!NOTE]
   >
   >Die [Freigabe](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md)URL wird automatisch zu allen freigegebenen Nachrichten hinzugefügt.

1. Wenn Sie oben **Statischen Inhalt hinzufügen** ausgewählt haben, bearbeiten Sie den Titel, die Beschriftung und die Beschreibung und laden Sie ein benutzerdefiniertes Bild hoch (aus Ihren [**Marketo-Bildern und -Dateien**](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md)).

   ![](assets/image2014-9-22-14-3a1-3a11.png)

   Siehe [Hinzufügen von Bildern und Dateien zu Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md).

   >[!NOTE]
   >
   >Wenn Sie ein Bild hochladen, wird es hier erst angezeigt, wenn Sie den Social-App-Editor schließen und erneut öffnen.

1. Klicken Sie auf **Weiter**.

Wenn Sie die Werte der Tags der Seite (og:title, og:caption und og:description) auswählen und die Miniaturansicht automatisch zu Facebook-Beiträgen hinzugefügt wird. Siehe den nächsten Schritt.

## Konfigurieren der Twitter-Nachricht {#configure-the-twitter-message}

1. Bearbeiten Sie die Freigabeaufforderung und die Nachricht, die in Twitter-Tweets angezeigt werden.

   ![](assets/image2014-9-22-14-3a2-3a31.png)

   >[!TIP]
   >
   >Verwenden Sie {html_title} in Ihrem Tweet-Text, um den Titel der Seite automatisch anzuzeigen.

1. Klicken Sie auf **Weiter**.

## Konfigurieren der LinkedIn-Nachricht {#configure-the-linkedin-message}

1. Konfigurieren Sie die Nachricht, die in LinkedIn-Beiträgen angezeigt wird.

   ![](assets/image2014-9-22-14-3a3-3a8.png)

   Wenn Sie **Dynamischen Inhalt hinzufügen** wählen, werden die Werte der Seiten-Tags (Titel und Beschreibung) und die Miniaturansicht automatisch zu LinkedIn-Beiträgen hinzugefügt. Siehe den nächsten Schritt.

   Wenn Sie **Statischen Inhalt hinzufügen** wählen, geben Sie den Titel, die Beschriftung und die Beschreibung ein und laden Sie ein Bild hoch. Siehe die nächsten beiden Schritte.

1. Klicken Sie im Fenster **Anzeigen und bearbeiten** auf **Bearbeitungen anzeigen** und bearbeiten Sie die Freigabeaufforderung und -meldung, die in LinkedIn-Beiträgen angezeigt werden.

   ![](assets/image2014-9-22-14-3a4-3a6.png)

   >[!TIP]
   >
   >Verwenden Sie {html_title} in Ihrem Post-Text, um den Titel der Seite automatisch anzuzeigen.

1. Wenn Sie oben &quot;**Inhalt hinzufügen** ausgewählt haben, bearbeiten Sie den Titel und die Beschreibung und laden Sie ein benutzerdefiniertes Bild hoch (aus Ihren [**Marketo-Bildern und -Dateien**](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md)).

   ![](assets/image2014-9-22-13-3a55-3a17.png)

>[!NOTE]
>
>Wenn Sie ein Bild hochladen, wird es hier erst angezeigt, wenn Sie den Social-App-Editor schließen und erneut öffnen.

>[!MORELIKETHIS]
>
>Als Nächstes können Sie auf **Beenden** > **Genehmigen und schließen** klicken und Ihre Social-Media-App auf einer Landingpage ablegen. Sie können auch die [Personenerfassung](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-person-capture-for-a-social-app.md) oder die Eingabeaufforderung [erneute Freigabe“ ](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-re-share-email-and-prompt-for-a-social-app.md).
