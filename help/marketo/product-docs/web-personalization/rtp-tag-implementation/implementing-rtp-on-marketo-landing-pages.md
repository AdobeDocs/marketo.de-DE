---
unique-page-id: 4720151
description: Implementieren von RTP auf Marketo-Landingpages - Marketo Docs - Produktdokumentation
title: Implementieren von RTP auf Marketo-Einstiegsseiten
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Implementieren von RTP auf Marketo-Einstiegsseiten {#implementing-rtp-on-marketo-landing-pages}

Befolgen Sie zur Implementierung Ihres RTP-Tags die folgenden Installationsanweisungen:

1. Wechseln Sie zu **Design Studio.** Öffnen Sie das Element, das Sie bearbeiten möchten. Wählen Sie **Vorlagenaktionen** und dann **Entwurf bearbeiten** aus.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Nehmen Sie Ihre Vorlagenänderungen auf der Registerkarte **HTML Source** vor.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Wechseln Sie in Ihrem RTP-Konto zu **Kontoeinstellungen**.

   a. Wenn Sie Ihr JavaScript-Tag bereits vom Support erhalten haben, fahren Sie mit Schritt 5 fort.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. Suchen Sie unter &quot;Domäne&quot;die entsprechende Domäne und klicken Sie auf **Tag generieren**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Kopieren Sie das RTP JavaScript -Tag und fügen Sie es zwischen den **`<head> </head>`** -Tags in alle Landingpage-Vorlagen ein.

1. Klicken Sie auf **Speichern** und **Schließen** im Fenster.

1. Genehmigen Sie in **Design Studio** die Landingpage über **Vorlagenaktionen** und klicken Sie auf **Genehmigen**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Schließlich müssen Sie alle Landingpages, die diese Vorlage verwenden, **erneut genehmigen**, damit die Vorlagenänderungen wirksam werden. Sie können sie alle gleichzeitig im Hauptabschnitt Einstiegsseiten erneut genehmigen.

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Vergewissern Sie sich, dass sie auf allen Seiten einschließlich Landingpages und Sub-Domains angezeigt wird.

   Klicken Sie dazu mit der rechten Maustaste auf die Seite Ihrer Website. Navigieren Sie zu **Seite Source anzeigen .** Suchen Sie nach **RTP** , um das Tag zu finden.
