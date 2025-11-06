---
unique-page-id: 2359457
description: Segmentierung genehmigen - Marketo-Dokumente - Produktdokumentation
title: Genehmigen einer Segmentierung
exl-id: c8b0fbe9-012c-47bf-8769-0167156b43d3
feature: Segmentation
source-git-commit: b29186ba84ec88be42432e56d1ad0e77c5b43900
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 2%

---

# Genehmigen einer Segmentierung {#approve-a-segmentation}

Eine Segmentierung muss genehmigt werden, bevor sie verwendet werden kann.

>[!PREREQUISITES]
>
>* [Segmentierung erstellen](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>* [Definieren von Segmentregeln](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>Es können maximal 20 Segmentierungen gleichzeitig genehmigt werden.

1. Navigieren Sie zur **[!UICONTROL Datenbank]**.

   ![](assets/approve-a-segmentation-1.png)

1. Klicken Sie in der Segmentierung **[!UICONTROL Segmentierungsaktionen]** und dann **[!UICONTROL Genehmigen]**.

   ![](assets/approve-a-segmentation-2.png)

   >[!NOTE]
   >
   >Der Status ändert sich in _Genehmigend_ während die Genehmigung ausgeführt wird.

   >[!CAUTION]
   >
   >Die Validierung kann je nach Größe der Datenbank einige Minuten bis zu einem oder zwei Tage dauern.

1. Nach der Genehmigung ändert [!UICONTROL Status] von [!UICONTROL Genehmigend] in [!UICONTROL Genehmigt].

   ![](assets/approve-a-segmentation-3.png)

   >[!TIP]
   >
   >Die Anzahl der Personen in jedem Segment wird in Klammern neben dem Segmentnamen angezeigt.

1. Die **[!UICONTROL Personen]** in **[!UICONTROL Segment]** zeigt jetzt die endgültige Liste der Personen für das Segment an.

   ![](assets/approve-a-segmentation-4.png)

>[!CAUTION]
>
>Die Gesamtzahl der Segmente, die Sie in einer Segmentierung erstellen können, hängt von der Anzahl und dem Typ der verwendeten Filter sowie davon ab, wie komplex die Logik Ihrer Segmente ist. Sie können zwar mithilfe von Standardfeldern bis zu 100 Segmente erstellen, aber die Verwendung anderer Filtertypen kann die Komplexität erhöhen, und Ihre Segmentierung kann möglicherweise nicht genehmigt werden. Einige Beispiele sind: benutzerdefinierte Felder, Felder für Mitglieder der Liste, Felder für Lead-Inhaber und Umsatzstadien.
>
>Wenn Sie während der Genehmigung eine Fehlermeldung erhalten und Unterstützung beim Reduzieren der Komplexität Ihrer Segmentierung benötigen, wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!MORELIKETHIS]
>
>[Verwenden von Segmentfiltern in einer Smart-Liste](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/use-segment-filters-in-a-smart-list.md)
