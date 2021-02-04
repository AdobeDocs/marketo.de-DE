---
unique-page-id: 5472348
description: Vorhandene Vorlage für eine Landingpage mit Freiform Mobile kompatibel machen - Marketing Docs - Produktdokumentation
title: Vorhandene Vorlage für eine Landingpage mit Freiform Mobile kompatibel machen
translation-type: tm+mt
source-git-commit: 2969e6f94f5fd781e2167ae2aa8680bb8d134754
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---


# Vorhandene Vorlage für eine Landingpage mit Freiform mit Mobilgeräten kompatibel machen {#make-an-existing-free-form-landing-page-template-mobile-compatible}

Dies kann an zwei Stellen erfolgen: dem Vorlageneditor und dem Landingpages-Editor.

## Aktualisierung vom Vorlageneditor {#upgrade-from-the-template-editor}

1. Wechseln Sie zu **Design Studio**.

   ![](assets/designstudio-1.png)

1. Wählen Sie **Vorlagen**.

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. Wählen Sie eine Vorlage aus, bei der **Mobil kompatibel** **Nein** ist.

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. Klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. Klicken Sie auf **Mobil kompatibel machen**.

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. Klicken Sie auf **Upgrade**.

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   Ihre Vorlage für die Landingpage ist jetzt mit Mobilgeräten kompatibel!

   >[!NOTE]
   >
   >Die Aktualisierung sollte harmlos sein, aber achten Sie darauf, die Seiten auf eventuelle Diskrepanzen zu überprüfen. Durch eine Aktualisierung werden Entwürfe aller Landingpages erstellt, die diese Vorlage verwenden.

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## Was macht eine Vorlage für Mobilgeräte kompatibel? {#what-makes-a-template-mobile-compatible}

Große Fragen! Ihre Vorlage muss die folgenden Tags aufweisen:

`<pre data-theme="Confluence">Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV></pre>`

Wenn alles gut aussieht, sehen Sie diese Nachricht.

![](assets/image2015-1-22-20-3a41-3a31.png)

Wenn ein Fehler auftritt, wird eine Fehlermeldung angezeigt. Klicken Sie auf &quot;Reparieren&quot;, um das Problem zu beheben, und wiederholen Sie den Validierungsprozess.

![](assets/image2015-1-22-20-3a43-3a20.png)

Wenn Sie Änderungen an der Vorlage vornehmen, klicken Sie auf Vorlagenaktionen und wählen Sie Mobilkompatibilität überprüfen.

## Aktualisieren einer Vorlage aus dem Editor für kostenlose Landingpages {#upgrading-a-template-from-the-free-form-landing-page-editor}

Wenn Sie eine Landingpage bearbeiten und auf die Registerkarte &quot;Mobil&quot;klicken, werden Sie mitunter bemerken, dass die Vorlage nicht aktualisiert wurde. Furcht nicht! Sie können es hier aktualisieren.

1. Klicken Sie auf die Registerkarte **Mobil**.

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. Aktivieren Sie das Kontrollkästchen und klicken Sie auf **Aktivieren**.

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >Wenn Sie die mobile Version einer Vorlage aktivieren, werden Entwürfe aller Landingpages erstellt, die diese verwenden.

Fantastisch! Sie können jetzt [die mobile Ansicht](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) aller Landingpages anpassen, die diese Vorlage verwenden.
