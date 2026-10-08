---
solution: Marketo Engage
product: marketo
title: Bearbeiten von E-Mail-Vorlagen mit dem erweiterten HTML-Editor
description: Erfahren Sie, wie Sie den rohen HTML-Quell-Code in der Marketo Engage E-Mail-Designer anzeigen und bearbeiten, einschließlich Leitplanken, Zugriffsschritten und wichtigen Einschränkungen.
level: Intermediate
feature: Email Designer
exl-id: b030e56a-de70-4b0d-9788-04a01235cffb
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: f8f7d99a-f455-45bb-8028-428a55a7130b
    internal-label: Email Designer
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 49%
---
# Bearbeiten von E-Mail-Vorlagen mit dem erweiterten HTML-Editor {#advanced-html-mode}

Im erweiterten HTML-Modus können Sie den Roh-Quell-Code von E-Mail-Vorlagen direkt über die [!DNL Marketo Engage] E-Mail-Designer-Benutzeroberfläche anzeigen und bearbeiten.

Mit dieser Funktion können Sie erweiterte Ausdrücke direkt in die Quelle einfügen. Wenn Sie zur visuellen Ansicht (Desktop) zurückkehren, wird der Inhalt erneut gerendert, damit Sie überprüfen können, wie er aussieht, und die Bearbeitung in jeder Ansicht fortsetzen können.

## Schutzmechanismen {#guardrails}

Wenn Sie den erweiterten HTML-Editor verwenden, sorgen die folgenden Schutzmechanismen für die Kompatibilität der Inhalte und legen die Erwartungen fest.

* Der erweiterte HTML-Editor **validiert Ihren Code nicht**. Syntaxfehler oder fehlerhafte Layouts werden nicht geprüft. Überprüfen Sie Ihre Inhalte sorgfältig, bevor Sie sie speichern.

* Zukünftige Systemaktualisierungen können Änderungen überschreiben, die Sie am Standard-Markup vornehmen. **Ihre Änderungen werden möglicherweise nicht beibehalten**.

* [!DNL Adobe] Support **kann Probleme nicht beheben oder**), die durch benutzerdefinierten Code und manuelle Änderungen verursacht werden. Erstellen Sie eine Sicherungskopie Ihres Inhalts, für den Fall, dass Sie ihn wiederherstellen müssen.

* In der erweiterten HTML-Ansicht können keine Inhalte simuliert werden. Zur Desktop-Ansicht wechseln, um eine Vorschau des Inhalts anzuzeigen.

* Um die Inhaltskompatibilität sicherzustellen, können Sie **nicht** in der erweiterten HTML-Ansicht speichern. Wechseln Sie zurück zur Desktop-Ansicht, wenn Sie zum Speichern Ihrer Änderungen bereit sind.

## Zugriff auf den erweiterten HTML-Modus {#access-html-mode}

Gehen Sie wie folgt vor, um den erweiterten HTML-Editor zu öffnen und Ihre Vorlagenquelle zu bearbeiten.

1. Öffnen oder [Erstellen einer E-Mail](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#create-an-email-template)Vorlage in der E-Mail-Designer.

1. Klicken Sie _Bildschirm „E_ Mail-Vorlage bearbeiten“ oben rechts auf die Schaltfläche HTML .

   ![](assets/advanced-html-mode-1.png){width="800" zoomable="yes"}

1. Beim ersten Öffnen des erweiterten HTML-Editors wird eine Warnmeldung angezeigt. Klicken Sie abschließend **[!UICONTROL OK]**.

   ![](assets/advanced-html-mode-2.png)

   >[!NOTE]
   >
   >Diese Warnung wird angezeigt, wenn Sie den erweiterten HTML-Editor zum ersten Mal öffnen und monatlich zurücksetzen.

1. Der erweiterte HTML-Editor wird angezeigt.

   ![](assets/advanced-html-mode-3.png){width="800" zoomable="yes"}

1. Fügen Sie die gewünschten Änderungen an Ihrem E-Mail-Inhalt hinzu.

   >[!WARNING]
   >
   >Stellen Sie sicher, dass Sie den richtigen HTML- und CSS-Code eingeben, da es keinen Syntaxvalidierungsprozess gibt und der Adobe-Support bei HTML-Bearbeitungen nicht behilflich sein kann.

1. Inhaltssimulation und -speicherung sind in der erweiterten HTML-Ansicht aus Kompatibilitätsgründen nicht verfügbar. Wechseln Sie zurück zur Desktop-Ansicht, um eine Vorschau Ihres Inhalts anzuzeigen und Ihre Änderungen zu speichern.

   ![](assets/advanced-html-mode-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >Ihre Bearbeitungen bleiben beim Wechseln der Ansichten erhalten.
