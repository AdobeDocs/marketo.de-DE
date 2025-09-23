---
unique-page-id: 7514126
description: Attributionsbeispiel 1 - Marketo-Dokumente - Produktdokumentation
title: Attributionsbeispiel 1
exl-id: 851cbad3-0f6d-4ea0-857f-8b15337c7540
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 7%

---

# Attributionsbeispiel 1 {#attribution-example}

Lesen Sie das folgende Szenario und versuchen Sie, die Zahlen zu bestimmen, die im Raster enthalten sein sollen.

* &#x200B;11. April | Fred wird erworben von (Fachmesse)
* &#x200B;15. April | Margo nimmt teil (Webinar) - Erfolg
* &#x200B;22. April | Fred ist mit der Opportunity verknüpft (Rolle).
* &#x200B;22. April | Opportunity wird für 3.000 $ erstellt

| Programmname | (Fachmesse) | (Webinar) |
|---|---|---|
| (FT) leer erstellt | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT) Erstellte Pipeline | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT) Opty Won | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT) Gewonnener Ertrag | `<pre>0</pre>` | `<pre>0</pre>` |

**Antworten anzeigen**

>[!NOTE]
>
>**Erläuterung**
>
>Zunächst ist zu verstehen, dass einige Typen COUNTS und andere WÄHRUNG sind. „Opty Created“ ist eine Zahl, eine Ganzzahl. Pipeline ist eine Währung. In Marketo entspricht die Währung den Einstellungen für Ihr Admin-Gebietsschema.
>
>Der Grund, warum die Messe alle Anerkennung erhielt, ist, dass Margo nicht mit einer Rolle in der Opportunity in Verbindung gebracht wurde. Keine Rolle, keine Anerkennung.

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
>* [Attributionsbeispiel 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Attributionsbeispiel 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Attributionsbeispiel 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
