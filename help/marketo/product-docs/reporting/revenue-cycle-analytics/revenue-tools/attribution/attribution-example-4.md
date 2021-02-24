---
unique-page-id: 7514151
description: Namensnennungsbeispiel 4 - Marketing Docs - Produktdokumentation
title: Zuordnungsbeispiel 4
translation-type: tm+mt
source-git-commit: fa4ab03b98ac922e10c6daf3647dc460c12244d3
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---


# Zuordnungsbeispiel 4 {#attribution-example}

Lesen Sie das folgende Szenario und versuchen Sie, die Zahlen zu ermitteln, die im Raster angezeigt werden sollen.

* 11. April | Michelle downloads e-Book (Content) - Erfolg
* 15. April | John besucht (Webinar) - Erfolg
* 22. April | (Chance 1) für 3.000 $ erstellt
* 24. April | (Chance 2) für 5.000 $ erstellt
* 25. April | John und Michelle sind mit **beide** Optionen verknüpft.
* 29. April | [Option 1] ist geschlossen

| Name des Programms | (Inhalt) | (Webinar) |
|---|---|---|
|  | (Option 1) | (Option 2) | (Option 1) | (Option 2) |
| (MT) Opty Created | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Pipeline erstellt | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT) Umsatz gewinnbringend | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**Antworten anzeigen**

>[!NOTE]
>
>**Erläuterung**
>
>Wenn Sie mehrere Möglichkeiten und mehrere Programm-Erfolgspersonen haben, müssen Sie die Gutschrift zwischen den Menschen und den Programmen aufteilen. Beachten Sie jedoch, dass die Gutschrift für Chancen 1 und 2 nicht kombiniert werden. Jede Bewertung ist eine eigene Bonitätsbewertung.
>
>Wenn viele Leute involviert sind, berechnet Marketo automatisch die Bruchteile einer Gelegenheit, um die Gutschrift zu geben.

>[!NOTE]
>
>**Zuordnungsregeln**
>
>1. Die Gutschrift wird gleichmäßig aufgeteilt
>1. Du kannst dir nicht mehr gutschreiben, als du verdient hast
>1. Man kann etwas nicht für etwas verantwortlich machen, das in der Vergangenheit passiert ist


Probieren Sie alle Beispiele aus und Sie werden ein Zuordnungs-Pro!

>[!MORELIKETHIS]
>
>* [Zuordnungsbeispiel 1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [Zuordnungsbeispiel 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Zuordnungsbeispiel 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)

