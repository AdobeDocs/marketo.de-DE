---
unique-page-id: 7514126
description: Attributionsbeispiel 1 - Marketo-Dokumente - Produktdokumentation
title: Attributionsbeispiel 1
exl-id: 851cbad3-0f6d-4ea0-857f-8b15337c7540
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 5%

---

# Attributionsbeispiel 1 {#attribution-example}

Lesen Sie das folgende Szenario und versuchen Sie, die Zahlen zu ermitteln, die im Raster angezeigt werden sollen.

* 11. April | Fred wird von (Tradeshow) erworben
* 15. April | Margo attends (Webinar) - success
* 22. April | Fred wird (Rolle) mit der Gelegenheit verknüpft
* 22. April | Die Möglichkeit wird für 3.000 $ geschaffen

| Programmname | (Fachmesse) | (Webinar) |
|---|---|---|
| (FT) Option erstellt | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT) Erstellte Pipeline | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT) Opty Won | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT) Gewonnener Ertrag | `<pre>0</pre>` | `<pre>0</pre>` |

**Antworten anzeigen**

>[!NOTE]
>
>**Erklärung**
>
>Zunächst muss man verstehen, dass einige Typen ZÄHLEN und andere WÄHRUNGEN sind. Option erstellt ist eine Zählung, eine Ganzzahl. Die Pipeline ist eine Währung. In Marketo entspricht die Währung Ihren Gebietsschemaeinstellungen für Administratoren.
>
>Der Grund, warum die Tradeshow alle Anerkennung erhielt, ist, dass Margo nicht mit einer Rolle in der Gelegenheit verbunden war. Keine Rolle, keine Gutschrift.

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
>* [Attributionsbeispiel 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Attributionsbeispiel 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Attributionsbeispiel 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

