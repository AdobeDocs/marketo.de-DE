---
unique-page-id: 2359449
description: Definieren von Segmentregeln - Marketo-Dokumente - Produktdokumentation
title: Segmentregeln definieren
exl-id: e6631848-aa8c-4709-b182-4c88abbd365b
feature: Segmentation
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Segmentregeln definieren {#define-segment-rules}

Durch die Definition von Segmentregeln können Sie Ihre Personen in verschiedene Gruppen kategorisieren, die sich gegenseitig ausschließen.

>[!PREREQUISITES]
>
>[Erstellen einer Segmentierung](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

1. Navigieren Sie zu **Datenbank.**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. Auswählen **Segmentierung** aus der Baumstruktur und klicken Sie dann auf ein bestimmtes **Segment**.

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. Klicken **Smart List** und Filter hinzufügen.

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >Segmente unterstützen derzeit nicht _In der Vergangenheit_ und _In Zeitrahmen_  Operatoren in Filtern. Dies liegt daran, dass Segmentierungen nur dann auf Aktualisierungen überprüfen, wenn ein Änderungsdatenwert protokolliert wird. Diese Werte sind _not_ protokolliert für Dinge, die sich automatisch ändern, wie beispielsweise Formelfelder und Datumswerte. Darüber hinaus werden Datumsoperatoren mit relativen Datumsbereichen nicht unterstützt, da sie zum Zeitpunkt der Segmentierungsgenehmigung und nicht zum Zeitpunkt der Aktivität Datenwert ändern berechnet werden.

   >[!NOTE]
   >
   >Die Filter &quot;SFDC-Typ&quot;und &quot;Microsoft-Typ&quot;werden derzeit nicht in Smart-Listen zur Segmentierung unterstützt.

1. Füllen Sie die entsprechenden Werte für die Filter aus.

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!CAUTION]
   >
   >Das Aktivitätsprotokollierungsverhalten für Kontofelder kann sich auf die Qualifizierung auswirken. Daher empfehlen wir, bei der Definition von Segmentregeln keine Kontofelder zu verwenden.

1. Klicken Sie auf **Personen (Entwurf)** um die Personen anzuzeigen, die sich möglicherweise als Mitglied dieses Segments qualifizieren.

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. Navigieren Sie zu **Segmentierungsaktionen**. Klicken **Genehmigen**.

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >Die Gesamtanzahl der Segmente, die Sie in einer Segmentierung erstellen können, hängt von der Anzahl und dem Typ der verwendeten Filter sowie davon ab, wie komplex die Logik Ihrer Segmente ist. Sie können zwar bis zu 100 Segmente mithilfe von Standardfeldern erstellen, aber die Verwendung anderer Filtertypen kann die Komplexität erhöhen und Ihre Segmentierung kann möglicherweise nicht genehmigt werden. Beispiele: benutzerdefinierte Felder, Mitglied der Liste, Felder des Lead-Eigentümers und Umsatzstufen.
   >
   >Wenn Sie eine Fehlermeldung während der Validierung erhalten und Unterstützung bei der Reduzierung der Komplexität Ihrer Segmentierung benötigen, wenden Sie sich an [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Im Dashboard erhalten Sie einen schnellen Überblick über Ihre Segmente in einem Tortendiagramm sowie über die angewendeten Regeln.

   ![](assets/image2014-9-15-11-3a36-3a19.png)

Gute Arbeit! Diese Segmente werden an vielen Orten in Marketo praktisch sein.

>[!NOTE]
>
>Eine Person kann sich für verschiedene Segmente qualifizieren, gehört jedoch letztendlich zu nur einem Segment, das von der Variablen [Prioritätsreihenfolge der Segmente](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md).

>[!NOTE]
>
>Der Bildschirm Personen (Entwurf) zeigt alle Personen an, die sich als Mitglied qualifizieren und nicht immer die endgültige Liste der Personen ist. Genehmigen Sie Ihr Segment, um die endgültige Liste anzuzeigen.

>[!MORELIKETHIS]
>
>[Genehmigen einer Segmentierung](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md)
