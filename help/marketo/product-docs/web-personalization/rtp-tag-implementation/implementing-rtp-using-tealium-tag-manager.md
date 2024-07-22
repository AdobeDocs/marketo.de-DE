---
unique-page-id: 9437340
description: Implementieren von RTP mit dem Tealium Tag Manager - Marketo Docs - Produktdokumentation
title: Implementieren von RTP mit dem Tag-Manager
exl-id: 7a099184-625c-46b2-a741-3bcdad0a238e
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Implementieren von RTP mit dem Tag-Manager {#implementing-rtp-using-tealium-tag-manager}

Befolgen Sie zur Implementierung Ihres RTP-Tags die unten stehenden Installationsanweisungen.

1. Melden Sie sich bei Ihrem Team-Tag-Manager-Konto an.

1. Navigieren Sie zur Registerkarte Tags und fügen Sie das benutzerdefinierte Tealium-Container-Tag hinzu, das sich auf der Registerkarte Sonstiges im Tag-Marketplace befindet.

1. Geben Sie im Feld &quot;Titel&quot;den Wert **Marketo RTP** ein und klicken Sie auf **Finish**.

1. Speichern Sie Ihre Änderungen.

   >[!NOTE]
   >
   >Der neue Container muss noch nicht veröffentlicht werden.

1. Nachdem das Profil gespeichert wurde, klicken Sie auf Ihren Namen/Ihre E-Mail-Adresse in der oberen rechten Ecke der Tealium iQ-Konsole.

1. Klicken Sie im Menü &quot;Admin&quot;unter &quot;Kontoadministrator&quot;auf **Vorlagen verwalten** .

1. Wählen Sie **Benutzerdefinierter Tealum-Container: Marketo RTP** aus der Dropdownliste aus, um die Tag-Vorlage zu öffnen.

1. Melden Sie sich bei Ihrem RTP-Konto an.

1. Navigieren Sie zu Kontoeinstellungen.

   >[!NOTE]
   >
   >Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 11 fort.

1. Suchen Sie unter &quot;Domäne&quot;die entsprechende Domäne und klicken Sie auf **Tag generieren**.

1. Kopieren Sie das RTP JavaScript-Tag und fügen Sie es zwischen dem Start Tag Library Code und dem End Tag Library Code in Ihre Tealium Profile Template ein.

   >[!NOTE]
   >
   >**Wichtige Schritte**
   >
   >Entfernen Sie die Tags `<!-- RTP tag -->` und `<!-- End of RTP tag -->` aus dem Code, den Sie in dieser Datei platzieren.
   >
   >Entfernen Sie alle `<script type='text/javascript'>` - und `</script>` -Tags aus dem Code, den Sie in dieser Datei platzieren.

1. **Klicken Sie auf Profilvorlage speichern** und veröffentlichen Sie Ihr neues Profil.
