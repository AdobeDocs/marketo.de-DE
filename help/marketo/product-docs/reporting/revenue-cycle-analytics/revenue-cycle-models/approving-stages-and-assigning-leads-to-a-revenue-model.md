---
unique-page-id: 4718683
description: Genehmigen von Phasen und Zuweisen von Interessenten zu einem Umsatzmodell - Marketing-Dokumente - Produktdokumentation
title: Genehmigen von Phasen und Zuweisen von Interessenten zu einem Umsatzmodell
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---


# Genehmigen von Phasen und Zuweisen von Interessenten zu einem Umsatzmodell {#approving-stages-and-assigning-leads-to-a-revenue-model}

Richten Sie Ihr **Umsatzmodell** ein, indem Sie vorhandene Interessenten hinzufügen und Zuordnungsregeln für alle neuen Interessenten erstellen.

## Genehmigungsphasen {#approving-stages}

Genehmigen wir die Phasen Ihres Modells, bevor Sie Interessenten hinzufügen.

1. Wechseln Sie zum Bereich **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Wählen Sie das Modell aus, dessen Phasen Sie genehmigen möchten.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. Wählen Sie unter **Modellaktionen** **Phasen genehmigen**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Sie werden mit einer Warnung begrüßt. Klicken Sie auf **Leads zuweisen**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

Ausgezeichnet! Lassen Sie uns fortfahren und diese Leads zuweisen.

## Zuweisen vorhandener Interessenten {#assigning-existing-leads}

[Erstellen Sie eine intelligente ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) Liste, um die Interessenten für eine Phase Ihres Modells in Ihrer Interessentendatenbank zu identifizieren.

1. Nachdem Sie [Ihre Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) erstellt haben, klicken Sie auf die Registerkarte **Interessenten**.

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Klicken Sie auf **Wählen Sie Alle** aus, um die Leads auszuwählen.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Öffnen Sie die Dropdownliste **Interessentenaktionen** und wählen Sie **Spezial**. Klicken Sie auf **Umsatzstufe ändern**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Wählen Sie das richtige **Modell** und die richtige **Stufe**. Klicken Sie auf **Jetzt ausführen**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Wiederholen Sie diese Schritte, bis alle Interessenten den verschiedenen Phasen Ihres Modells zugeordnet sind.

Großartig! Erstellen Sie Zuordnungsregeln, um festzulegen, wie den Phasen neue Leads zugewiesen werden.

>[!NOTE]
>
>Wenn sich Ihr Modell im Status &quot;Genehmigte Phasen&quot;befindet, werden in den Aktivitäten-Protokollen der Interessenten keine Ereignisse zur Umsatzstufe ändern angezeigt. Wenn Ihr Modell vollständig genehmigt ist, wird dieser Flussschritt übersprungen, wenn Sie einen Interessenten in dieselbe Phase verschieben, in der er sich gerade befindet.

## Neue Interessenten: Aufgabenregeln {#new-leads-create-assignment-rules} erstellen

1. Klicken Sie erneut auf **Markieren Sie** und wählen Sie **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Klicken Sie in der Struktur auf Ihr Modell und wählen Sie dann im Menü **Modellaktionen** die Option **Zuweisungsregeln**.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. Wenn Ihre Zuordnungsregeln mehr als nur eine Standardauswahl enthalten, klicken Sie auf **Stage**, wählen Sie aus und klicken Sie dann auf **Hinzufügen Auswahl**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Beispielzuweisungsregel {#example-assignment-rule}

Erstellen Sie eine Interessentenbewertungsregel, um die neuen Interessenten mit einer Mindestpunktzahl einem entsprechenden Schritt zuzuweisen.

1. Wählen Sie unter **Wenn** **Interessentenbewertung**. Wählen Sie dann **mindestens**.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. Geben Sie **40** in das Feld ein und wählen Sie **Verkaufsleiter** als Phase. Klicken Sie auf **Speichern**, um abzuschließen.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Um Ihr Modell zu genehmigen, lesen Sie unsere Hilfeseite unter **[Genehmigen und Nicht genehmigen eines Umsatzmodells](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
