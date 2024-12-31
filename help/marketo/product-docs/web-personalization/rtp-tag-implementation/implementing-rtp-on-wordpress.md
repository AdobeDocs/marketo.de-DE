---
unique-page-id: 4720149
description: Implementieren von RTP in WordPress - Marketo-Dokumente - Produktdokumentation
title: Implementieren von RTP in WordPress
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Implementieren von RTP in WordPress {#implementing-rtp-on-wordpress}

Um Ihr RTP-Tag zu implementieren, befolgen Sie die folgenden Installationsanweisungen:

1. Öffnen Sie die Datei **header.php** Ihres **WordPress-Designs**.

   Sie können entweder einen FTP-Client verwenden, um auf Ihren Server zuzugreifen oder Ihre Design-Dateien direkt über das WordPress-Dashboard bearbeiten. Ihr Dateieditor befindet sich unter der Registerkarte **Erscheinungsbild** im Seitenleistenmenü.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. Suchen Sie in der Liste der Vorlagendateien rechts vom Texteditor nach **header.php** und öffnen Sie diese.

1. Navigieren Sie **Kontoeinstellungen**.

   a. Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 5 fort.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. Suchen Sie unter „Domain“ nach der entsprechenden Domain und klicken Sie auf **Tag generieren**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Kopieren Sie das RTP-JavaScript-Tag und fügen Sie es in Ihre Website-Vorlagen ein.

   a. Stellen Sie sicher, dass es das erste Skript in der Kopfzeile der Seite ist - zwischen den **`<head> </head>`** Tags.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Klicken Sie auf **Datei aktualisieren** für die Datei header.php.

1. Vergewissern Sie sich, dass sie auf allen Seiten angezeigt wird, einschließlich Landingpages und Subdomains.

   a. Klicken Sie dazu mit der rechten Maustaste auf die Seite Ihrer Website. Navigieren Sie zu **Seite anzeigen Source.** Suchen Sie nach **RTP**, um das Tag zu finden.
