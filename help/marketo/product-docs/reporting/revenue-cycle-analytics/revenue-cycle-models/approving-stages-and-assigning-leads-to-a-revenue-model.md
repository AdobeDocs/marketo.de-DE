---
unique-page-id: 4718683
description: Genehmigen von Phasen und Zuweisen von Leads zu einem Umsatzmodell - Marketo-Dokumente - Produktdokumentation
title: Genehmigen von Phasen und Zuweisen von Leads zu einem Umsatzmodell
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# Genehmigen von Phasen und Zuweisen von Leads zu einem Umsatzmodell {#approving-stages-and-assigning-leads-to-a-revenue-model}

Starten Sie Ihr **Umsatzmodell** indem Sie vorhandene Leads hinzufügen und Zuweisungsregeln für neue Leads erstellen.

## Stadien werden genehmigt {#approving-stages}

Genehmigen wir die Phasen Ihres Modells, bevor Sie Leads hinzufügen.

1. Wechseln Sie zum Bereich **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Wählen Sie das Modell aus, dessen Stadien Sie genehmigen möchten.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. Wählen **unter &quot;**&quot; die Option **Phasen genehmigen**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Sie werden mit einem Warnhinweis begrüßt. Klicken Sie auf **Leads zuweisen**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

Ausgezeichnet! Fahren wir fort und weisen wir diese Leads zu.

## Zuweisen vorhandener Leads {#assigning-existing-leads}

[Erstellen Sie eine Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md), um die Leads für einen Schritt Ihres Modells in Ihrer Lead-Datenbank zu identifizieren.

1. Nachdem Sie [Smart-Liste erstellt haben](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) klicken Sie auf die Registerkarte **Leads**.

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Klicken Sie **Alle auswählen** um die Leads auszuwählen.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Öffnen Sie **Dropdown-Liste** Lead-Aktionen“ und wählen Sie &quot;**&quot;**. Klicken Sie **Umsatzschritt ändern**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Wählen Sie das richtige **Modell** und das richtige **Staging** aus. Klicken Sie **Jetzt ausführen**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Wiederholen Sie den Vorgang, bis alle Leads den verschiedenen Phasen des Modells zugewiesen sind.

Sehr gut! Um festzulegen, wie neue Leads den Phasen zugewiesen werden, erstellen Sie Zuweisungsregeln.

>[!NOTE]
>
>Wenn sich Ihr Modell im Status Genehmigte Stadien befindet, werden in den Aktivitätsprotokollen der Leads keine Ereignisse vom Typ Änderungsumsatz-Stadium angezeigt. Wenn Ihr Modell vollständig genehmigt ist, wird dieser Flussschritt übersprungen, wenn Sie einen Lead in das Stadium verschieben, in dem er sich derzeit befindet.

## Neue Leads: Zuweisungsregeln erstellen  {#new-leads-create-assignment-rules}

1. Klicken Sie erneut auf **Marketo** Startseite und wählen Sie dann **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Klicken Sie in der Baumstruktur auf Ihr Modell und anschließend auf **Menü** Modellaktionen“, wobei Sie **Zuweisungsregeln** auswählen.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. Wenn Ihre Zuweisungsregeln mehr als nur eine Standardauswahl enthalten, klicken Sie auf **Staging**, treffen Sie Ihre Auswahl und klicken Sie dann auf **Auswahl hinzufügen**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Beispiel für eine Zuweisungsregel {#example-assignment-rule}

Erstellen Sie eine Regel für die Lead-Bewertung , um die neuen Leads mit einer Mindestpunktzahl einem entsprechenden Schritt zuzuweisen.

1. Wählen **unter „Wenn** die Option **Lead-Bewertung**. Wählen Sie dann **Mindestens** aus.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. Geben Sie **40** in das Feld ein und wählen Sie **Vertriebs-Lead** als Stufe aus. Klicken Sie **Speichern**, um den Vorgang abzuschließen.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Um Ihr Modell zu genehmigen, lesen Sie unsere Hilfeseite unter **[Genehmigen und Rückgängigmachen der Genehmigung eines Umsatzmodells](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
