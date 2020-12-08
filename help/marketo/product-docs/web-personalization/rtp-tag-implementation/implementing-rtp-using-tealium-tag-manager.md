---
unique-page-id: 9437340
description: Implementierung von RTP mit dem Tealium Tag Manager - MarketingTo Docs - Produktdokumentation
title: Implementierung von RTP mit dem Tealium Tag Manager
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Implementierung von RTP mit dem Tealium Tag Manager {#implementing-rtp-using-tealium-tag-manager}

Zur Implementierung Ihres RTP-Tags folgen Sie den Installationsanweisungen unten.

1. Melden Sie sich bei Ihrem Team Tag Manager-Konto an.
1. Navigieren Sie zur Registerkarte &quot;Tags&quot;und fügen Sie das Tag &quot;Tealium Custom Container&quot;hinzu, das sich auf der Registerkarte &quot;Misc&quot;des Tags Marketplace befindet.
1. Geben Sie im Feld Titel **Marketo RTP** ein und klicken Sie auf **Fertig stellen**.
1. Speichern Sie Ihre Änderungen.

   >[!NOTE]
   >
   >Der neue Container muss noch nicht veröffentlicht werden.

1. Klicken Sie nach dem Speichern des Profils auf Ihren Namen/Ihre E-Mail-Adresse in der oberen rechten Ecke der Tealium iQ-Konsole.
1. Klicken Sie im Menü &quot;Admin&quot;unter &quot;Kontoadministrator&quot;auf Vorlagen **verwalten** .
1. Wählen Sie &quot; **Tealium Custom Container&quot;: Marketo RTP** aus der Dropdown-Liste, um die Tag-Vorlage zu öffnen.
1. Melden Sie sich bei Ihrem RTP-Konto an.
1. Wechseln Sie zu Kontoeinstellungen.

   >[!NOTE]
   >
   >Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 11 fort.

1. Suchen Sie unter &quot;Domäne&quot;die entsprechende Domäne und klicken Sie auf Tag **generieren**.
1. Kopieren Sie das RTP-JavaScript-Tag und fügen Sie es zwischen dem Beginn-Tag-Bibliothekscode und dem End-Tag-Bibliothekscode in Ihre Tealium-Profil-Vorlage ein.

   >[!NOTE]
   >
   >**Wichtige Schritte**
   >
   >Entfernen Sie die Tags `<!-- RTP tag -->` und `<!-- End of RTP tag -->` aus dem Code, den Sie in dieser Datei platzieren.
   >
   >Entfernen Sie alle `<script type='text/javascript'>` und `</script>` -Tags aus dem Code, den Sie in dieser Datei platzieren.

1. **Klicken Sie auf Profil-Vorlage** speichern und veröffentlichen Sie Ihr neues Profil.

