---
unique-page-id: 2360401
description: Vergleichen der Kanaleffektivität mit dem Programm-Analyzer - Marketo Docs - Produktdokumentation
title: Kanaleffektivität mit dem Programm-Analyzer vergleichen
exl-id: bfe635a7-b077-4074-889d-fc2256102cd5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Kanaleffektivität mit dem Programm-Analyzer vergleichen {#compare-channel-effectiveness-with-the-program-analyzer}

Verwenden Sie den Programm-Analyzer, um die Kanalkosten, die Mitgliederakquise, die Pipeline, den Umsatz und mehr zu vergleichen und Ihre effektivsten Kanäle zu identifizieren.

>[!PREREQUISITES]
>
>[Programm-Analyzer erstellen](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/create-a-program-analyzer.md)

1. Klicken Sie auf **Analytics** in **My Marketo**.

   ![](assets/image2014-9-17-18-3a36-3a13.png)

1. Wählen Sie Ihre **Programm-Analyzer**.

   ![](assets/image2014-9-17-18-3a36-3a40.png)

1. Ändern Sie die Ansicht in **Nach Kanal**.

   ![](assets/image2014-9-17-18-3a36-3a59.png)

1. Verwenden Sie die **X Achse** Dropdown, um eine Metrik für die horizontale Achse auszuwählen. Fangen wir mit **Programmkosten**.

   ![](assets/image2014-9-17-18-3a37-3a7.png)

1. Verwenden Sie die Dropdownliste Y-Achse , um eine Metrik für die vertikale Achse auszuwählen. Hier gehen wir **(FT) Pipeline erstellt**.

   ![](assets/image2014-9-17-18-3a37-3a50.png)

   >[!NOTE]
   >
   >Viele der Metriken, die Sie im Programm-Analyzer auswählen können, stehen bei Erstkontakt- (FT-) und Multi-Touch-(MT-)Berechnungen zur Verfügung. Es ist wichtig, die [Differenz zwischen FT- und MT-Attribution](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

1. Verwenden Sie die **Y-Achse** Dropdown zur Auswahl **(MT) Pipeline erstellt**.

   ![](assets/image2014-9-17-18-3a39-3a5.png)

   In dieser Multi-Touch-Attributionsansicht sehen wir, dass der Webinar-Kanal einen größeren Einfluss auf die erstellte Pipeline hat und weniger kostet als die Tradeshow- und Online-Werbekanäle.

   Fügen wir nun zwei weitere Dimensionen hinzu!

1. Verwenden Sie die **Blasengröße** in der Dropdown-Liste eine zusätzliche Kennzahl auswählen, z. B. **Neue Namen**.

   ![](assets/image2014-9-17-18-3a39-3a36.png)

1. Sehen Sie sich an, wie sich das Diagramm ändert.

   ![](assets/image2014-9-17-18-3a39-3a55.png)

   Wir sehen, dass der Webinar-Kanal schrumpft, gemessen durch **Neue Namen**. Wir können zu dem Schluss kommen, dass es zwar viele Mitglieder hat, aber weniger effektiv ist, neue Leads zu erzeugen als der Tradeshow-Kanal.

1. Verwenden Sie abschließend das Dropdown-Menü Farbe , um die vierte Dimension hinzuzufügen. Wählen Sie **(FT) Umsatz gewinnt**.

   ![](assets/image2014-9-17-18-3a41-3a7.png)

1. Sehen Sie sich die Farbänderungen in Ihrem Diagramm an.

   ![](assets/image2014-9-17-18-3a41-3a19.png)

   Aus den Farben erfahren wir, dass der Kanal Tradeshow, die grünste Blase, den höchsten erzielten Umsatz beeinflusst hat, gemessen durch Erstkontakt-Attribution.

1. Wenn wir jetzt die Farbmetrik in **(MT) Umsatz gewinnt**, sehen wir, dass der Online-Advertising-Kanal, der jetzt grünste Kanal, mehr Umsatz beeinflusst hat - im Zeitverlauf - als die Webinar- und Tradeshow-Kanäle.

   ![](assets/image2014-9-17-18-3a41-3a40.png)

In unserem Beispiel sehen wir, dass der Kanal Tradeshow sowohl der teuerste (am weitesten rechts) als auch der erfolgreichste (am höchsten auf der Y-Achse) ist, wenn es darum geht, die durch Erstkontakt erstellte Pipeline zu messen. Betrachten wir nun die Pipeline jedes Kanals, die anhand der Multi-Touch-Attribution erstellt wurde.

>[!TIP]
>
>Die Beispiele in diesen Schritten messen die Effektivität basierend auf der erstellten Pipeline. Verwenden Sie die Dropdown-Liste Y-Achse , um andere Möglichkeiten zur Messung der Kanalwirksamkeit auszuwählen, z. B. neue Namen, Mitglieder, Kosten pro Erfolg usw.

>[!MORELIKETHIS]
>
>* [Kennenlernen von Programm- und Kanaldetails mit dem Programm-Analyzer](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/explore-program-and-channel-details-with-the-program-analyzer.md)
>* [Vergleichen der Programmwirksamkeit mit dem Programm-Analyzer](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/compare-program-effectiveness-with-the-program-analyzer.md)

