---
unique-page-id: 7504676
description: Die Kosten des Zeitraums - Marketing-Dokumente - Produktdokumentation
title: Die Kosten des Zeitraums
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---


# Die Kosten für den Zeitraum {#understanding-period-costs}

## Übersicht {#overview}

Die Zeitkosten beziehen sich auf das Geld, das Sie in einem bestimmten Monat für ein Programm ausgeben.

>[!NOTE]
>
>**Beispiel**
>
>Wenn Sie 1000 $ ausgeben, um einen Illustrator für ein eBook zu mieten, das im Juli gestartet wird, würde das eBook-Programm im Juli Kosten von 1000 $ verursachen.
>
>Wenn Sie $200 pro Monat für Google Adwords ausgeben, hätte das Google Adwords Programm einen Zeitraum von $200 **pro Monat**.

>[!NOTE]
>
>[Programme verstehen](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[Informationen zur Programm-Mitgliedschaft](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## Berechnung der Periodenkosten {#how-period-costs-are-calculated}

Stellen Sie sich ein Ereignis vor, wie ein Webinar, das im März stattfindet. Im Januar und Februar werden neue Leute von der Werbung angeworben. Neue Kontakte werden auch nach dem Ereignis erworben, wenn Leute das Webinar in den Monaten April und Mai herunterladen.

1. Mit einem einzigen Zeitraum Kosten auf März...

   ![](assets/graph1.png)

   ...Kontakte, die in den Monaten vor und nach hinzugefügt wurden, zählen *nur* bis März.

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
   >Zusammenfassend - Monate ohne definierten Zeitraum werden die Kosten &quot;rückwärts&quot;auf den letzten definierten Zeitraum zurückgeführt. Wenn keine Kosten für einen vorherigen Zeitraum entstehen, werden die Monate auf den nächsten, der definiert wurde, weitergeleitet. Wenn für _beliebige_-Monate keine Periodenkosten definiert wurden, steht der Berichte in RCE für das Programm nicht zur Verfügung.

   >[!MORELIKETHIS]
   >
   >* [Verwenden von Periodenkosten in einem Programm](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [Filtern eines Programm-Berichts nach Zeitraumkosten](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)

