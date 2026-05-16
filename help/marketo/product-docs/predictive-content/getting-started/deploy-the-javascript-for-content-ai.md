---
unique-page-id: 11385053
description: Erfahren Sie, wie Sie das RTP-Web-Personalization-Tag für prädiktive Inhalte generieren und platzieren. Kopieren Sie sie in Ihren Seitenkopf, überprüfen Sie die Abdeckung und bestätigen Sie, dass der Umschalter aktiviert bleibt.
title: Bereitstellen von JavaScript für Content-AI
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
TQID: https://experienceleague.adobe.com/LHzl0KuIoJvZ99eFWGFE6RdDW1xRxBS4LG3XU9ujj4U
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 162
ht-degree: 8%

---

# Bereitstellen von JavaScript für Content-AI {#deploy-the-javascript-for-content-ai}

Um prädiktive Inhalte zu verwenden, müssen Sie das RTP-Tag (Web Personalization) generieren und einrichten.

## Tag generieren {#generate-tag}

1. Melden Sie sich bei Ihrem Predictive Content-Konto an. Navigieren Sie **[!UICONTROL Kontoeinstellungen]**.

   ![](assets/settings-dropdown-account-hands.png)

1. Suchen Sie **[!UICONTROL Domain-Konfiguration]** die entsprechende Domain und klicken Sie auf **[!UICONTROL Tag generieren]**.

   ![](assets/generate-tag.png)

1. Kopieren Sie das Web-Personalization-Tag und fügen Sie es in die HTML Ihrer Website ein.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Kopieren Sie das Tag Web Personalization JavaScript und fügen Sie es als erstes Skript in die Kopfzeile Ihrer Seiten zwischen den `<head> </head>` Tags ein. Weitere Informationen finden Sie [Implementierungsanweisungen hier](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Überprüfen Sie, ob das Tag auf allen Seiten angezeigt wird, einschließlich Landingpages und Subdomains. Überprüfen Sie dies, indem Sie mit der rechten Maustaste auf die Seite Ihrer Website klicken. Navigieren Sie **[!UICONTROL Seite Source anzeigen]** in einem Webbrowser. Suche: „RTP“.

1. Bestätigen Sie, dass der Umschalter Tag auf **[!UICONTROL EIN]** eingestellt ist.
