---
unique-page-id: 4720151
description: Erfahren Sie mehr über die Implementierung von RTP auf Marketo-Landingpages in Marketo Engage, einschließlich der Implementierung von RTP auf Marketo. Verwenden Sie dieses Handbuch, um Ihren nächsten Schritt abzuschließen.
title: Implementieren von RTP in Marketo-Landingpages
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
TQID: https://experienceleague.adobe.com/scyZfbFBloPu8JRfJiMjm62AFCHM7WCxaats3qssq2A
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 213
ht-degree: 6%

---

# Implementieren von RTP in Marketo-Landingpages {#implementing-rtp-on-marketo-landing-pages}

Um Ihr [!UICONTROL RTP-Tag &#x200B;] implementieren, folgen Sie den folgenden Installationsanweisungen:

1. Navigieren Sie zum **[!UICONTROL Design Studio].** Öffnen Sie das Element, das Sie bearbeiten möchten. Wählen Sie **[!UICONTROL Vorlagenaktionen]** und wählen Sie **[!UICONTROL Entwurf bearbeiten]**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Nehmen Sie die Vorlagenänderungen auf der Registerkarte **HTML Source** vor.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Navigieren Sie in Ihrem RTP-Konto zu **[!UICONTROL Kontoeinstellungen]**.

   a. Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 5 fort.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. Suchen Sie unter [!UICONTROL Domain] die entsprechende Domain und klicken Sie auf **[!UICONTROL Tag generieren]**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Kopieren Sie das RTP-JavaScript-Tag und fügen Sie es zwischen den **`<head> </head>`**-Tags in alle Landingpage-Vorlagen ein.

1. Klicken Sie auf **[!UICONTROL Speichern]** und **[!UICONTROL Schließen]**.

1. Zurück im **[!UICONTROL Design Studio]** genehmigen Sie die Landingpage über **[!UICONTROL Vorlagenaktionen]** und klicken Sie auf **[!UICONTROL Genehmigen]**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Schließlich müssen Sie alle Landingpages, **diese Vorlage verwenden** erneut genehmigen, damit die Vorlagenänderungen wirksam werden. Sie können sie alle gleichzeitig im Hauptabschnitt [!UICONTROL Landingpages“ erneut &#x200B;].

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Vergewissern Sie sich, dass sie auf allen Seiten angezeigt wird, einschließlich Landingpages und Subdomains.

   Klicken Sie dazu mit der rechten Maustaste auf die Seite Ihrer Website. Gehen Sie zu **[!UICONTROL Seite Source anzeigen].** Suchen Sie nach **[!UICONTROL RTP]**, um das Tag zu finden.
