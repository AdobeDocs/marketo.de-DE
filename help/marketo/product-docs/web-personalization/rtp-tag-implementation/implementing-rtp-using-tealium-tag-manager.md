---
unique-page-id: 9437340
description: Erfahren Sie mehr über die Implementierung von RTP mit dem Tagmanager Tealium in Marketo Engage, einschließlich der Implementierung von RTP mit DNL. Verwenden Sie dieses Handbuch, um Ihren nächsten Schritt abzuschließen.
title: Implementieren von RTP mit dem Tealium Tag Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 50befbf7339cd7a8b25b0942515497f6acc8f9ab
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 3%

---

# Implementieren von RTP mit [!DNL Tealium] Tag Manager {#implementing-rtp-using-tealium-tag-manager}

Um Ihr RTP-Tag zu implementieren, folgen Sie bitte den unten stehenden Installationsanweisungen.

1. Melden Sie sich bei Ihrem [!DNL Tealium] Tag Manager-Konto an.

1. Navigieren Sie zur Registerkarte [!UICONTROL Tags] und fügen Sie das [!UICONTROL Tealium Custom Container Tag] hinzu, das sich auf der Registerkarte [!UICONTROL Sonstiges] des Tags-Marktplatzes befindet.

1. Geben [!UICONTROL  im Feld „Titel] **Marketo RTP ein** klicken Sie auf **[!UICONTROL Beenden]**.

1. Speichern Sie Ihre Änderungen.

   >[!NOTE]
   >
   >Es ist noch nicht erforderlich, den neuen Container zu veröffentlichen.

1. Nachdem das Profil gespeichert wurde, klicken Sie auf Ihren Namen/Ihre E-Mail-Adresse in der oberen rechten Ecke der Tealium iQ-Konsole.

1. Klicken Sie im Menü [!UICONTROL Admin] unter **[!UICONTROL Kontoadministrator]** auf [!UICONTROL Vorlagen verwalten].

1. Wählen Sie **[!UICONTROL Tealium Custom Container]: Marketo RTP** aus der Dropdown-Liste aus, um die Tag-Vorlage zu öffnen.

1. Melden Sie sich bei Ihrem RTP-Konto an.

1. Navigieren Sie [!UICONTROL Kontoeinstellungen].

   >[!NOTE]
   >
   >Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 11 fort.

1. Suchen Sie unter „Domain“ nach der entsprechenden Domain und klicken Sie auf **[!UICONTROL Tag generieren]**.

1. Kopieren Sie das RTP JavaScript-Tag und fügen Sie es zwischen [!UICONTROL Start Tag Library Code] und [!UICONTROL End Tag Library Code] in Ihre Tealium-Profilvorlage ein.

   >[!NOTE]
   >
   >**Wichtige Schritte**
   >
   >Entfernen Sie die `<!-- RTP tag -->`- und `<!-- End of RTP tag -->`-Tags aus dem Code, den Sie in diese Datei einfügen.
   >
   >Entfernen Sie alle `<script type='text/javascript'>`- und `</script>`-Tags aus dem Code, den Sie in diese Datei einfügen.

1. Klicken Sie **[!UICONTROL Profilvorlage speichern]** und veröffentlichen Sie Ihr neues Profil.
