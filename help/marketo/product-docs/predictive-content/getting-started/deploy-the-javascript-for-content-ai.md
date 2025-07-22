---
unique-page-id: 11385053
description: Bereitstellen der JavaScript für Content-KI - Marketo-Dokumente - Produktdokumentation
title: Bereitstellen des JavaScript für Content-AI
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 1%

---

# Bereitstellen des JavaScript für Content-AI {#deploy-the-javascript-for-content-ai}

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
