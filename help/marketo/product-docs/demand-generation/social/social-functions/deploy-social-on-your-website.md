---
unique-page-id: 2950524
description: Social auf Ihrer Website bereitstellen - Marketo-Dokumente - Produktdokumentation
title: Social auf Ihrer Website bereitstellen
exl-id: bccfa461-29c1-4cf1-8e6a-2186c36bdf7e
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Social auf Ihrer Website bereitstellen {#deploy-social-on-your-website}

Betten Sie Social-Apps auf Ihren Nicht-Marketo-Seiten ein.

>[!IMPORTANT]
>
>Am 31. Juli 2024 begannen wir mit der Einstellung dieser Funktion. Neue Assets können nicht mehr erstellt werden. Vorhandene Assets werden bis zum 31. Januar 2025 weiterhin funktionieren. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>Nicht alle Marketo Engage-Benutzer haben diese Funktion erworben. Weitere Informationen erhalten Sie vom Adobe Account Team (Ihrem Kundenbetreuer).

Sie können Social-Apps auf Ihrer eigenen Website bereitstellen, um Ihre Zielgruppe einzubinden und alle Beteiligten in das größere Gespräch in sozialen Netzwerken einzubinden. Wenn Personen Ihre Promotions und Inhalte mit ihren Freunden in sozialen Netzwerken teilen, generieren Sie mehr Traffic auf Ihrer Site.

1. Wählen Sie eine genehmigte Social-App aus, z. B. eine YouTube-Video- oder Social-Schaltfläche.

   ![](assets/image2015-5-12-11-3a43-3a24.png)

1. Wählen Sie **Einbettungscode** aus Social-App-Aktionen aus.

   ![](assets/image2015-5-12-12-3a59-3a46.png)

1. Kopieren Sie den Code für den Seitenkopf (`<head>`) und den Hauptteil (`<body>`) Ihrer Site.

   ![](assets/image2015-5-12-13-3a3-3a34.png)

1. Fügen Sie das erste Codefragment in den Seitenkopf Ihrer Website ein.

   ![](assets/socialonsite-embedhead.png)

1. Fügen Sie das zweite Codefragment in jede Seite ein, auf der Ihre Social-App auf der Seite angezeigt werden soll.

   ![](assets/socialonsite-embedwidget.png)

1. Wenn Sie die Größe der Social-App auf bestimmte Dimensionen auf Ihrer Seite festlegen müssen, fügen Sie die Optionen **outerHeight** und **outerWidth** zum zweiten Codeausschnitt hinzu. Sie können beispielsweise `options='{"outerHeight":400, "outerWidth":600}'` hinzufügen, wie in:

   ![](assets/socialonsite-resizewidget2.png)

   Ihre Marketo Social-App fügt Ihrer Website jetzt Inhalte und Interaktivität hinzu und lädt Fans, Besucher und Bestandskunden dazu ein, das Wort über Sie zu verbreiten. Gleichzeitig werden die Profildaten zu Ihrer Datenbank hinzugefügt und Metriken zu sozialen Einflüssen verfolgt.

   >[!MORELIKETHIS]
   >
   >* [Schaltfläche &quot;Social-App anpassen&quot;](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)
   >* [Anforderung zur Freigabe in sozialen Netzwerken festlegen](/help/marketo/product-docs/demand-generation/social/social-functions/set-social-share-requirement.md)
   >* [Publish-Einstiegsseiten in Facebook](/help/marketo/product-docs/demand-generation/facebook/publish-landing-pages-to-facebook.md)
