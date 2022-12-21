---
unique-page-id: 2360389
description: Bereitstellen eines Programms ohne Periodenkosten in Umsatz-Explorer und Analyzern - Marketo-Dokumente - Produktdokumentation
title: Bereitstellen eines Programms ohne Periodenkosten in Umsatz-Explorer und Analyzern
exl-id: 45a24b9f-d92f-4f48-a7d1-0be14cd128b1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Bereitstellen eines Programms ohne Periodenkosten in Umsatz-Explorer und Analyzern {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

Die Kosten des Programmzeitraums ermöglichen es Ihnen, &quot;Wie viel Geld&quot;und &quot;Wann&quot;für ein Programm zu definieren. Dies wird in Umsatz-Cycle Explorer angezeigt und [Analyzer](/help/marketo/product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md).

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

Einige Programme müssen möglicherweise auch ohne Zeitraumkosten eingeschlossen werden. Sie können zwar 0 für die Zeitraumkosten eingeben, doch wir haben die Einbeziehung dieser Programme vereinfacht.

>[!NOTE]
>
>Der Programm-Analyzer erfasst den Erfolg des Programms nach Zeitraumkosten. Wenn keine Zeitraumkosten verfügbar sind, wird der Erfolg des Programms unabhängig vom Analyseverhalten des Programms nicht angezeigt. Wenn das Analytics-Verhalten eingerichtet ist, werden Daten für Opportunitätsmetriken angezeigt (Pipeline-Chancen, Umsatz usw.).

1. Klicken Sie im Abschnitt &quot;Admin&quot;auf **Tags**.

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. Erweitern Sie Ihre Kanäle und doppelklicken Sie auf den gewünschten Kanal.

   >[!NOTE]
   >
   >Alle Programme, die diesen Kanal verwenden, stehen unabhängig von den Zeitraumkosten für den Umsatz-Explorer und Analyzer zur Verfügung. Diese Änderung wird am folgenden Tag wirksam.

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. Ändern Sie das Analytics-Verhalten in &quot;Inclusive&quot;und klicken Sie auf **Speichern**.

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>Haben Sie die Betriebsoption bemerkt? Das tut das Gegenteil. Diese Programme werden unabhängig von den Zeitraumkosten ausgeschlossen.

Gut gemacht! Jetzt werden alle Programme, die den modifizierten Kanal verwenden, in den Umsatz-Explorer und Analyzer aufgenommen, ohne dass Zeitraumkosten erforderlich sind.

>[!MORELIKETHIS]
>
>[Analytics-Verhalten auf Programmebene überschreiben](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/override-analytics-behavior-at-the-program-level.md)
