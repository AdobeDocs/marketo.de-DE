---
unique-page-id: 7514146
description: Attributionsbeispiel 2 - Marketo-Dokumente - Produktdokumentation
title: Attributionsbeispiel 2
exl-id: 8f00abb5-85f8-4f05-874e-57aa6442548c
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 4%

---

# Attributionsbeispiel 2 {#attribution-example}

Lesen Sie das folgende Szenario und versuchen Sie, die Zahlen zu bestimmen, die im Raster enthalten sein sollen.

* &#x200B;11. April | Rechnung wird erworben von (Fachmesse)
* &#x200B;15. April | Joan wurde erworben von (Webinar)
* &#x200B;22. April | (Opportunity 1) für 6.000 $ erstellt
* &#x200B;24. April | (Opportunity 2) für 10.000 $ erstellt
* &#x200B;25. April | Bill und Joan sind Rollen von (**)** zugeordnet
* &#x200B;29. April | (Opportunity 1) wurde abgeschlossen

| Programmname | (Fachmesse) | (Webinar) |
|---|---|---|
| (FT) leer erstellt | `<pre>1</pre>` | `<pre>1</pre>` |
| (FT) Erstellte Pipeline | `<pre>$8,000</pre>` | `<pre>$8,000</pre>` |
| (FT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (FT) Gewonnener Ertrag | `<pre>$3,000</pre>` | `<pre>$3,000</pre>` |

**Antworten anzeigen**

>[!NOTE]
>
>**Erläuterung**
>
>Da sowohl Bill als auch Joan Rollen zugeordnet wurden, um **BEIDE** Opportunitys, teilte das System (gemäß den Regeln) die Gutschrift gleichmäßig zwischen ihnen auf.
>
>Die für jedes Programm erstellte Pipeline (8.000 $) entspricht der Hälfte der insgesamt verfügbaren Pipeline (16.000 $), die als Gutschrift vergeben werden kann.

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
>* [Attributionsbeispiel 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Attributionsbeispiel 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
