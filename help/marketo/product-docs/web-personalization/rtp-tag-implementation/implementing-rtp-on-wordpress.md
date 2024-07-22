---
unique-page-id: 4720149
description: Implementieren von RTP in Wordpress - Marketo Docs - Produktdokumentation
title: Implementieren von RTP in Wordpress
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Implementieren von RTP in Wordpress {#implementing-rtp-on-wordpress}

Befolgen Sie zur Implementierung Ihres RTP-Tags die folgenden Installationsanweisungen:

1. Öffnen Sie die Datei **header.php** Ihres **WordPress-Designs**.

   Sie können entweder einen FTP-Client verwenden, um auf Ihren Server zuzugreifen, oder Ihre Designdateien direkt im WordPress-Dashboard bearbeiten. Ihr Dateieditor befindet sich auf der Registerkarte **Erscheinungsbild** im Seitenleistenmenü.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. Suchen Sie in der Liste der Vorlagendateien rechts neben dem Texteditor **header.php** und öffnen Sie sie.

1. Wechseln Sie zu **Kontoeinstellungen**.

   a. Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 5 fort.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. Suchen Sie unter &quot;Domäne&quot;die entsprechende Domäne und klicken Sie auf **Tag generieren**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Kopieren Sie das RTP JavaScript-Tag und fügen Sie es in Ihre Website-Vorlagen ein.

   a. Stellen Sie sicher, dass es sich um das erste Skript im Header der Seite handelt - zwischen den **`<head> </head>`** -Tags.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Klicken Sie auf **Datei aktualisieren** für die Datei &quot;header.php&quot;.

1. Vergewissern Sie sich, dass sie auf allen Seiten einschließlich Landingpages und Sub-Domains angezeigt wird.

   a. Klicken Sie mit der rechten Maustaste auf die Seite Ihrer Website. Navigieren Sie zu **Seite Source anzeigen .** Suchen Sie nach **RTP** , um das Tag zu finden.
