---
unique-page-id: 7514149
description: Attributionsbeispiel 3 - Marketo-Dokumente - Produktdokumentation
title: Attributionsbeispiel 3
exl-id: d8ca63a2-58de-4cde-b915-ff7f2e6468d9
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 3%

---

# Attributionsbeispiel 3 {#attribution-example}

Lesen Sie das folgende Szenario und versuchen Sie, die Zahlen zu ermitteln, die im Raster angezeigt werden sollen.

* 11. April | Steve-Downloads (Inhalt) - Erfolg
* 22. April | Die Möglichkeit wird für 3.000 USD geschaffen (sowohl Steve als auch Jason haben Rollen)
* 25. April | Jason attends (Webinar) - success
* 30. April | Chancen sind geschlossen

| Attributionsmetrik | (Inhalt) | (Webinar) |
|---|---|---|
| (MT) Opty Created | `<pre>1</pre>` | `<pre>0</pre>` |
| (MT) Erstellte Pipeline | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Gewonnener Ertrag | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**Antworten anzeigen**

>[!NOTE]
>
>**Erklärung**
>
>Merken Sie sich die Zuordnungsregel Nr. 3. Jason hatte Programmerfolg NACH der Erstellung der Option. Daher kann das Webinar nicht für die Schaffung der Chance angesetzt werden. Nur für die &quot;Opty&quot;wird der Gewinn gutgeschrieben.
>
>Daher wird (Inhalt) 100 % der Gutschrift für die Erstellung und Pipeline von Opty zugeschrieben, aber nur 50 % der Gutschrift für die erzielte Opty.

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
>* [Attributionsbeispiel 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
