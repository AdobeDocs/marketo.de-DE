---
unique-page-id: 4718683
description: Genehmigen von Phasen und Zuweisen von Leads zu einem Umsatzmodell - Marketo Docs - Produktdokumentation
title: Genehmigen von Phasen und Zuweisen von Leads zu einem Umsatzmodell
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Genehmigen von Phasen und Zuweisen von Leads zu einem Umsatzmodell {#approving-stages-and-assigning-leads-to-a-revenue-model}

Holen Sie sich **Umsatzmodell** durch Hinzufügen vorhandener Leads und Erstellen von Zuweisungsregeln für alle neuen Leads ausgeführt werden.

## Stadien werden genehmigt {#approving-stages}

Genehmigen wir die Phasen Ihres Modells, bevor Sie Leads hinzufügen.

1. Navigieren Sie zu **Analytics** Bereich.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Wählen Sie das Modell aus, dessen Etappen Sie validieren möchten.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. under **Modellaktionen** auswählen **Phasen genehmigen**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Sie werden mit einem Warnhinweis begrüßt. click **Leads zuweisen**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

Ausgezeichnet! Lassen Sie uns fortfahren und diese Leads zuweisen.

## Zuweisen vorhandener Leads {#assigning-existing-leads}

[Erstellen einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) , um die Leads für eine Phase Ihres Modells in Ihrer Lead-Datenbank zu identifizieren.

1. Sobald du [Smart List erstellt haben](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md), klicken Sie auf die **Leads** Registerkarte.

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Klicken **Alle auswählen** , um die Leads auszuwählen.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Öffnen Sie die **Lead-Aktionen** und wählen Sie **Sonderaktion**. Klicken **Umsatzstufe ändern**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Richtig auswählen **Modell** und der korrekten **Staging**. Klicken **Jetzt ausführen**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Wiederholen Sie diese Schritte, bis alle Leads den verschiedenen Phasen Ihres Modells zugewiesen sind.

Sehr gut! Um festzulegen, wie neue Leads Bühnen zugewiesen werden, erstellen Sie Zuweisungsregeln.

>[!NOTE]
>
>Wenn sich Ihr Modell im Status &quot;Genehmigte Phasen&quot;befindet, werden in den Aktivitätsprotokollen der Leads keine Ereignisse vom Typ &quot;Umsatzstufe ändern&quot;angezeigt. Wenn Ihr Modell vollständig genehmigt ist, wird dieser Flussschritt übersprungen, wenn Sie einen Lead in dieselbe Phase verschieben, in der er sich derzeit befindet.

## Neue Leads: Erstellen von Zuweisungsregeln  {#new-leads-create-assignment-rules}

1. Klicken **Marketo - Startseite** Wählen Sie erneut **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Klicken Sie auf Ihr Modell in der Baumstruktur und dann auf das **Modellaktionen** Menü, auswählen **Zuweisungsregeln**.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. Wenn Ihre Zuweisungsregeln mehr als nur eine Standardauswahl enthalten, klicken Sie auf **Staging**, wählen Sie Ihre Auswahl aus und klicken Sie auf **Auswahl hinzufügen**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Beispielzuweisungsregel {#example-assignment-rule}

Erstellen Sie eine Lead-Score-Regel, um die neuen Leads mit einem Mindestwert einem entsprechenden Schritt zuzuweisen.

1. under **Wenn** auswählen **Lead-Punktzahl**. Dann wählen Sie **mindestens**.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. Eingabe **40** und wählen Sie **Vertriebsmitarbeiter** als Bühne. Klicken **Speichern** zu beenden.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Um Ihr Modell zu genehmigen, lesen Sie unsere Hilfeseite unter **[Genehmigen und Aufheben der Genehmigung eines Umsatzmodells](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
