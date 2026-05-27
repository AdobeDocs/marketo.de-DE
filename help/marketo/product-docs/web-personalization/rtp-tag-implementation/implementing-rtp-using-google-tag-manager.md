---
unique-page-id: 4720145
description: Erfahren Sie mehr über die Implementierung von RTP mithilfe von Google Tag Manager in Marketo Engage, einschließlich der Implementierung von RTP mithilfe von Google DNL. Verwenden Sie dieses Handbuch, um Ihren nächsten Schritt abzuschließen.
title: Implementieren von RTP mit dem Google Tag Manager
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
TQID: https://experienceleague.adobe.com/XesXGBf2aDsnsbS2Ro1RLdd1EVrj-mBdCiv8C0dj8NU
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 173
ht-degree: 4%

---

# Implementieren von RTP mit [!DNL Google Tag Manager] {#implementing-rtp-using-google-tag-manager}

Um Ihr RTP-Tag zu implementieren, folgen Sie bitte den unten stehenden Installationsanweisungen.

1. Melden Sie sich bei Ihrem [!DNL Google Tag Manager] an.

1. Fügen Sie ein neues **[!UICONTROL Tag]** > **[!UICONTROL Tag-Konfigurationen]** > **[!UICONTROL Benutzerdefiniertes HTML-Tag] hinzu.** Nennen Sie es **RTP**.

1. Melden Sie sich bei Ihrem **RTP-** an.

1. Navigieren Sie **[!UICONTROL Kontoeinstellungen]**.

   a. Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 6 fort.

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. Suchen Sie unter [!UICONTROL Domain] die entsprechende Domain und klicken Sie auf **[!UICONTROL Tag generieren]**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. Kopieren Sie das RTP-JavaScript-Tag und fügen Sie es in das neue **benutzerdefinierte HTML-Tag** ein, das Sie erstellt haben (Schritt 1).

1. Klicken Sie **[!UICONTROL Regel zu Auslöser-Tag hinzufügen]**. Wählen Sie **[!UICONTROL Alle Seiten]** aus.

1. Klicken Sie auf **[!UICONTROL Speichern]** und [veröffentlichen Sie die neue Version](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Vergewissern Sie sich, dass sie auf allen Seiten angezeigt wird, einschließlich Landingpages und Subdomains.

   a. Klicken Sie dazu mit der rechten Maustaste auf die Seite Ihrer Website. Navigieren Sie zu **[!UICONTROL Element überprüfen]**, suchen Sie nach **RTP**, um das Tag zu finden.
