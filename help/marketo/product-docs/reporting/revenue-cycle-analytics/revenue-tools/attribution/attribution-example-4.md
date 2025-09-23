---
unique-page-id: 7514151
description: Attributionsbeispiel 4 - Marketo-Dokumente - Produktdokumentation
title: Attributionsbeispiel 4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 6%

---

# Attributionsbeispiel 4 {#attribution-example}

Lesen Sie das folgende Szenario und versuchen Sie, die Zahlen zu bestimmen, die im Raster enthalten sein sollen.

* &#x200B;11. April | Michelle lädt E-Book herunter (Inhalt) - Erfolg
* &#x200B;15. April | John nimmt teil (Webinar) - Erfolg
* &#x200B;22. April | (Opportunity 1) für 3.000 $ erstellt
* &#x200B;24. April | (Opportunity 2) für 5.000 $ erstellt
* &#x200B;25. April | John und Michelle sind mit Optys **beide** verbunden
* &#x200B;29. April | [Opty 1] ist abgeschlossen gewonnen

| Programmname | (Inhalt) | (Webinar) |
|---|---|---|
|   | (leer 1) | (leer 2) | (leer 1) | (leer 2) |
| (MT) leer erstellt | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Erstellte Pipeline | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT) Gewonnener Ertrag | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**Antworten anzeigen**

>[!NOTE]
>
>**Erläuterung**
>
>Wenn Sie mehrere Opportunities und mehrere Personen mit Programmerfolg haben, müssen Sie die Gutschrift auf die Personen und Programme aufteilen. Beachten Sie jedoch, dass die Gutschrift für Opportunity 1 und Opportunity 2 nicht kombiniert wird. Jedes ist eine eigene Bonitätsbeurteilung.
>
>Wenn viele Personen involviert sind, berechnet Marketo automatisch den Teil einer Chance, für den man Anerkennung zollen kann.

>[!NOTE]
>
>**Attributionsregeln**
>
>1. Die Kredite werden gleichmäßig aufgeteilt
>1. Man kann nicht mehr zuschreiben, als man verdient
>1. Man kann nicht für etwas verantwortlich machen, das in der Vergangenheit passiert ist

Probieren Sie alle Beispiele aus und Sie werden ein Attribution-Profi!

>[!MORELIKETHIS]
>
>* [Attributionsbeispiel 1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [Attributionsbeispiel 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Attributionsbeispiel 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
