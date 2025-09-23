---
unique-page-id: 5472348
description: Kompatibilität einer vorhandenen Freiform-Landingpage-Vorlage herstellen - Marketo-Dokumente - Produktdokumentation
title: Kompatibel machen einer bestehenden Vorlage für Freiform-Landingpages auf Mobilgeräten
exl-id: 942456a5-3f3e-4a71-aecc-4cc6bf6237b3
feature: Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 3%

---

# Erstellen einer vorhandenen Freiform-Landingpage-Vorlage [!UICONTROL Mobile-kompatibel] {#make-an-existing-free-form-landing-page-template-mobile-compatible}

Dies kann an zwei Stellen geschehen, im Vorlagen-Editor und im Landingpage-Editor.

## Aktualisieren aus dem Vorlageneditor {#upgrade-from-the-template-editor}

1. Gehen Sie zum **[!UICONTROL Design Studio]**.

   ![](assets/designstudio-1.png)

1. Wählen Sie **[!UICONTROL Vorlagen]** aus.

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. Wählen Sie eine Vorlage aus **[!UICONTROL bei der „Mobile]**&quot; **[!UICONTROL Nein]** ist.

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. Klicken Sie **[!UICONTROL Entwurf bearbeiten]**.

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. Klicken Sie auf **[!UICONTROL Mobile kompatibel machen]**.

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. Klicken Sie auf **[!UICONTROL Aktualisieren]**.

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   Ihre Landingpage-Vorlage ist jetzt mobil kompatibel!

   >[!NOTE]
   >
   >Ein Upgrade sollte harmlos sein, aber stellen Sie sicher, dass Sie die Seiten auf Diskrepanzen überprüfen. Beim Upgrade werden Entwürfe aller Landingpages erstellt, die diese Vorlage verwenden.

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## Was macht eine Vorlage [!UICONTROL Mobile kompatibel]? {#what-makes-a-template-mobile-compatible}

Gute Fragen! Ihre Vorlage muss über die folgenden Tags verfügen:

`Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV>`

Wenn alles gut aussieht, wirst du diese Nachricht sehen.

![](assets/image2015-1-22-20-3a41-3a31.png)

Wenn ein Fehler auftritt, wird eine Fehlermeldung angezeigt. Klicken Sie auf „Reparieren“, um das Problem zu beheben, und wiederholen Sie den Validierungsprozess.

![](assets/image2015-1-22-20-3a43-3a20.png)

Wenn Sie Änderungen an der Vorlage vornehmen, klicken Sie auf [!UICONTROL Vorlagenaktionen] und wählen Sie [!UICONTROL Kompatibilität mit Mobilgeräten überprüfen].

## Aktualisieren einer Vorlage im Freiform-Landingpage-Editor {#upgrading-a-template-from-the-free-form-landing-page-editor}

Wenn Sie eine Landingpage bearbeiten und auf die Registerkarte Mobile klicken, werden Sie manchmal feststellen, dass die Vorlage nicht aktualisiert wurde. Fürchte dich nicht! Sie können es direkt hier aktualisieren.

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Mobil“.

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. Aktivieren Sie das Kontrollkästchen und klicken Sie auf **[!UICONTROL Aktivieren]**.

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >Durch die Aktivierung der mobilen Version einer Vorlage werden Entwürfe für alle Landingpages erstellt, die diese verwenden.

Fantastisch! Sie können jetzt [die mobile Ansicht](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) aller Landingpages anpassen, die diese Vorlage verwenden.
