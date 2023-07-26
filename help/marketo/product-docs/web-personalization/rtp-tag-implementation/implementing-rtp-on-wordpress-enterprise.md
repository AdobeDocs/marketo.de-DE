---
unique-page-id: 4720215
description: Implementieren von RTP auf Wordpress Enterprise - Marketo Docs - Produktdokumentation
title: Implementieren von RTP in Wordpress Enterprise
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---

# Implementieren von RTP in Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Befolgen Sie zur Implementierung Ihres RTP-Tags die folgenden Installationsanweisungen:

1. Navigieren Sie zu **Kontoeinstellungen**.

   a. Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 3 fort.

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. Suchen Sie unter Domäne die entsprechende Domäne und klicken Sie auf **Tag generieren**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Kopieren Sie das RTP-JavaScript-Tag.

1. Melden Sie sich bei Ihrem WordPress-Konto als Admin-Benutzer an

   a. **Erscheinungsbild**, gehen Sie zu **Benutzerdefiniertes JavaScript**.
b. Fügen Sie das RTP-JavaScript-Tag direkt nach dem vorhandenen Code ein.

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >Schließen Sie beim Einfügen des Codes die folgenden Tags aus:
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`
   >
   >Fügen Sie das Skript NUR selbst ein.

1. Klicks **Aktualisieren**.
