---
unique-page-id: 4718683
description: Genehmigen von Phasen und Zuweisen von Leads zu einem Umsatzmodell - Marketo Docs - Produktdokumentation
title: Genehmigen von Phasen und Zuweisen von Leads zu einem Umsatzmodell
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# Genehmigen von Phasen und Zuweisen von Leads zu einem Umsatzmodell {#approving-stages-and-assigning-leads-to-a-revenue-model}

Erstellen Sie Ihr **Umsatzmodell**, indem Sie vorhandene Leads hinzufügen und Zuweisungsregeln für neue Leads erstellen.

## Stadien werden genehmigt {#approving-stages}

Genehmigen wir die Phasen Ihres Modells, bevor Sie Leads hinzufügen.

1. Wechseln Sie zum Bereich **Analytics** .

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Wählen Sie das Modell aus, dessen Etappen Sie validieren möchten.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. Wählen Sie unter **Modellaktionen** die Option **Phasen genehmigen**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Sie werden mit einem Warnhinweis begrüßt. Klicken Sie auf **Leads zuweisen**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

Ausgezeichnet! Lassen Sie uns fortfahren und diese Leads zuweisen.

## Zuweisen vorhandener Leads {#assigning-existing-leads}

[Erstellen Sie eine Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) , um die Leads für eine Phase Ihres Modells in Ihrer Lead-Datenbank zu identifizieren.

1. Nachdem Sie [ Ihre Smart-Liste erstellt haben, klicken Sie auf die Registerkarte **Leads** .](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Klicken Sie auf **Alle auswählen** , um die Leads auszuwählen.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Öffnen Sie das Dropdown-Menü **Lead-Aktionen** und wählen Sie **Special** aus. Klicken Sie auf **Umsatzstufe ändern**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Wählen Sie das richtige **Modell** und die richtige **Bühne** aus. Klicken Sie auf **Jetzt ausführen**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Wiederholen Sie diese Schritte, bis alle Leads den verschiedenen Phasen Ihres Modells zugewiesen sind.

Sehr gut! Um festzulegen, wie neue Leads Bühnen zugewiesen werden, erstellen Sie Zuweisungsregeln.

>[!NOTE]
>
>Wenn sich Ihr Modell im Status &quot;Genehmigte Phasen&quot;befindet, werden in den Aktivitätsprotokollen der Leads keine Ereignisse vom Typ &quot;Umsatzstufe ändern&quot;angezeigt. Wenn Ihr Modell vollständig genehmigt ist, wird dieser Flussschritt übersprungen, wenn Sie einen Lead in dieselbe Phase verschieben, in der er sich derzeit befindet.

## Neue Leads: Zuweisungsregeln erstellen  {#new-leads-create-assignment-rules}

1. Klicken Sie erneut auf **Marketo-Startseite** und wählen Sie dann **Analytics** aus.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Klicken Sie auf Ihr Modell in der Struktur und dann im Menü **Modellaktionen** und wählen Sie **Zuweisungsregeln** aus.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. Wenn Ihre Zuweisungsregeln mehr als eine Standardauswahl enthalten, klicken Sie auf **Bühne**, wählen Sie Ihre Auswahl aus und klicken Sie auf **Auswahl hinzufügen**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Beispielzuweisungsregel {#example-assignment-rule}

Erstellen Sie eine Lead-Score-Regel, um die neuen Leads mit einem Mindestwert einem entsprechenden Schritt zuzuweisen.

1. Wählen Sie unter &quot;**If**&quot;die Option &quot;**Lead-Punktzahl**&quot;. Wählen Sie dann **mindestens** aus.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. Geben Sie **40** in das Feld ein und wählen Sie **Verkaufsleiter** als Bühne aus. Klicken Sie zum Abschluss auf **Speichern** .

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Um Ihr Modell zu genehmigen, lesen Sie unsere Hilfeseite unter **[Genehmigen und Nicht genehmigen eines Umsatzmodells](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
