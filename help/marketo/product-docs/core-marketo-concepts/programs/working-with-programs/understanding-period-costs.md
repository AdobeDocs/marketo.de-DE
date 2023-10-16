---
unique-page-id: 7504676
description: Zeitraumkosten - Marketo-Dokumente - Produktdokumentation
title: Zeitkosten verstehen
exl-id: 99f50eaf-28cf-4a8b-8ebd-89a4beef986a
feature: Programs
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Zeitkosten verstehen {#understanding-period-costs}

## Überblick {#overview}

Die Periodenkosten beziehen sich auf das Geld, das Sie in einem bestimmten Monat für ein Programm ausgeben.

>[!NOTE]
>
>**Beispiel**
>
>Wenn Sie 1000 $ ausgeben, um einen Illustrator für ein eBook zu mieten, das im Juli startet, würde das eBook-Programm im Juli einen Zeitraum von 1000 $ kosten.
>
>Wenn Sie 200 USD pro Monat ausgeben [!DNL Google Adwords] - die [!DNL Google Adwords] Das Programm hätte Kosten in Höhe von 200 USD _jeden Monat_.

>[!NOTE]
>
>[Grundlegendes zu Programmen](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[Grundlegendes zur Programmmitgliedschaft](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## Berechnung der Zeitraumkosten {#how-period-costs-are-calculated}

Stellen Sie sich ein Ereignis vor, wie ein Webinar, das im März stattfindet. Im Vorfeld werden im Januar und Februar neue Menschen durch Werbung angeworben. Nach der Veranstaltung, wenn die Teilnehmer das Webinar in den Monaten April und Mai herunterladen, werden auch neue Kontakte aufgenommen.

1. Mit einem einzigen Zeitraum Kosten auf März...

   ![](assets/graph1.png)

   ...in den Monaten vor und nach hinzugefügten Kontakten *only* bis März.

   ![](assets/graph2.png)

1. Mit Zeitraumkosten, die Januar, Februar und März..

   ![](assets/graph3.png)

   ...werden Kontakte, die nur in den Monaten nach März hinzugefügt werden, auf März angerechnet.

   ![](assets/graph4.png)

1. Mit Zeitraumkosten, die Januar und April zugeordnet werden...

   ![](assets/graph5.png)

   ... werden die in den Monaten Januar bis März hinzugefügten Kontakte auf Januar angerechnet. In den Monaten April und Mai hinzugefügte Kontakte werden bis April zählen.

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >Zusammenfassend: Monate ohne definierten Zeitraum führen die Kosten &quot;rückwärts&quot;zum letzten definierten. Wenn keine vorherigen Zeitraumkosten entstehen, werden die Monate auf den nächsten, der definiert wurde, &quot;weitergeleitet&quot;. Wenn für _any_ -Monate nicht verfügbar sein, wird die Berichterstellung in RCE nicht für das Programm verfügbar sein.

   >[!MORELIKETHIS]
   >
   >* [Verwenden von Zeitraumkosten in einem Programm](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [Filtern eines Programmberichts nach Periodenkosten](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)
