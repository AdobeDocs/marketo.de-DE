---
unique-page-id: 7515767
description: Regeln und Schritte für die Freigabe von Segmentierungen über Arbeitsbereiche und Partitionen hinweg, einschließlich Einschränkungen und Tipps für die Erstellung von Segmentierungen im Standardarbeitsbereich.
title: Freigeben von Segmentierungen über Arbeitsbereiche und Partitionen hinweg
exl-id: b50f4328-fdba-4e39-bc0d-75bade1f9cbc
feature: Partitions, Workspaces
TQID: https://experienceleague.adobe.com/fzHumE5x1Y5tSVjUUlHabe-cZgPC5jmqwtl4aLYhjDA
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2: id: a1d50dda-6d94-4e16-8c30-5eb7181c4650id: cdd4e0f6-e87e-453f-88ee-2ee54a7de272id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 471
ht-degree: 4%

---

# Freigeben von Segmentierungen über Arbeitsbereiche und Partitionen hinweg {#share-segmentations-across-workspaces-and-partitions}

>[!PREREQUISITES]
>
>Dieser Artikel ist nur für Kunden mit Arbeitsbereichen und Partitionen.

## Was ist eine Segmentierung? {#whats-a-segmentation}

Marketo identifiziert die richtigen Personen für ein Programm oder eine intelligente Kampagne. Für dauerhaftere Rollen sollten Sie jedoch Segmentierungen verwenden. Sie werden benötigt, um erweiterte dynamische Inhalte in Marketo zu verwenden.

>[!NOTE]
>
>Erfahren Sie [wie Sie Segmentierungen erstellen](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).

Nachdem Sie diese Rollen eingerichtet haben (_und_ Arbeitsbereiche verwenden), sollten Sie sie für alle Ihre Arbeitsbereiche freigeben. Hier sind einige gute Dinge zu wissen:

## Regeln und Tipps {#rules-tips}

* Jedes Marketo-Abonnement kann bis zu 20 Segmentierungen „insgesamt“ über mehrere Arbeitsbereiche hinweg enthalten (**20 pro Arbeitsbereich**).
* Sie können eine Segmentierung nur für Arbeitsbereiche freigeben, auf die Sie Zugriff haben.
* Erstellen und verwenden Sie einen **Standardarbeitsbereich mit Einblick in alle Partitionen**.

* Die Segmentierungsverarbeitung wird nur für die Personen im Arbeitsbereich ausgeführt, in dem die Segmentierung erstellt wurde.

   * Erstellen Sie die Segmentierung, die Sie in der Standard-Workspace freigeben möchten.
      * Segmentierung genehmigen
      * Im freigegebenen Arbeitsbereich wird ein gesperrter Ordner angezeigt, und die Segmentierung ist schreibgeschützt.
      * Die freigegebene Version kann nicht bearbeitet werden. Sie können nur die ursprüngliche Segmentierung bearbeiten, in der sie erstellt wurde.

   * Wenn Sie innerhalb einer freigegebenen Segmentierung auf ein Segment (z. B. das Gesundheitswesen) klicken, sind die angezeigten Personen nur Personen in der Partition, die mit dem angezeigten Arbeitsbereich verknüpft ist.
      * Wenn Sie eine Segmentierung in Workspace 1 (WS1) erstellen und sie für WS2 freigeben und WS1 keinen Zugriff auf die Partition für WS2 hat, wird die Segmentierung NICHT neu berechnet.
      * Wenn Sie eine Segmentierung in einem Arbeitsbereich mit begrenzten Partitionen erstellen und sie dann für einen anderen Arbeitsbereich freigeben, werden in diesem Arbeitsbereich, der die freigegebene Segmentierung erhalten hat, nur Personen mit Überschneidungen angezeigt.

>[!NOTE]
>
>Einige dieser Regeln sind komplex. Es wird empfohlen, mit bestimmten Personen zu testen. Neue Segmentierungen können erstellt und alte nach Bedarf gelöscht werden.

## Beispielszenarien {#example-scenarios}

![](assets/share-segmentations-across-workspaces-and-partitions-1.png)

![](assets/share-segmentations-across-workspaces-and-partitions-2.png)

## Segmentierung freigeben {#share-a-segmentation}

1. Navigieren Sie zur **[!UICONTROL Datenbank]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-3.png)

1. Klicken Sie mit der rechten Maustaste **[!UICONTROL Segmentierungen]** und wählen Sie **[!UICONTROL Neuer Ordner]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-4.png)

1. Benennen Sie den Ordner, der für alle Arbeitsbereiche freigegeben werden soll (Beispiel: Segmentierungen freigeben), und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-5.png)

1. Verschieben Sie die Segmentierung(en), die Sie freigeben möchten, in den Ordner .

   ![](assets/share-segmentations-across-workspaces-and-partitions-6.png)

1. Klicken Sie mit der rechten Maustaste auf den Ordner und wählen Sie **[!UICONTROL Ordner freigeben]** aus.

   ![](assets/share-segmentations-across-workspaces-and-partitions-7.png)

1. Wählen Sie die Arbeitsbereiche aus, für die Sie den Ordner freigeben möchten. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/share-segmentations-across-workspaces-and-partitions-8.png)

   >[!NOTE]
   >
   >Das Dialogfeld zeigt die Arbeitsbereiche an, für die Sie über die Berechtigung zum Anzeigen verfügen. Aus diesem Grund empfiehlt Marketo, Segmentierungen aus dem Standardarbeitsbereich zu erstellen und freizugeben, der Einblick in alle Arbeitsbereiche und Partitionen bietet.

Der ursprüngliche Ordner wird in der Datenbankstruktur mit einem Pfeil angezeigt, der angibt, dass er für andere Arbeitsbereiche freigegeben ist. Innerhalb des freigegebenen Arbeitsbereichs wird der Ordner mit einer Sperre angezeigt, um anzugeben, dass der Inhalt des Ordners von einem anderen Arbeitsbereich freigegeben wurde und schreibgeschützt ist.
