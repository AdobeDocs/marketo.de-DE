---
unique-page-id: 2950561
description: Konversionsskript für benutzerspezifische Ereignisse - Marketo-Dokumente - Produktdokumentation
title: Konvertierungsskript für benutzerdefinierte Ereignisse
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 1%

---

# Konvertierungsskript für benutzerdefinierte Ereignisse {#conversion-script-for-custom-events}

Sie definieren das Erfüllungsziel beim Erstellen eines Empfehlungsangebots. Wenn die Aktion, die für das Ziel zählt, ein bestimmtes Ereignis auf Ihrer eigenen Web-Seite ist, können Sie ein Konversionsskript verwenden, um unsere JavaScript-API aufzurufen.

>[!IMPORTANT]
>
>Am 31. Juli 2024 haben wir mit der Einstellung dieser Funktion begonnen. Neue Assets können nicht mehr erstellt werden. Vorhandene Assets funktionieren bis zum 31. Januar 2025 weiterhin. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## Abrufen des Konvertierungsskripts {#retrieve-the-conversion-script}

1. Klicken Sie im Editor für Empfehlungsangebote auf **Angebotsdetails** und wählen Sie dann **Customer JavaScript Event** aus der Dropdown-Liste „Erfüllungsziel“ aus.

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. Kopieren Sie das Top-Skript in das graue Feld und platzieren Sie es auf Ihrer Web-Seite innerhalb der `<body>` Tags. Das untere Skript wird innerhalb der `<header>` Tags platziert.

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >Denken Sie daran, beide Skripte zu kopieren und einzufügen, wenn sie auf einer Nicht-Marketo-Website verwendet werden.

## Loader-Skript abrufen {#retrieve-the-loader-script}

1. Wählen Sie das Empfehlungsangebot aus der Baumstruktur aus und klicken Sie dann auf **Verweisangebotsaktionen** und **Einbettungs-Code**.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. Klicken Sie mit der rechten Maustaste auf **Kopfzeilen-Code** und fügen Sie ihn in die Kopfzeile Ihrer Web-Seite ein. Führen Sie dann dasselbe für den **Textkörper-Code** aus.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Einfügen der Skripte auf Ihrer Web-Seite {#pasting-the-scripts-onto-your-webpage}

Fügen Sie die Konvertierungsskripte für den Hauptteil und die Kopfzeile in die HTML ein. Platzieren Sie als Nächstes die Laderskripte in der HTML für den Hauptteil und die Kopfzeile.

![](assets/image2015-4-20-21-3a0-3a16.png)

## Verbinden des Konvertierungsskripts {#connecting-the-conversion-script}

Hier schreiben Sie eine JavaScript-Funktion, die die spezifische HTML-ID des Seitenelements verwendet, für das Sie einen Trigger zum Abschluss des Ziels erstellen möchten. Beispiel:

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

In diesem Beispiel befindet sich eine Schaltfläche auf der Web-Seite mit der ID &quot;#myButtonId“. Wenn auf diese Schaltfläche geklickt wird, wird die Person registriert, die das Ziel erreicht hat.

Fantastisch! Ihre Website erfasst jetzt benutzerdefinierte Social-Media-Werbeziele mit Marketo.

>[!MORELIKETHIS]
>
>* [Ziel für Empfehlungsangebot angeben](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [Erstellen eines Empfehlungsangebots](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Bereitstellen von Social Media auf Ihrer Website](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)
