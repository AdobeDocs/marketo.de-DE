---
unique-page-id: 2950617
description: Verwenden dynamischer Inhalte in einer E-Mail - Marketo-Dokumente - Produktdokumentation
title: Verwenden dynamischer Inhalte in einer E-Mail
exl-id: a1178f76-6760-4a4a-9510-f129ee6a9032
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Verwenden dynamischer Inhalte in einer E-Mail {#using-dynamic-content-in-an-email}

>[!PREREQUISITES]
>
>[Erstellen einer Segmentierung](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

Verwenden Sie dynamische Inhalte in E-Mails, um Ihre Interessenten-Targeting-Informationen zu senden.

>[!NOTE]
>
>Die Verwendung von Variablen in dynamischen Inhalten in einer E-Mail wird nur bei der Verwendung von Trigger-Kampagnen unterstützt. Es ist **not** wird bei der Verwendung von Batch-Kampagnen unterstützt.

## Segmentierung hinzufügen {#add-segmentation}

1. Navigieren Sie zu **Marketingaktivitäten**.

   ![](assets/login-marketing-activities.png)

1. E-Mail auswählen und auf **Entwurf bearbeiten**.

   ![](assets/1.2.png)

1. In diesem Beispiel machen wir die Betreffzeile dynamisch. Klicken Sie in das Feld Betreff und dann auf das **Dynamisch machen** Schaltfläche.

   ![](assets/1.3.png)

   >[!NOTE]
   >
   >Sie können auch ein Element innerhalb der E-Mail dynamisch gestalten. Wählen Sie dazu den Bereich aus, klicken Sie auf das Zahnradsymbol und wählen Sie **Dynamisch machen** (oder [Ersetzen durch Snippet](/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md), je nachdem, was Sie tun).

1. Geben Sie den Segmentierungsnamen ein, wählen Sie ihn aus und klicken Sie auf **Speichern**.

   ![](assets/1.4.png)

   Ihre Segmentierung und ihre Segmente werden rechts auf der Registerkarte Dynamisch angezeigt.

   ![](assets/1.5.png)

## Dynamische Inhalte anwenden {#apply-dynamic-content}

>[!CAUTION]
>
>Die zulässige Anzahl von dynamischen Inhaltselementen ist nicht unbegrenzt. Auch wenn es keine bestimmte Anzahl von E-Mails gibt (diese können je nach Inhaltskombination variieren), kann die Überverwendung dynamischer Inhalte die Leistung der E-Mail beeinträchtigen. Es wird empfohlen, die Anzahl der dynamischen Inhaltselemente, die pro E-Mail verwendet werden, unter 20 zu halten.

1. Klicken Sie auf Ihre Segmente und fügen Sie Ihre Betreffzeile hinzu.

![](assets/2.1.png)

1. Wiederholen Sie diesen Vorgang für jedes Segment.

   ![](assets/2.2.png)

>[!TIP]
>
>Erstellen Sie eine Standard-E-Mail, bevor Sie Inhalte auf die verschiedenen Segmente anwenden.

>[!CAUTION]
>
>Änderungen am Inhaltsbaustein für Standardsegmente werden auf alle Segmente angewendet.

Süß! Jetzt können Sie flexible E-Mails an Ihre Zielgruppe senden.

>[!MORELIKETHIS]
>
>* [Vorschau einer E-Mail mit dynamischem Inhalt](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md)
>* [Dynamische Inhalte in einer Landingpage verwenden](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/use-dynamic-content-in-a-free-form-landing-page.md)
