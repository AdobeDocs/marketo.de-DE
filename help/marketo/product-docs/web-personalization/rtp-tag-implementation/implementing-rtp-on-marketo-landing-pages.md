---
unique-page-id: 4720151
description: Implementieren von RTP auf Marketo-Landingpages - Marketo Docs - Produktdokumentation
title: Implementieren von RTP auf Marketo-Einstiegsseiten
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Implementieren von RTP auf Marketo-Einstiegsseiten {#implementing-rtp-on-marketo-landing-pages}

Befolgen Sie zur Implementierung Ihres RTP-Tags die folgenden Installationsanweisungen:

1. Navigieren Sie zu **Design Studio.** Öffnen Sie das Element, das Sie bearbeiten möchten. Auswählen **Vorlagenaktionen** auswählen **Entwurf bearbeiten**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Nehmen Sie Ihre Vorlagenänderungen an der **HTML-Source** Registerkarte.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Gehen Sie in Ihrem RTP-Konto zu **Kontoeinstellungen**.

   a. Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 5 fort.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. Suchen Sie unter Domäne die entsprechende Domäne und klicken Sie auf **Tag generieren**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Kopieren Sie das RTP-JavaScript-Tag und fügen Sie es in alle Landingpage-Vorlagen zwischen den **`<head> </head>`** Tags.

1. Klicks **Speichern** und **Schließen** das Fenster.

1. Zurück im **Design Studio** validieren Sie die Landingpage über **Vorlagenaktionen** klicken **Genehmigen**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Schließlich müssen Sie **erneut genehmigen** alle Landingpages, die diese Vorlage verwenden, damit die Vorlagenänderungen wirksam werden. Sie können sie alle gleichzeitig im Hauptabschnitt Einstiegsseiten erneut genehmigen.

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Vergewissern Sie sich, dass sie auf allen Seiten einschließlich Landingpages und Sub-Domains angezeigt wird.

   Klicken Sie dazu mit der rechten Maustaste auf die Seite Ihrer Website. Navigieren Sie zu **Seitenquelle anzeigen.** Suchen Sie nach **RTP** , um das Tag zu finden.
