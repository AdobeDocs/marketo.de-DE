---
unique-page-id: 5472348
description: Vorhandene Freiform-Landingpage-Vorlage für Mobilgeräte kompatibel machen - Marketo Docs - Produktdokumentation
title: Vorhandene Freiform-Landingpage-Vorlage für Mobilgeräte kompatibel machen
exl-id: 942456a5-3f3e-4a71-aecc-4cc6bf6237b3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---

# Vorhandene Freiform-Landingpage-Vorlage für Mobilgeräte kompatibel machen {#make-an-existing-free-form-landing-page-template-mobile-compatible}

Dies kann an zwei Stellen erfolgen: im Vorlagen-Editor und im Landingpage-Editor.

## Aktualisierung vom Vorlagen-Editor {#upgrade-from-the-template-editor}

1. Navigieren Sie zu **Design Studio**.

   ![](assets/designstudio-1.png)

1. Auswählen **Vorlagen**.

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. Wählen Sie eine Vorlage aus, in der **Kompatibel mit Mobilgeräten** is **Nein**.

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. Klicken **Entwurf bearbeiten**.

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. Klicken **Kompatibel mit Mobilgeräten**.

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. Klicken **Upgrade**.

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   Ihre Landingpage-Vorlage ist jetzt mit Mobilgeräten kompatibel!

   >[!NOTE]
   >
   >Die Aktualisierung sollte harmlos sein. Achten Sie jedoch darauf, die Seiten auf Abweichungen zu überprüfen. Durch die Aktualisierung werden Entwürfe von Landingpages erstellt, die diese Vorlage verwenden.

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## Was macht eine Vorlage für Mobilgeräte kompatibel? {#what-makes-a-template-mobile-compatible}

Große Fragen! Ihre Vorlage muss die folgenden Tags aufweisen:

`<pre data-theme="Confluence">Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV></pre>`

Wenn alles gut aussieht, wirst du diese Nachricht sehen.

![](assets/image2015-1-22-20-3a41-3a31.png)

Wenn etwas nicht stimmt, wird eine Fehlermeldung angezeigt. Klicken Sie auf &quot;Reparieren&quot;, um das Problem zu beheben, und wiederholen Sie den Validierungsprozess.

![](assets/image2015-1-22-20-3a43-3a20.png)

Wenn Sie Änderungen an der Vorlage vornehmen, klicken Sie auf Vorlagenaktionen und wählen Sie &quot;Mobile Kompatibilität überprüfen&quot;.

## Aktualisieren einer Vorlage über den Freiform-Landingpage-Editor {#upgrading-a-template-from-the-free-form-landing-page-editor}

Wenn Sie eine Landingpage bearbeiten und auf die Registerkarte &quot;Mobil&quot;klicken, werden Sie manchmal feststellen, dass die Vorlage nicht aktualisiert wurde. Keine Angst! Sie können es direkt dort aktualisieren.

1. Klicken Sie auf **Mobile** Registerkarte.

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. Klicken Sie auf das Kontrollkästchen und klicken Sie auf **Aktivieren**.

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >Durch die Aktivierung der mobilen Version einer Vorlage werden Entwürfe von Landingpages erstellt, die diese verwenden.

Fantastisch Sie können jetzt [Mobile-Ansicht anpassen](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) aller Landingpages, die diese Vorlage verwenden.
