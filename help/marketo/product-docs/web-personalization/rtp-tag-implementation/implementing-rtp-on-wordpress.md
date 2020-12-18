---
unique-page-id: 4720149
description: Implementierung von RTP auf Wordpress - Marketing Docs - Produktdokumentation
title: Implementierung von RTP auf Wordpress
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---


# Implementierung von RTP auf Wordpress {#implementing-rtp-on-wordpress}

Befolgen Sie zur Implementierung Ihres RTP-Tags die Installationsanweisungen unten:

1. Öffnen Sie die Datei **header.php** Ihres **WordPress-Designs**.

   Sie können entweder einen FTP-Client verwenden, um auf Ihren Server zuzugreifen, oder Ihre Designdateien direkt über das WordPress-Dashboard bearbeiten. Ihr Dateieditor befindet sich im Seitenleistenmenü unter der Registerkarte **Erscheinungsbild**.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. Suchen Sie in der Liste der Vorlagendateien rechts neben dem Texteditor nach **header.php** und öffnen Sie es.
1. Gehen Sie zu **Kontoeinstellungen.**

   Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 5 fort.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. Suchen Sie unter &quot;Domäne&quot;die entsprechende Domäne und klicken Sie auf **Tag** generieren.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Kopieren Sie das RTP JavaScript-Tag und fügen Sie es in Ihre Website-Vorlagen ein.

   Vergewissern Sie sich, dass es sich um das erste Skript in der Kopfzeile der Seite handelt - zwischen den Tags **`<head> </head>`**.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Klicken Sie für die Datei header.php auf **Datei aktualisieren**.
1. Vergewissern Sie sich, dass sie auf allen `pages including`-Landingpages und -Subdomänen angezeigt wird.

   Dazu klicken Sie mit der rechten Maustaste auf die Seite `website’s`. Gehen Sie zu **Seitenquelle der Ansicht.** Suchen Sie nach  **** RTP, um das Tag zu suchen.
