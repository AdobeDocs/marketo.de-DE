---
unique-page-id: 7514151
description: Attributionsbeispiel 4 - Marketo-Dokumente - Produktdokumentation
title: Attributionsbeispiel 4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 3%

---

# Attributionsbeispiel 4 {#attribution-example}

Lesen Sie das folgende Szenario und versuchen Sie, die Zahlen zu ermitteln, die im Raster angezeigt werden sollen.

* 11. April | Michelle downloads e-Book (Content) - Erfolg
* 15. April | John besucht (Webinar) - Erfolg
* 22. April | (Chance 1) erstellt für 3.000 $
* 24. April | (Chancen 2) erstellt für 5.000 $
* 25. April | John und Michelle sind **beide** Optionen zugeordnet
* 29. April | [Opty 1] is Closed-Won

| Programmname | (Inhalt) | (Webinar) |
|---|---|---|
|   | (Option 1) | (Option 2) | (Option 1) | (Option 2) |
| (MT) Opty Created | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Erstellte Pipeline | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT) Gewonnener Ertrag | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**Antworten anzeigen**

>[!NOTE]
>
>**Erklärung**
>
>Wenn Sie mehrere Möglichkeiten und mehrere Personen mit Programmerfolg haben, müssen Sie die Gewichtung zwischen Personen und Programmen aufteilen. Beachten Sie jedoch, dass die Gutschrift für die Chancen 1 und 2 nicht kombiniert wird. Jede ist eine eigene Bonitätsbeurteilung.
>
>Wenn viele Personen beteiligt sind, berechnet Marketo automatisch die Bruchteile einer Chance, die man sich zutraut.

>[!NOTE]
>
>**Attributionsregeln**
>
>1. Die Gewichtung wird gleichmäßig aufgeteilt
>1. Du kannst nicht mehr Guthaben als du verdient hast
>1. Man kann etwas, das in der Vergangenheit passiert ist, nicht zuschreiben

Probieren Sie alle Beispiele aus und Sie werden ein Attributionsprofi sein!

>[!MORELIKETHIS]
>
>* [Attributionsbeispiel 1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [Attributionsbeispiel 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Attributionsbeispiel 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
