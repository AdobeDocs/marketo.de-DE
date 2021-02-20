---
unique-page-id: 11385053
description: JavaScript für Content-AI - Marketing Docs - Produktdokumentation bereitstellen
title: JavaScript für Content-AI bereitstellen
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---


# JavaScript für Content-AI {#deploy-the-javascript-for-content-ai} bereitstellen

Zur Verwendung von Predictive Content müssen Sie das RTP-Tag (Web Personalization) erstellen und einrichten.

## Tag {#generate-tag} erstellen

1. Melden Sie sich bei Ihrem Predictive Content-Konto an. Gehen Sie zu **Kontoeinstellungen**.

   ![](assets/settings-dropdown-account-hands.png)

1. Suchen Sie unter **Domänenkonfiguration** die entsprechende Domäne und klicken Sie auf **Tag** erstellen.

   ![](assets/generate-tag.png)

1. Kopieren Sie das Web-Personalization-Tag und fügen Sie es in den HTML-Code Ihrer Website ein.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Kopieren Sie das JavaScript-Tag &quot;Web-Personalisierung&quot;und fügen Sie es als erstes Skript in die Kopfzeile Ihrer Seiten zwischen den Tags `<head> </head>` ein. Detailliertere [Implementierungsanweisungen finden Sie hier](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

1. Vergewissern Sie sich, dass das Tag auf allen Seiten, einschließlich Landingpages und Subdomänen, angezeigt wird. Überprüfen Sie dies, indem Sie mit der rechten Maustaste auf die Seite Ihrer Website klicken. Gehen Sie in einem Webbrowser zu **Seitenquelle der Ansicht**. Suchen: &quot;RTP&quot;.

1. Vergewissern Sie sich, dass der Tag-Umschalter auf **ON** eingestellt ist.
