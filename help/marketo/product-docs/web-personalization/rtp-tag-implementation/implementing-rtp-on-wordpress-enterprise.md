---
unique-page-id: 4720215
description: Implementierung von RTP auf Wordpress Enterprise - Marketing Docs - Produktdokumentation
title: Implementierung von RTP in Wordpress Enterprise
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---


# Implementierung von RTP auf Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Befolgen Sie zur Implementierung Ihres RTP-Tags die Installationsanweisungen unten:

1. Gehen Sie zu **Kontoeinstellungen**.

   a. Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 3 fort.

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. Suchen Sie unter &quot;Domäne&quot;die entsprechende Domäne und klicken Sie auf **Tag** generieren.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Kopieren Sie das RTP JavaScript-Tag.

1. Melden Sie sich bei Ihrem WordPress-Konto als Admin-Benutzer an

   a. Wechseln Sie unter **Erscheinungsbild** zu **Benutzerdefiniertes JavaScript**.
b. Fügen Sie das RTP-Javascript-Tag direkt nach dem vorhandenen Code ein.

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >BEIM Einfügen des Codes AUSSCHLIESSEN der folgenden Tags:
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`

   >
   >Fügen Sie das Skript NUR selbst ein.

1. Klicken Sie auf **Aktualisieren**.
