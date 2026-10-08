---
unique-page-id: 2360389
description: Erfahren Sie, wie Sie ein Programm ohne Zeitraumkosten in Revenue Explorer und Analyzer in Marketo Engage verfügbar machen. Verwenden Sie dieses Handbuch, um Ihren nächsten Schritt abzuschließen.
title: Verfügbarmachen eines Programms ohne Kostenzeitraum in Revenue Explorer und Analyzern
exl-id: 45a24b9f-d92f-4f48-a7d1-0be14cd128b1
feature: Reporting, Revenue Cycle Analytics
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
    internal-label: Reporting
  - id: 126e34f9-e02a-505e-9978-ea36537f3ef9
    internal-label: Revenue Cycle Analytics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 11%
---
# Verfügbarmachung eines Programms ohne Kostenzeitraum in Revenue Explorer und Analyzer {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

Mit Kosten für den Programmzeitraum können Sie festlegen, „wie viel Geld“ und „wann“ für ein Programm ausgegeben werden soll. Dies wird im Umsatzzyklus-Explorer und in [Analyzer](/help/marketo/product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md) angezeigt.

>[!NOTE]
>
>**Admin-Berechtigungen erforderlich**

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
