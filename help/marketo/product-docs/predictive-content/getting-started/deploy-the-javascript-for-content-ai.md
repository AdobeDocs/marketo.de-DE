---
unique-page-id: 11385053
description: Bereitstellen von JavaScript für Content-AI - Marketo Docs - Produktdokumentation
title: JavaScript für Content-AI bereitstellen
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 1%

---

# JavaScript für Content-AI bereitstellen {#deploy-the-javascript-for-content-ai}

Zur Verwendung von Predictive Content müssen Sie das RTP (Web Personalization)-Tag generieren und einrichten.

## Tag generieren {#generate-tag}

1. Melden Sie sich bei Ihrem Predictive Content-Konto an. Wechseln Sie zu **Kontoeinstellungen**.

   ![](assets/settings-dropdown-account-hands.png)

1. Suchen Sie in **Domänenkonfiguration** die entsprechende Domäne und klicken Sie auf **Tag generieren**.

   ![](assets/generate-tag.png)

1. Kopieren Sie das Web Personalization-Tag und fügen Sie es in die HTML Ihrer Website ein.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Kopieren Sie das Tag Web Personalization JavaScript und fügen Sie es als erstes Skript in die Kopfzeile Ihrer Seiten zwischen den Tags `<head> </head>` ein. Detailliertere [Implementierungsanweisungen finden Sie hier](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Überprüfen Sie, ob das Tag auf allen Seiten angezeigt wird, einschließlich Landingpages und Subdomänen. Klicken Sie mit der rechten Maustaste auf die Seite Ihrer Website. Navigieren Sie in einem Webbrowser zu **Seite Source anzeigen** . Suche: &quot;RTP&quot;.

1. Vergewissern Sie sich, dass der Umschalter Tag auf **ON** gesetzt ist.
