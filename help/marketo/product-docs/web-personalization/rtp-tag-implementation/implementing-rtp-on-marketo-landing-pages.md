---
unique-page-id: 4720151
description: Implementieren von RTP auf Marketo-Landingpages - Marketo-Dokumente - Produktdokumentation
title: Implementieren von RTP auf Marketo-Landingpages
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Implementieren von RTP auf Marketo-Landingpages {#implementing-rtp-on-marketo-landing-pages}

Um Ihr [!UICONTROL RTP-Tag &#x200B;] implementieren, folgen Sie den folgenden Installationsanweisungen:

1. Gehen Sie zum **[!UICONTROL Design Studio].** Öffnen Sie das Element, das Sie bearbeiten möchten. Wählen Sie **[!UICONTROL Vorlagenaktionen]** und wählen Sie **[!UICONTROL Entwurf bearbeiten]**.

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

   Klicken Sie dazu mit der rechten Maustaste auf die Seite Ihrer Website. Navigieren Sie **[!UICONTROL Seite Source anzeigen].** Suchen Sie nach **[!UICONTROL RTP]**, um das Tag zu finden.
