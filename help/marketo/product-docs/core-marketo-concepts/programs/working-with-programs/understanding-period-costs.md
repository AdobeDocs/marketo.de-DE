---
unique-page-id: 7504676
description: Die Kosten des Zeitraums - Marketing-Dokumente - Produktdokumentation
title: Die Kosten des Zeitraums
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# Die Kosten des Zeitraums {#understanding-period-costs}

## Übersicht {#overview}

Die Zeitkosten beziehen sich auf das Geld, das Sie in einem bestimmten Monat für ein Programm ausgeben.

>[!NOTE]
>
>**Beispiel**
>
>Wenn Sie 1000 $ ausgeben, um einen Illustrator für ein eBook zu mieten, das im Juli gestartet wird, würde das eBook-Programm im Juli Kosten von 1000 $ verursachen.
>
>Wenn Sie $200 pro Monat für Google Adwords ausgeben, würde das Google Adwords Programm einen Zeitraum von $200 **monatlich** kosten.

>[!NOTE]
>
>**Tieftauchen**
>
>[Programme verstehen](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[Informationen zur Programm-Mitgliedschaft](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## Berechnung der Zeitkosten {#how-period-costs-are-calculated}

Stellen Sie sich ein Ereignis vor, wie ein Webinar, das im März stattfindet. Im Januar und Februar werden neue Leute von der Werbung angeworben. Neue Kontakte werden auch nach dem Ereignis erworben, wenn Leute das Webinar in den Monaten April und Mai herunterladen.

1. Mit einem einzigen Zeitraum Kosten auf März...

   ![](assets/graph1.png)

   ...Die in den Monaten vor und nach hinzugefügten Kontakte werden *erst* bis März gezählt.

   ![](assets/graph2.png)

1. Mit Zeitraumkosten, die Januar, Februar und März...

   ![](assets/graph3.png)

   ...Kontakte, die erst in den Monaten nach März hinzugefügt werden, werden bis März gezählt.

   ![](assets/graph4.png)

1. Mit Zeitraumkosten, die auf Januar und April...

   ![](assets/graph5.png)

   ...Die in den Monaten Januar bis März hinzugefügten Kontakte werden auf Januar angerechnet. Die in den Monaten April und Mai hinzugefügten Kontakte werden bis April gezählt.

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >**Erinnerung**
   >
   >
   >Zusammenfassend - Monate ohne definierten Zeitraum werden die Kosten &quot;rückwärts&quot;auf den letzten definierten Zeitraum zurückgeführt. Wenn keine Kosten für einen vorherigen Zeitraum entstehen, werden die Monate auf den nächsten, der definiert wurde, weitergeleitet. Wenn keine Zeitraumkosten für *irgendwelche* Monate definiert wurden, steht der Berichte in RCE für das Programm nicht zur Verfügung.

   >[!NOTE]
   >
   >**Verwandte Artikel**
   >
   >    
   >    
   >    * [Verwenden von Periodenkosten in einem Programm](using-period-costs-in-a-program.md)
   >    * [Filtern eines Programm-Berichts nach Zeitraumkosten](../../../../product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)


