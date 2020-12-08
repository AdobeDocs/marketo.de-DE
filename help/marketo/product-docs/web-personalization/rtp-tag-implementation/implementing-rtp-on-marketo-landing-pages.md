---
unique-page-id: 4720151
description: Implementierung von RTP auf Marketing-Landingpages - Marketing Docs - Produktdokumentation
title: Implementierung von RTP zu Marketo-Landingpages
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# Implementierung von RTP zu Marketo-Landingpages {#implementing-rtp-on-marketo-landing-pages}

Befolgen Sie zur Implementierung Ihres RTP-Tags die Installationsanweisungen unten:

1. Gehen Sie zum **Design Studio.** Öffnen Sie das Element, das Sie bearbeiten möchten. Wählen Sie **Vorlagenaktionen** und dann Entwurf **bearbeiten**

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Nehmen Sie die Vorlagenänderungen auf der Registerkarte &quot; **HTML-Quelle** &quot;vor.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Wechseln Sie in Ihrem RTP-Konto zu** Kontoeinstellungen.**

1. Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 5 fort.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. Suchen Sie unter &quot;Domäne&quot;die entsprechende Domäne und klicken Sie auf Tag **generieren**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Kopieren Sie das RTP JavaScript-Tag und fügen Sie es in alle Ihre Vorlagen für Landingpages zwischen den **`<head> </head>`** Tags ein.
1. Klicken Sie auf **Speichern** und **Schließen** des Fensters.
1. Genehmigen Sie in **Design Studio** die Landingpage aus den **Vorlagenaktionen** und klicken Sie auf **Genehmigen**.\
   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Schließlich müssen Sie alle Landingpages, die diese Vorlage verwenden, **erneut genehmigen** , damit die Vorlagenänderungen wirksam werden. Sie können sie alle auf einmal im Hauptabschnitt Landingpages erneut genehmigen.

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Vergewissern Sie sich, dass sie auf allen `pages including` Landingpages und Subdomänen angezeigt wird.

   Dazu klicken Sie mit der rechten Maustaste auf Ihre `website’s` Seite. Zur Seitenquelle **Ansicht gehen.** Suchen Sie nach **RTP** , um das Tag zu suchen.
