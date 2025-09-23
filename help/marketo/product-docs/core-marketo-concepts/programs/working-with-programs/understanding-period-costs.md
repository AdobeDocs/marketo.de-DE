---
unique-page-id: 7504676
description: Grundlegendes zu Periodenkosten - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zu Kostenzeiträumen
exl-id: 99f50eaf-28cf-4a8b-8ebd-89a4beef986a
feature: Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 2%

---

# Grundlegendes zu Kostenzeiträumen {#understanding-period-costs}

## Überblick {#overview}

Periodenkosten beziehen sich auf das Geld, das Sie in einem bestimmten Monat für ein Programm ausgeben.

>[!NOTE]
>
>**Beispiel**
>
>Wenn Sie 1000 US-Dollar ausgeben, um einen Illustrator für ein [!DNL eBook] zu mieten, das im Juli startet, würde das [!DNL eBook]-Programm im Juli einen Zeitraum von 1000 US-Dollar kosten.
>
>Wenn Sie pro Monat 200 $ für [!DNL Google Adwords] ausgeben, würde das [!DNL Google Adwords]-Programm einen Zeitraum von 200 $ (_Monat)_.

>[!NOTE]
>
>[Grundlegendes zu Programmen](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
>
>[Grundlegendes zur Programmmitgliedschaft](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)

## So werden Periodenkosten berechnet {#how-period-costs-are-calculated}

Stellen Sie sich ein Ereignis wie ein Webinar im März vor. Durch Werbung im Januar und Februar werden im Vorfeld neue Personen gewonnen. Neue Kontakte werden auch im Anschluss an die Veranstaltung geknüpft, wenn das Webinar in den Monaten April und Mai heruntergeladen wird.

1. Mit einem einzigen Zeitraum, der März zugeordnet wurde…

   ![](assets/graph1.png)

   …Kontakte, die in den Monaten davor und danach hinzugefügt wurden _werden_ bis März gezählt.

   ![](assets/graph2.png)

1. Mit Periodenkosten, die Januar, Februar und März zugeordnet werden…

   ![](assets/graph3.png)

   …Kontakte, die erst in den Monaten nach März hinzugefügt werden, zählen bis März.

   ![](assets/graph4.png)

1. Mit Periodenkosten, die Januar und April zugeordnet werden…

   ![](assets/graph5.png)

   …Kontakte, die in den Monaten Januar bis März hinzugefügt wurden, werden bis Januar gezählt. In den Monaten April und Mai hinzugefügte Kontakte werden bis April gezählt.

   ![](assets/graph6.png)

   >[!NOTE]
   >
   >Zusammenfassend lässt sich sagen, dass Monate ohne definierten Zeitraum die Kosten „rückwärts“ auf den letzten definierten Zeitraum abrollen. Wenn es keine Kosten für die Vorperiode gibt, werden die Monate auf die nächste definierte Periode „vorgerollt“. Wenn für einen Zeitraum von (_) Monaten kein_ definiert wurde, steht für das Programm kein RCE-Bericht zur Verfügung.

   >[!MORELIKETHIS]
   >
   >* [Periodenkosten in einem Programm verwenden](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program.md)
   >* [Filtern Sie einen Programmbericht nach Periodenkosten](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/filter-a-program-report-by-period-cost.md)
