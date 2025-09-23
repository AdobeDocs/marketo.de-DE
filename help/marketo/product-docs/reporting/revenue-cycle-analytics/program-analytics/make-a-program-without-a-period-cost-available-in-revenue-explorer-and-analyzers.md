---
unique-page-id: 2360389
description: Erstellen Sie ein Programm ohne Kostenzeitraum in Revenue Explorer und Analyzer - Marketo-Dokumente - Produktdokumentation
title: Verfügbarmachung eines Programms ohne Kostenzeitraum in Revenue Explorer und Analyzer
exl-id: 45a24b9f-d92f-4f48-a7d1-0be14cd128b1
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 10%

---

# Verfügbarmachung eines Programms ohne Kostenzeitraum in Revenue Explorer und Analyzer {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

Mit Kosten für den Programmzeitraum können Sie festlegen, „wie viel Geld“ und „wann“ für ein Programm ausgegeben werden soll. Dies wird im Umsatzzyklus-Explorer und in [Analyzer](/help/marketo/product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md) angezeigt.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

Einige Programme müssen möglicherweise einbezogen werden, auch wenn sie keine Periodenkosten haben. Obwohl Sie für den Kostenzeitraum 0 eingeben können, haben wir die Einbeziehung dieser Programme vereinfacht.

>[!NOTE]
>
>Der Programm-Analyzer erfasst den Programmerfolg nach Kostenzeitraum. Wenn keine Periodenkosten verfügbar sind, wird der Programmerfolg unabhängig vom Analyseverhalten des Programms nicht angezeigt. Wenn das Analytics-Verhalten eingerichtet ist, werden Daten für Opportunity-Metriken angezeigt (Pipeline-Opportunities, gewonnener Umsatz usw.).

1. Klicken Sie [!UICONTROL  Abschnitt ]Admin“ auf **[!UICONTROL Tags]**.

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. Erweitern Sie Ihre Kanäle und doppelklicken Sie auf den Kanal Ihrer Wahl.

   >[!NOTE]
   >
   >Alle Programme, die diesen Kanal verwenden, werden unabhängig von den Periodenkosten für Revenue Explorer und Analyzer verfügbar. Diese Änderung wird am folgenden Tag wirksam.

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. Ändern Sie [!UICONTROL Analytics Behavior] in **Inclusive** und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>Haben Sie die Option „Operativ“ bemerkt? Dies bewirkt das Gegenteil. Sie schließt diese Programme unabhängig von den Periodenkosten aus.

Gute Arbeit! Jetzt werden alle Programme, die den geänderten Kanal verwenden, in den Umsatz-Explorer und -Analyzer einbezogen, ohne dass ein Kostenzeitraum erforderlich ist.

>[!MORELIKETHIS]
>
>[Überschreiben des Analytics-Verhaltens auf Programmebene](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/override-analytics-behavior-at-the-program-level.md)
