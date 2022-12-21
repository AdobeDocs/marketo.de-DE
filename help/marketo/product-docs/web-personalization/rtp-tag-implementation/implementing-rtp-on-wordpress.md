---
unique-page-id: 4720149
description: Implementieren von RTP in Wordpress - Marketo Docs - Produktdokumentation
title: Implementieren von RTP in Wordpress
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# Implementieren von RTP in Wordpress {#implementing-rtp-on-wordpress}

Befolgen Sie zur Implementierung Ihres RTP-Tags die folgenden Installationsanweisungen:

1. Öffnen Sie die **header.php** -Datei **WordPress-Design**.

   Sie können entweder einen FTP-Client verwenden, um auf Ihren Server zuzugreifen, oder Ihre Designdateien direkt im WordPress-Dashboard bearbeiten. Ihr Dateieditor befindet sich unter der **Erscheinungsbild** im Menü der Seitenleiste.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. In der Liste der Vorlagendateien rechts neben dem Texteditor finden Sie **header.php** und öffnen Sie sie.

1. Navigieren Sie zu **Kontoeinstellungen**.

   a. Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 5 fort.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. Suchen Sie unter &quot;Domain&quot;die entsprechende Domäne und klicken Sie auf **Tag generieren**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Kopieren Sie das RTP-JavaScript-Tag und fügen Sie es in Ihre Website-Vorlagen ein.

   a. Stellen Sie sicher, dass es das erste Skript im Header der Seite ist - zwischen dem **`<head> </head>`** Tags.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Klicken Sie auf **Datei aktualisieren** für die Datei header.php.

1. Vergewissern Sie sich, dass sie auf allen Seiten einschließlich Landingpages und Sub-Domains angezeigt wird.

   a. Klicken Sie dazu mit der rechten Maustaste auf die Seite Ihrer Website. Navigieren Sie zu **Seitenquelle anzeigen.** Suchen Sie nach **RTP** , um das Tag zu finden.
