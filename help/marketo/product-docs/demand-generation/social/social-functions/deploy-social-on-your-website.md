---
unique-page-id: 2950524
description: Bereitstellen von Social Media auf Ihrer Website - Marketo-Dokumente - Produktdokumentation
title: Bereitstellen von Social Media auf Ihrer Website
exl-id: bccfa461-29c1-4cf1-8e6a-2186c36bdf7e
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Bereitstellen von Social Media auf Ihrer Website {#deploy-social-on-your-website}

Einbetten von Social-Media-Apps in Nicht-Marketo-Seiten.

>[!IMPORTANT]
>
>Am 31. Juli 2024 haben wir mit der Einstellung dieser Funktion begonnen. Neue Assets können nicht mehr erstellt werden. Vorhandene Assets funktionieren bis zum 31. Januar 2025 weiterhin. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>Nicht alle Marketo Engage-Benutzer haben diese Funktion erworben. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).

Sie können Social-Media-Apps auf Ihrer eigenen Website bereitstellen, um Ihr Publikum anzusprechen und alle Personen in die größeren Konversationen in den sozialen Netzwerken einzubinden. Wenn Personen Ihre Angebote und Inhalte in sozialen Netzwerken mit ihren Freunden teilen, generieren Sie mehr Traffic auf Ihrer Site.

1. Wählen Sie eine genehmigte Social-Media-App aus, z. B. ein YouTube-Video oder eine Social-Media-Schaltfläche.

   ![](assets/image2015-5-12-11-3a43-3a24.png)

1. Wählen Sie **Einbettungs-Code** aus Social-App-Aktionen aus.

   ![](assets/image2015-5-12-12-3a59-3a46.png)

1. Kopieren Sie den Code für die Seitenkopfzeile (`<head>`) und den Hauptteil (`<body>`) Ihrer Site.

   ![](assets/image2015-5-12-13-3a3-3a34.png)

1. Fügen Sie das erste Codefragment in die Kopfzeile Ihrer Website ein.

   ![](assets/socialonsite-embedhead.png)

1. Fügen Sie das zweite Code-Fragment in jede Seite ein, auf der Ihre Social-Media-App auf der Seite angezeigt werden soll.

   ![](assets/socialonsite-embedwidget.png)

1. Wenn Sie die Größe der Social-App auf bestimmte Dimensionen auf Ihrer Seite festlegen müssen, fügen Sie die Optionen **outerHeight** und **outerWidth** zum zweiten Codeausschnitt hinzu. Sie können beispielsweise `options='{"outerHeight":400, "outerWidth":600}'` hinzufügen, wie in:

   ![](assets/socialonsite-resizewidget2.png)

   Ihre Marketo Social-App fügt Ihrer Website jetzt Inhalte und Interaktivität hinzu und lädt Fans, Besucher und Bestandskunden ein, über Sie zu informieren. Gleichzeitig werden die Profildaten zu Ihrer Datenbank hinzugefügt und Metriken zum sozialen Einfluss verfolgt.

   >[!MORELIKETHIS]
   >
   >* [Schaltfläche „Social-App anpassen](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)
   >* [Anforderung für Social Share festlegen](/help/marketo/product-docs/demand-generation/social/social-functions/set-social-share-requirement.md)
   >* [Publish-Landingpages in Facebook](/help/marketo/product-docs/demand-generation/facebook/publish-landing-pages-to-facebook.md)
