---
unique-page-id: 7515767
description: Freigeben von Segmenten über Arbeitsbereiche und Partitionen - Marketing-Dokumente - Produktdokumentation
title: Freigeben von Segmenten über Workspaces und Partitionen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---


# Freigeben von Segmenten über Arbeitsbereiche und Partitionen {#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>Dieser Artikel gilt nur für Kunden mit Arbeitsbereichen und Partitionen

## Was ist eine Segmentierung? {#whats-a-segmentation}

Marketo ist großartig darin, genau die richtigen Leute für ein Programm oder eine intelligente Kampagne auszuwählen. Für permanentere Personen sollten Sie jedoch Segmentationen verwenden. Sie werden benötigt, um erweiterte dynamische Inhalte in Marketing zu verwenden.

>[!NOTE]
>
>**Tieftauchen**
>
>Lernen Sie [wie Sie Segmentationen](../../../product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md) erstellen.

Nachdem Sie diese Personen eingerichtet haben (**und** verwenden Sie Arbeitsbereiche), möchten Sie sie auf allen Arbeitsbereichen freigeben. Hier einige gute Dinge zu wissen:

## Regeln und Tipps {#rules-tips}

* Jedes Marketo-Abonnement kann bis zu 20 Segmentationen &quot;gesamt&quot;über mehrere Arbeitsbereiche hinweg enthalten (**nicht 20 pro Arbeitsbereich**).
* Sie können eine Segmentierung nur für Arbeitsbereiche freigeben, auf die Sie Zugriff haben.
* Stellen Sie sicher, dass Sie einen **Standardarbeitsbereich erstellen und verwenden, der Sichtbarkeit in allen Partitionen** aufweist.

* Die Segmentierungsverarbeitung wird nur für die Personen im Arbeitsbereich ausgeführt, in dem die Segmentierung erstellt wird.

   * Erstellen Sie die Segmentierung, die Sie im Standardarbeitsbereich freigeben möchten.

      * Segmentierung genehmigen
      * Der freigegebene Arbeitsbereich sieht einen gesperrten Ordner und die Segmentierung ist schreibgeschützt.
      * Die freigegebene Version kann nicht bearbeitet werden. Sie können die ursprüngliche Segmentierung nur dort bearbeiten, wo sie erstellt wurde.
   * Wenn Sie innerhalb einer freigegebenen Segmentierung auf ein Segment (z. B. das Gesundheitswesen) klicken, werden nur Personen in der Partition angezeigt, die mit dem angezeigten Arbeitsbereich verbunden sind.

      * Wenn Sie eine Segmentierung in Workspace 1 (WS1) erstellen und sie mit WS2 und WS1 freigeben, die keinen Zugriff auf die Partition für WS2 haben, wird die Segmentierung NICHT neu berechnet.
      * Wenn Sie eine Segmentierung in einem Arbeitsbereich mit eingeschränkten Partitionen erstellen und diese dann für einen anderen Arbeitsbereich freigeben, sieht dieser Arbeitsbereich, der die freigegebene Segmentierung erhalten hat, nur Personen, die sich überschneiden.


>[!NOTE]
>
>Einige dieser Regeln sind etwas komplex. Die einfachste Möglichkeit, mit bestimmten Personen zu beginnen, besteht darin, sie zu testen. Sie können immer neue Segmente erstellen und die alten entfernen.

## Beispielszenarios {#example-scenarios}

![](assets/image2015-5-27-16-3a26-3a25.png)

** ![](assets/image2015-5-27-16-3a26-3a48.png)

**

## Freigeben einer Segmentierung {#share-a-segmentation}

1. Wechseln Sie zur Datenbank.

   ![](assets/image2017-3-29-8-3a15-3a40.png)

1. Klicken Sie mit der rechten Maustaste auf Segmente und wählen Sie Neue Ordner.

   ![](assets/image2017-3-29-8-3a40-3a31.png)

1. Benennen Sie den Ordner, den Sie für mehrere Arbeitsbereiche freigeben möchten (Beispiel: Segmente freigeben.)

   ![](assets/image2017-3-29-8-3a40-3a45.png)

1. Verschieben Sie die Segmente, die Sie freigeben möchten, in den Ordner.

   ![](assets/image2017-3-29-8-3a41-3a3.png)

1. Klicken Sie mit der rechten Maustaste auf den Ordner und wählen Sie Ordner freigeben.

   ![](assets/image2017-3-29-8-3a41-3a19.png)

1. Wählen Sie die Arbeitsflächen aus, für die Sie den Ordner freigeben möchten. Klicken Sie auf Speichern.

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >Im Dialogfeld werden die Arbeitsbereiche angezeigt, für die Sie über die Berechtigung zur Ansicht verfügen. Daher empfiehlt Marketo die Erstellung und Freigabe von Segmenten aus dem Standardarbeitsbereich, der alle Arbeitsbereiche und Partitionen sichtbar macht.

Der ursprüngliche Ordner wird in der Datenbankstruktur mit einem Pfeil angezeigt, der angibt, dass er für andere Arbeitsbereiche freigegeben ist. Innerhalb des freigegebenen Arbeitsbereichs wird der Ordner mit einer Sperre angezeigt, um anzugeben, dass der Inhalt des Ordners von einem anderen Arbeitsbereich freigegeben wurde und schreibgeschützt ist.

>[!NOTE]
>
>**Verwandte Artikel**
>
>[Segmentierung und Snippets](http://docs.marketo.com/display/docs/segmentation+and+snippets)

