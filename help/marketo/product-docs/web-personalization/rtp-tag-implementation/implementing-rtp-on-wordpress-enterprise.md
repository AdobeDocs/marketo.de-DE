---
unique-page-id: 4720215
description: Erfahren Sie mehr über die Implementierung von RTP in WordPress Enterprise in Marketo Engage, einschließlich der Implementierung von RTP in WordPress. Verwenden Sie dieses Handbuch, um Ihren nächsten Schritt abzuschließen.
title: Implementieren von RTP in WordPress Enterprise
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
TQID: 'https://experienceleague.adobe.com/S0LvRrD1V6hkWN5L5TlnoaIqcDvXLjfm5do2-1WQTNw'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
    internal-label: Implementation
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
    internal-label: Personalization
  - id: 664d862c-1673-5ed4-a3d6-386ac83225e4
    internal-label: Web Personalization
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 13%
---
# Implementieren von RTP in WordPress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Um Ihr [!UICONTROL RTP-Tag ] implementieren, folgen Sie den folgenden Installationsanweisungen:

1. Navigieren Sie **[!UICONTROL Kontoeinstellungen]**.

   a. Wenn Sie bereits Ihr JavaScript-Tag vom Support erhalten haben, fahren Sie mit Schritt 3 fort.

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. Suchen Sie unter [!UICONTROL Domain] die entsprechende Domain und klicken Sie auf **[!UICONTROL Tag generieren]**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Kopieren Sie das RTP-JavaScript-Tag.

1. Melden Sie sich bei Ihrem [!DNL WordPress] als Admin-Benutzer an

   a. Navigieren **[!UICONTROL unter]** zu **[!UICONTROL Benutzerdefiniertes JavaScript]**.
   b. Fügen Sie das RTP-JavaScript-Tag direkt nach dem vorhandenen Code ein.

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >Beim Einfügen des Codes schließen Sie die folgenden Tags aus:
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`
   >
   >Fügen Sie das Skript NUR selbst ein.

1. Klicken Sie auf **[!UICONTROL Aktualisieren]**.
