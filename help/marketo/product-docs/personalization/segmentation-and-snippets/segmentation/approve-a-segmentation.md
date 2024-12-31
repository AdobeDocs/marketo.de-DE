---
unique-page-id: 2359457
description: Segmentierung genehmigen - Marketo-Dokumente - Produktdokumentation
title: Segmentierung genehmigen
exl-id: c8b0fbe9-012c-47bf-8769-0167156b43d3
feature: Segmentation
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 0%

---

# Segmentierung genehmigen {#approve-a-segmentation}

Eine Segmentierung muss genehmigt werden, bevor sie verwendet werden kann.

>[!PREREQUISITES]
>
>* [Segmentierung erstellen](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>* [Definieren von Segmentregeln](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>Es können maximal 20 Segmentierungen gleichzeitig genehmigt werden.

1. Navigieren Sie zur **Datenbank**.

   ![](assets/image2017-3-28-14-3a25-3a49.png)

1. Klicken Sie in der Segmentierung **Segmentierungsaktionen** und dann **Genehmigen**.

   ![](assets/image2017-3-28-14-3a46-3a22.png)

   >[!NOTE]
   >
   >Der Status ändert sich in Genehmigen mit sich drehendem Rad ( ![](assets/image2014-9-15-15-3a31-3a43.png)) , während die Genehmigung ausgeführt wird.

   >[!CAUTION]
   >
   >Die Validierung kann je nach Größe der Datenbank einige Minuten bis über einen Tag dauern.

   Nach der Genehmigung ändert sich der Status von Genehmigend in Genehmigt.
   ![](assets/image2017-3-28-14-3a46-3a44.png)

   >[!TIP]
   >
   >Die Anzahl der Personen in jedem Segment wird in Klammern neben dem Segmentnamen angezeigt.

1. Die **Personen** in **Segment** zeigt jetzt die endgültige Liste der Personen für das Segment an.

   ![](assets/image2017-3-28-14-3a47-3a10.png)

>[!CAUTION]
>
>Die Gesamtzahl der Segmente, die Sie in einer Segmentierung erstellen können, hängt von der Anzahl und dem Typ der verwendeten Filter sowie davon ab, wie komplex die Logik Ihrer Segmente ist. Sie können zwar mithilfe von Standardfeldern bis zu 100 Segmente erstellen, aber die Verwendung anderer Filtertypen kann die Komplexität erhöhen, und Ihre Segmentierung kann möglicherweise nicht genehmigt werden. Einige Beispiele sind: benutzerdefinierte Felder, Felder für Mitglieder der Liste, Felder für Lead-Inhaber und Umsatzstadien.
>
>Wenn Sie während der Genehmigung eine Fehlermeldung erhalten und Unterstützung beim Reduzieren der Komplexität Ihrer Segmentierung benötigen, wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!MORELIKETHIS]
>
>[Verwenden von Segmentfiltern in einer Smart-Liste](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/use-segment-filters-in-a-smart-list.md)
