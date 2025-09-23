---
unique-page-id: 4720149
description: Implementieren von RTP in WordPress - Marketo-Dokumente - Produktdokumentation
title: Implementieren von RTP in WordPress
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 2%

---

# Implementieren von RTP in [!DNL Wordpress] {#implementing-rtp-on-wordpress}

Um Ihr [!UICONTROL RTP-Tag &#x200B;] implementieren, folgen Sie den folgenden Installationsanweisungen:

1. Öffnen Sie die Datei **header.php** Ihres **[!DNL WordPress]Designs**.

   Sie können entweder einen FTP-Client verwenden, um auf Ihren Server zuzugreifen, oder Ihre Design-Dateien direkt über das [!DNL WordPress]-Dashboard bearbeiten. Ihr Dateieditor befindet sich unter der Registerkarte **[!UICONTROL Erscheinungsbild]** im Seitenleistenmenü.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. Suchen Sie in der Liste der Vorlagendateien rechts vom Texteditor nach **header.php** und öffnen Sie diese.

1. Navigieren Sie **[!UICONTROL Kontoeinstellungen]**.

   a. Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 5 fort.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. Suchen Sie unter [!UICONTROL Domain] die entsprechende Domain und klicken Sie auf **[!UICONTROL Tag generieren]**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Kopieren Sie das RTP-JavaScript-Tag und fügen Sie es in Ihre Website-Vorlagen ein.

   a. Stellen Sie sicher, dass es das erste Skript in der Kopfzeile der Seite ist - zwischen den **`<head> </head>`** Tags.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Klicken Sie auf **[!UICONTROL Datei aktualisieren]** für die Datei header.php.

1. Vergewissern Sie sich, dass sie auf allen Seiten angezeigt wird, einschließlich Landingpages und Subdomains.

   a. Klicken Sie dazu mit der rechten Maustaste auf die Seite Ihrer Website. Navigieren Sie **[!UICONTROL Seite Source anzeigen].** Suchen Sie nach **RTP**, um das Tag zu finden.
