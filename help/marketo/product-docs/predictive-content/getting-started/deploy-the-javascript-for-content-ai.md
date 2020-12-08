---
unique-page-id: 11385053
description: JavaScript für Content-AI - Marketing Docs - Produktdokumentation bereitstellen
title: JavaScript für Content-AI bereitstellen
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# JavaScript für Content-AI bereitstellen {#deploy-the-javascript-for-content-ai}

>[!NOTE]
>
>Je nach Kaufdatum kann Ihr Marketing-Abonnement entweder Marketing-to-Predictive-Inhalte oder Inhalte`<sup>AI</sup>`enthalten. Für Personen, die Predictive Content verwenden, aktiviert Marketing bis zum 30. April 2018 Content`<sup>AI</sup>` Analytics-Funktionen. Wenden Sie sich an Ihren Marketing-Kundenbetreuer, um ein Upgrade auf Marketing-Inhalte`<sup>AI</sup>`durchzuführen, damit diese Funktionen über das entsprechende Datum hinausgehen.

Zur Verwendung von Predictive Content müssen Sie Ihr RTP (Web Personalization) erstellen und einrichten `tag.`

## Tag erstellen {#generate-tag}

1. Melden Sie sich bei Ihrem Predictive Content-Konto an. Wechseln Sie zu **Kontoeinstellungen**.

   ![](assets/settings-dropdown-account-hands.png)

1. Suchen Sie in der **Domänenkonfiguration** die entsprechende Domäne und klicken Sie auf Tag **generieren.**

   ![](assets/generate-tag.png)

1. Kopieren Sie das Web-Personalization-Tag und fügen Sie es in den HTML-Code Ihrer Website ein.

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Kopieren Sie das JavaScript-Tag &quot;Web-Personalisierung&quot;und fügen Sie es als erstes Skript in die Kopfzeile Ihrer Seiten zwischen den `<head> </head>` Tags ein. Detailliertere [Implementierungsanweisungen finden Sie hier](http://docs.marketo.com/display/docs/rtp+tag+implementation)[.](http://pages2.marketo.com/rtp-implementation.html)

1. Vergewissern Sie sich, dass das Tag auf allen Seiten, einschließlich Landingpages und Subdomänen, angezeigt wird. Überprüfen Sie dies, indem Sie mit der rechten Maustaste auf Ihre `website’s` Seite klicken. Wechseln Sie in einem Webbrowser zur **Seitenquelle** der Ansicht. Suchen: &quot;RTP&quot;.
1. Vergewissern Sie sich, dass der Tag-Umschalter auf **EIN** eingestellt ist.

