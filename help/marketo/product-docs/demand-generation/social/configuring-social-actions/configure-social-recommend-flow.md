---
unique-page-id: 2950549
description: Konfigurieren des empfohlenen Social-Media-Flusses - Marketo-Dokumente - Produktdokumentation
title: Empfohlene Social-Media-Flüsse konfigurieren
exl-id: 01b54215-4a0c-4639-80d2-ec30603b3695
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 1%

---

# Empfohlene Social-Media-Flüsse konfigurieren {#configure-social-recommend-flow}

Wenn Sie eine Social-Media-App erstellen, können Sie die Auswahl und die Eingabeaufforderungen der Social-Media-Netzwerke konfigurieren, auf die ein Benutzer bei der Anmeldung trifft.

>[!IMPORTANT]
>
>Am 31. Juli 2024 haben wir mit der Einstellung dieser Funktion begonnen. Neue Assets können nicht mehr erstellt werden. Vorhandene Assets funktionieren bis zum 31. Januar 2025 weiterhin. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## Netzwerke für die Freigabe auswählen {#select-networks-for-sharing}

>[!NOTE]
>
>Dies ähnelt sehr dem [Konfigurieren des Social-Anmelde-/Freigabeflusses](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-social-sign-up-share-flow.md), aber dies ist für die Freigabe-Links _unter_ der Social-App.

1. Navigieren Sie **Marketing-Aktivitäten**.

   ![](assets/login-marketing-activities-1.png)

1. Wählen Sie die App aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2014-9-22-11-3a51-3a6.png)

1. Gehen Sie im Social-App-Editor zu **Fluss empfehlen** > **Soziale Netzwerke**.

   ![](assets/recommendedflow.png)

1. Wählen Sie die Netzwerke aus, die ein Benutzer freigeben kann.

   ![](assets/socialnetworkschoose.png)

## Konfigurieren der Facebook-Nachricht {#configure-the-facebook-message}

1. Konfigurieren Sie die Nachricht, die in Facebook-Beiträgen angezeigt wird.

   ![](assets/image2014-9-22-11-3a53-3a21.png)

   >[!NOTE]
   >
   >In einer Videofreigabe wird die Miniaturansicht automatisch generiert.

   Wenn Sie **Dynamischen Inhalt hinzufügen** wählen, werden die Werte der OpenGraph-Tags der Seite (og:title, og:caption und og:description) und die Miniaturansicht automatisch zu Facebook-Beiträgen hinzugefügt. Siehe den nächsten Schritt.

   Wenn Sie **Statischen Inhalt hinzufügen** wählen, geben Sie den Titel, die Beschriftung und die Beschreibung ein und laden Sie ein Bild hoch. Siehe die nächsten beiden Schritte.

1. Klicken Sie im Fenster Anzeigen und bearbeiten auf **Bearbeitungen anzeigen**, um die Freigabeaufforderung und -meldung anzupassen, die in Facebook-Beiträgen angezeigt werden.

   >[!TIP]
   >
   >Weitere Informationen finden Sie unter [Facebook Rich-Post-Einstellungen bearbeiten](/help/marketo/product-docs/demand-generation/facebook/edit-facebook-rich-post-settings.md).

   ![](assets/image2014-9-22-11-3a54-3a36.png)

   >[!NOTE]
   >
   >Die [Freigabe](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md)URL wird automatisch zu allen freigegebenen Nachrichten hinzugefügt.

1. Wenn Sie oben **Statischen Inhalt hinzufügen** ausgewählt haben, bearbeiten Sie den Titel, die Beschriftung und die Beschreibung und laden Sie ein benutzerdefiniertes Bild (aus Ihren Marketo-Bildern und -Dateien) hoch.

   ![](assets/image2014-9-22-11-3a55-3a14.png)

   Siehe [Hinzufügen von Bildern und Dateien zu Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md).

   >[!NOTE]
   >
   >Wenn Sie ein Bild hochladen, wird es hier erst angezeigt, wenn Sie den Social-App-Editor schließen und erneut öffnen.

1. Klicken Sie auf **Weiter**.

Wenn Sie auswählen, werden die Werte der OpenGraph-Tags der Seite (og:title, og:caption und og:description) und die Miniaturansicht automatisch zu Facebook-Beiträgen hinzugefügt. Siehe den nächsten Schritt.

## Konfigurieren der Twitter-Nachricht {#configure-the-twitter-message}

1. Klicken Sie hier, um die Eingabeaufforderung und Nachricht zu bearbeiten, die beim Twitter von Tweets angezeigt werden.

   ![](assets/image2014-9-22-12-3a2-3a40.png)

   >[!TIP]
   >
   >Verwenden Sie {html_title} in Ihrem Tweet-Text, um den Titel der Seite automatisch anzuzeigen.

1. Klicken Sie auf **Weiter**.

## Konfigurieren der LinkedIn-Nachricht {#configure-the-linkedin-message}

1. Konfigurieren Sie die Nachricht, die in LinkedIn-Beiträgen angezeigt wird.

   ![](assets/image2014-9-22-12-3a3-3a21.png)

   Wenn Sie **Dynamischen Inhalt hinzufügen** auswählen, werden die Werte der Seiten-Tags (Titel und Beschreibung) und die Miniaturansicht automatisch zu LinkedIn-Beiträgen hinzugefügt. Siehe den nächsten Schritt.

   Wenn Sie **Statischen Inhalt hinzufügen** wählen, geben Sie den Titel, die Beschriftung und die Beschreibung ein und laden Sie ein Bild hoch. Siehe die nächsten beiden Schritte.

1. Klicken Sie im Fenster **Anzeigen und bearbeiten** auf **Bearbeitungen anzeigen** und bearbeiten Sie die Freigabeaufforderung und -meldung, die in LinkedIn-Beiträgen angezeigt werden.

   ![](assets/image2014-9-22-12-3a3-3a38.png)

   >[!TIP]
   >
   >Verwenden Sie {html_title} in Ihrem Post-Text, um den Titel der Seite automatisch anzuzeigen.

1. Wenn Sie oben **Statischen Inhalt hinzufügen** ausgewählt haben, bearbeiten Sie den Titel und die Beschreibung und laden Sie ein benutzerdefiniertes Bild (aus Ihren Marketo-Bildern und -Dateien) hoch.

   ![](assets/image2014-9-22-12-3a4-3a43.png)

   Siehe [Hinzufügen von Bildern und Dateien zu Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md).

   >[!NOTE]
   >
   >Wenn Sie ein Bild hochladen, wird es hier erst angezeigt, wenn Sie den Social-App-Editor schließen und erneut öffnen.

1. Klicken Sie auf **Weiter**.

## Bestätigungsnachricht konfigurieren {#configure-the-confirmation-message}

1. Bearbeiten Sie den Text der Freigabebestätigung.

   ![](assets/image2014-9-22-12-3a5-3a30.png)

1. Klicken Sie **Beenden** > **Genehmigen** und **Schließen**.

   ![](assets/image2014-9-22-12-3a5-3a45.png)

>[!MORELIKETHIS]
>
>Der nächste Schritt besteht darin[ ](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-video-share-flow.md) Ihre Videofreigabe oder [Abfrage](/help/marketo/product-docs/demand-generation/social/creating-a-poll/create-a-poll.md) zu einer Landingpage, Facebook oder Ihrer eigenen Website hinzuzufügen.
