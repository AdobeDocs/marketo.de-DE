---
unique-page-id: 11385053
description: Bereitstellen von JavaScript für Content-AI - Marketo Docs - Produktdokumentation
title: Bereitstellen von JavaScript für Content-AI
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 1%

---

# Bereitstellen von JavaScript für Content-AI {#deploy-the-javascript-for-content-ai}

Zur Verwendung von Predictive Content müssen Sie das RTP-Tag (Web Personalization) generieren und einrichten.

## Tag generieren {#generate-tag}

1. Melden Sie sich bei Ihrem Predictive Content-Konto an. Navigieren Sie zu **Kontoeinstellungen**.

   ![](assets/settings-dropdown-account-hands.png)

1. In **Domänenkonfiguration**, suchen Sie die entsprechende Domäne und klicken Sie auf **Tag generieren**.

   ![](assets/generate-tag.png)

1. Kopieren Sie das Tag Web-Personalisierung und fügen Sie es in die HTML Ihrer Website ein.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Kopieren Sie das JavaScript-Tag Web-Personalisierung und fügen Sie es als erstes Skript in die Kopfzeile Ihrer Seiten zwischen dem `<head> </head>` Tags. Weitere Informationen [Implementierungsanweisungen hier](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Überprüfen Sie, ob das Tag auf allen Seiten angezeigt wird, einschließlich Landingpages und Subdomänen. Klicken Sie mit der rechten Maustaste auf die Seite Ihrer Website. Navigieren Sie zu **Seitenquelle anzeigen** in einem Webbrowser. Suchen: &quot;RTP&quot;.

1. Vergewissern Sie sich, dass der Umschalter Tag auf **ON**.
