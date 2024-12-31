---
unique-page-id: 9437340
description: Implementieren von RTP mit Tealium Tag Manager - Marketo-Dokumente - Produktdokumentation
title: Implementieren von RTP mit dem Tealium Tag Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 1%

---

# Implementieren von RTP mit dem Tealium Tag Manager {#implementing-rtp-using-tealium-tag-manager}

Um Ihr RTP-Tag zu implementieren, folgen Sie bitte den unten stehenden Installationsanweisungen.

1. Melden Sie sich bei Ihrem Tealium Tag Manager-Konto an.

1. Navigieren Sie zur Registerkarte Tags und fügen Sie das benutzerdefinierte Tag Tealium-Container hinzu, das sich auf der Registerkarte Sonstiges des Tags-Marketplace befindet.

1. Geben Sie im Feld Titel **Marketo RTP** ein und klicken Sie auf **Beenden**.

1. Speichern Sie Ihre Änderungen.

   >[!NOTE]
   >
   >Es ist noch nicht erforderlich, den neuen Container zu veröffentlichen.

1. Nachdem das Profil gespeichert wurde, klicken Sie auf Ihren Namen/Ihre E-Mail-Adresse in der oberen rechten Ecke der Tealium iQ-Konsole.

1. Klicken Sie im Menü Admin auf **Vorlagen verwalten** unter Kontoadministrator.

1. Wählen Sie **Tealium Custom Container: Marketo RTP** aus der Dropdown-Liste aus, um die Tag-Vorlage zu öffnen.

1. Melden Sie sich bei Ihrem RTP-Konto an.

1. Zu den Kontoeinstellungen gehen.

   >[!NOTE]
   >
   >Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 11 fort.

1. Suchen Sie unter „Domain“ nach der entsprechenden Domain und klicken Sie auf **Tag generieren**.

1. Kopieren Sie das RTP-JavaScript-Tag und fügen Sie es zwischen dem Code der Start-Tag-Bibliothek und dem Code der End-Tag-Bibliothek in Ihre Tealium-Profilvorlage ein.

   >[!NOTE]
   >
   >**Wichtige Schritte**
   >
   >Entfernen Sie die `<!-- RTP tag -->`- und `<!-- End of RTP tag -->`-Tags aus dem Code, den Sie in diese Datei einfügen.
   >
   >Entfernen Sie alle `<script type='text/javascript'>`- und `</script>`-Tags aus dem Code, den Sie in diese Datei einfügen.

1. **Klicken Sie auf Profilvorlage speichern** und veröffentlichen Sie Ihr neues Profil.
