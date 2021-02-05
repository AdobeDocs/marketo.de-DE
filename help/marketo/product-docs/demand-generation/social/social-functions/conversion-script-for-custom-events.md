---
unique-page-id: 2950561
description: Konvertierungsskript für benutzerdefinierte Ereignis - Marketing-Dokumente - Produktdokumentation
title: Konvertierungsskript für benutzerdefinierte Ereignis
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Konvertierungsskript für benutzerdefinierte Ereignis {#conversion-script-for-custom-events}

Sie definieren das Fulfillment-Ziel, wenn Sie ein Angebot für eine Verweisung erstellen. Wenn es sich bei der zum Ziel zählenden Aktion um ein bestimmtes Ereignis auf Ihrer eigenen Webseite handelt, können Sie ein Konvertierungsskript verwenden, um unsere JavaScript-API aufzurufen.

## Umrechnungsskript abrufen {#retrieve-the-conversion-script}

1. Klicken Sie im Befassungs-Angebot-Editor auf **Angebot-Details** und wählen Sie **Customer JavaScript-Ereignis** aus der Dropdownliste Fulfillment-Ziel.

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. Kopieren Sie das obere Skript im grauen Feld und platzieren Sie es auf Ihrer Webseite innerhalb der `<body>`-Tags. Das untere Skript wird innerhalb der Tags `<header>` platziert.

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >Denken Sie daran, beide Skripte zu kopieren und einzufügen, wenn sie auf einer Nicht-Marketo-Website laufen.

## Loader Script abrufen {#retrieve-the-loader-script}

1. Wählen Sie in der Struktur das Referrer-Angebot aus und klicken Sie dann auf **Referrer-Angebot-Aktionen** und **Einbettungscode**.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. Klicken Sie mit der rechten Maustaste auf den **Kopfzeilencode** und fügen Sie ihn in die Kopfzeile Ihrer Webseite ein. Führen Sie dann dasselbe für **Body Code** aus.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Einfügen der Skripten auf Ihrer Webseite {#pasting-the-scripts-onto-your-webpage}

Fügen Sie die Konvertierungsskripte in den HTML-Code für den Text und die Kopfzeile ein. Platzieren Sie anschließend die Loader-Skripten in den HTML-Code für den Text und die Kopfzeile.

![](assets/image2015-4-20-21-3a0-3a16.png)

## Verbinden des Konvertierungsskripts {#connecting-the-conversion-script}

Hier schreiben Sie eine JavaScript-Funktion, die die spezifische HTML-ID jedes Seitenelements verwendet, bei dem das Trigger abgeschlossen werden soll. Beispiel:

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

In diesem Beispiel gibt es eine Schaltfläche auf der Webseite mit der ID &quot;#myButtonId&quot;. Wenn auf diese Schaltfläche geklickt wird, wird die Person registriert, als habe sie das Ziel erreicht.

Fantastisch! Ihre Website erfasst jetzt mit Marketo benutzerdefinierte Ziele sozialer Werbung.

>[!MORELIKETHIS]
>
>* [Angebot für Verweis angeben](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [Erstellen eines Referrer-Angebots](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Social auf Ihrer Website bereitstellen](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)

