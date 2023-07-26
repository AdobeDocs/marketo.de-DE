---
unique-page-id: 2950561
description: Konversionsskript für benutzerspezifische Ereignisse - Marketo-Dokumente - Produktdokumentation
title: Konversionsskript für benutzerspezifische Ereignisse
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 1%

---

# Konversionsskript für benutzerspezifische Ereignisse {#conversion-script-for-custom-events}

Sie definieren das Erfüllungsziel beim Erstellen eines Verweisangebots. Wenn die Aktion, die auf das Ziel angerechnet wird, ein bestimmtes Ereignis auf Ihrer eigenen Webseite ist, können Sie ein Konversionsskript verwenden, um unsere JavaScript-API aufzurufen.

## Konvertierungsskript abrufen {#retrieve-the-conversion-script}

1. Klicken Sie im Referenzwebenerditor auf **Angebotsdetails** und wählen Sie **JavaScript-Ereignis des Kunden** aus der Dropdown-Liste &quot;Erfüllungsziel&quot;.

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. Kopieren Sie das obere Skript in die graue Kachel und platzieren Sie es auf Ihrer Webseite in der `<body>` Tags. Das untere Skript wird im `<header>` Tags.

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >Denken Sie daran, beide Skripte zu kopieren und einzufügen, wenn sie sich auf einer Nicht-Marketo-Website befinden.

## Loader-Skript abrufen {#retrieve-the-loader-script}

1. Wählen Sie das Verweisangebot aus dem Baum aus und klicken Sie auf **Verweisangebotsaktionen** und **Einbettungscode**.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. Rechtsklicken Sie auf die **Kopfzeilencode** und fügen Sie sie in Ihren Webseitenkopf ein. Führen Sie dann dasselbe für die **Textkörper**.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Einfügen der Skripte in Ihre Webseite {#pasting-the-scripts-onto-your-webpage}

Fügen Sie die Konvertierungsskripte in die HTML für den Hauptteil und die Kopfzeile ein. Platzieren Sie anschließend die Lader-Skripte in die HTML für den Hauptteil und die Kopfzeile.

![](assets/image2015-4-20-21-3a0-3a16.png)

## Verbinden des Konvertierungsskripts {#connecting-the-conversion-script}

Hier schreiben Sie eine JavaScript-Funktion, die die spezifische HTML-ID des Seitenelements verwendet, für das Sie das Trigger-Ziel abschließen möchten. Beispiel:

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

In diesem Beispiel gibt es eine Schaltfläche auf der Webseite mit der ID &quot;#myButtonId&quot;. Wenn auf diese Schaltfläche geklickt wird, wird die Person registriert, als habe sie das Ziel erreicht.

Fantastisch Ihre Website erfasst jetzt benutzerdefinierte Ziele für die Social-Media-Werbung mit Marketo.

>[!MORELIKETHIS]
>
>* [Ziel für Verweisangebot angeben](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [Erstellen eines Verweisangebots](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Social auf Ihrer Website bereitstellen](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)
