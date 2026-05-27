---
unique-page-id: 4720149
description: Erfahren Sie mehr über die Implementierung von RTP in WordPress in Marketo Engage, einschließlich der Implementierung von RTP in DNL WordPress. Verwenden Sie dieses Handbuch, um Ihren nächsten Schritt abzuschließen.
title: Implementieren von RTP in WordPress
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
TQID: https://experienceleague.adobe.com/5V3CEgasEJi4zrYoezh8Tt340VGHNNHaliF2wdbBLwY
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 202
ht-degree: 3%

---

# Implementieren von RTP in [!DNL Wordpress] {#implementing-rtp-on-wordpress}

Um Ihr [!UICONTROL RTP-Tag ] implementieren, folgen Sie den folgenden Installationsanweisungen:

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

   a. Klicken Sie dazu mit der rechten Maustaste auf die Seite Ihrer Website. Gehen Sie zu **[!UICONTROL Seite Source anzeigen].** Suchen Sie nach **RTP**, um das Tag zu finden.
