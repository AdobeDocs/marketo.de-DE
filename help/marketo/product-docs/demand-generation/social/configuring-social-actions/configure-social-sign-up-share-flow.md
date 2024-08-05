---
unique-page-id: 2950530
description: Konfigurieren des Social-Anmeldungs-/Freigabeflusses - Marketo-Dokumente - Produktdokumentation
title: Konfigurieren des Social-Anmeldungs-/Freigabeflusses
exl-id: 521187d1-2228-42e7-a87b-3b20a45adb03
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 1%

---

# Konfigurieren des Social-Anmeldungs-/Freigabeflusses {#configure-social-sign-up-share-flow}

Wenn Sie eine Social-App erstellen, können Sie die Auswahlmöglichkeiten für soziale Netzwerke konfigurieren und Aufforderungen festlegen, auf die ein Benutzer bei seiner Anmeldung stößt.

>[!IMPORTANT]
>
>Am 31. Juli 2024 begannen wir mit der Einstellung dieser Funktion. Neue Assets können nicht mehr erstellt werden. Vorhandene Assets werden bis zum 31. Januar 2025 weiterhin funktionieren. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## Netzwerke für die Freigabe auswählen {#select-networks-for-sharing}

1. Wechseln Sie zu **Marketingaktivitäten**.

   ![](assets/ma-1.png)

1. Wählen Sie die App aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2014-9-22-13-3a57-3a43.png)

1. Klicken Sie im Social-App-Editor auf **Anmeldungs-Fluss** > **Soziale Netzwerke**.

   ![](assets/three.png)

1. Wählen Sie die Netzwerke aus, für die eine Person freigeben kann (oder deaktivieren Sie sie).

   ![](assets/four.png)

## Konfigurieren der Facebook-Nachricht {#configure-the-facebook-message}

1. Wechseln Sie zu **Anmeldungs-Fluss** > **Nachrichten teilen**.

   ![](assets/five.png)

1. Konfigurieren Sie die Nachricht, die in Facebook-Beiträgen angezeigt wird.

   ![](assets/image2014-9-22-13-3a58-3a54.png)

   >[!NOTE]
   >
   >Bei einer Videofreigabe wird die Miniaturansicht automatisch generiert.

   Wenn Sie **Dynamischen Inhalt hinzufügen** auswählen, werden die Werte der **OpenGraph** -Tags der Seite (og:title, og:caption und og:description) und die Miniaturansicht automatisch zu Facebook-Beiträgen hinzugefügt. Siehe nächsten Schritt.

   Wenn Sie **Statischen Inhalt hinzufügen** auswählen, geben Sie den Titel, die Beschriftung, die Beschreibung ein und laden Sie ein Bild hoch. Siehe die nächsten beiden Schritte.

1. Klicken Sie im Fenster &quot;Ansicht und Bearbeiten&quot;auf **Bearbeitungen anzeigen** und bearbeiten Sie die Freigabeaufforderung und -meldung, die in Facebook-Beiträgen angezeigt werden.

   >[!TIP]
   >
   >Weitere Informationen finden Sie unter [Bearbeiten der Rich-Post-Einstellungen für Facebook](/help/marketo/product-docs/demand-generation/facebook/edit-facebook-rich-post-settings.md).

   ![](assets/image2014-9-22-13-3a59-3a57.png)

   >[!NOTE]
   >
   >Die [Freigabe-URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) wird automatisch zu allen Freigabemeldungen hinzugefügt.

1. Wenn Sie oben &quot;**Statischen Inhalt hinzufügen**&quot;ausgewählt haben, bearbeiten Sie den Titel, die Beschriftung und die Beschreibung und laden Sie ein benutzerdefiniertes Bild hoch (aus Ihren [**Marketo-Bildern und -Dateien**](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md)).

   ![](assets/image2014-9-22-14-3a1-3a11.png)

   Siehe [Hinzufügen von Bildern und Dateien zu Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md).

   >[!NOTE]
   >
   >Wenn Sie ein Bild hochladen, wird es hier erst angezeigt, wenn Sie den Social-App-Editor schließen und erneut öffnen.

1. Klicken Sie auf **Weiter**.

Wenn Sie die Werte der Tags der Seite auswählen (og:title, og:caption und og:description), werden die Miniaturansichten automatisch zu Facebook-Beiträgen hinzugefügt. Siehe nächsten Schritt.

## Konfigurieren der Twitter-Nachricht {#configure-the-twitter-message}

1. Bearbeiten Sie die Freigabeaufforderung und -meldung, die in Twitter-Tweets angezeigt werden.

   ![](assets/image2014-9-22-14-3a2-3a31.png)

   >[!TIP]
   >
   >Verwenden Sie {html_title} in Ihrem Tweet-Text, um den Titel der Seite automatisch anzuzeigen.

1. Klicken Sie auf **Weiter**.

## Konfigurieren der LinkedIn-Nachricht {#configure-the-linkedin-message}

1. Konfigurieren Sie die Nachricht, die in LinkedIn-Beiträgen angezeigt wird.

   ![](assets/image2014-9-22-14-3a3-3a8.png)

   Wenn Sie **Dynamischen Inhalt hinzufügen** auswählen, werden die Werte der Seiten-Tags (Titel und Beschreibung) und die Miniaturansicht automatisch zu LinkedIn-Beiträgen hinzugefügt. Siehe nächsten Schritt.

   Wenn Sie **Statischen Inhalt hinzufügen** auswählen, geben Sie den Titel, die Beschriftung und die Beschreibung ein und laden Sie ein Bild hoch. Siehe die nächsten beiden Schritte.

1. Klicken Sie im Fenster **Anzeigen und Bearbeiten** auf **Bearbeitungen anzeigen** und bearbeiten Sie die Freigabeaufforderung und -meldung, die in LinkedIn-Beiträgen angezeigt werden.

   ![](assets/image2014-9-22-14-3a4-3a6.png)

   >[!TIP]
   >
   >Verwenden Sie {html_title} in Ihrem Beitragstext, um den Seitentitel automatisch anzuzeigen.

1. Wenn Sie oben &quot;**Statischen Inhalt hinzufügen**&quot;ausgewählt haben, bearbeiten Sie den Titel und die Beschreibung und laden Sie ein benutzerdefiniertes Bild hoch (aus Ihren [**Marketo-Bildern und -Dateien**](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md)).

   ![](assets/image2014-9-22-13-3a55-3a17.png)

>[!NOTE]
>
>Wenn Sie ein Bild hochladen, wird es hier erst angezeigt, wenn Sie den Social-App-Editor schließen und erneut öffnen.

>[!MORELIKETHIS]
>
>Als Nächstes können Sie auf **Beenden** > **Genehmigen und schließen** klicken und Ihre Social-App auf eine Landingpage stellen. Sie können auch die [Personenerfassung](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-person-capture-for-a-social-app.md) oder die [Aufforderung zur erneuten Freigabe](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-re-share-email-and-prompt-for-a-social-app.md) konfigurieren.
