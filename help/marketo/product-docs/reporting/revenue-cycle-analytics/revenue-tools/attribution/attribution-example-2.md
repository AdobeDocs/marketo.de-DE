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

Lesen Sie das folgende Szenario und versuchen Sie, die Zahlen zu ermitteln, die im Raster angezeigt werden sollen.

* 11. April | Bill wird von (Tradeshow) erworben
* 15. April | Joan wird von (Webinar) erworben
* 22. April | (Chance 1) erstellt für 6.000 $
* 24. April | (Chancen 2) erstellt für 10.000 $
* 25. April | Bill und Joan sind mit den Rollen **BEIDE** Optionen verknüpft.
* 29. April | (Chancen 1) ist geschlossen

| Programmname | (Gewerbeproben) | (Webinar) |
|---|---|---|
| (FT) Option erstellt | `<pre>1</pre>` | `<pre>1</pre>` |
| (FT) Erstellte Pipeline | `<pre>$8,000</pre>` | `<pre>$8,000</pre>` |
| (FT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (FT) Gewonnener Ertrag | `<pre>$3,000</pre>` | `<pre>$3,000</pre>` |

**Antworten anzeigen**

>[!NOTE]
>
>**Erklärung**
>
>Da sowohl Bill als auch Joan mit den Rollen verknüpft waren, um **BEIDE** Gelegenheiten zu bieten, teilte das System (gemäß den Regeln) den Kredit gleichmäßig zwischen ihnen auf.
>
>Die für jedes Programm erstellte Pipeline ($ 8.000) entspricht der Hälfte der insgesamt als Gutschrift verfügbaren Pipeline ($16.000).

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
>* [Attributionsbeispiel 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Attributionsbeispiel 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
