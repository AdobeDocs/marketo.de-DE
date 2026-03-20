---
unique-page-id: 7514149
description: Erfahren Sie mehr über Attributionsbeispiel 3 in Marketo Engage, einschließlich Attributionsbeispiel 3 Attributionsbeispiel. Verwenden Sie dieses Handbuch, um Ihren nächsten Schritt abzuschließen.
title: Attributionsbeispiel 3
exl-id: d8ca63a2-58de-4cde-b915-ff7f2e6468d9
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 50befbf7339cd7a8b25b0942515497f6acc8f9ab
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 6%

---

# Attributionsbeispiel 3 {#attribution-example}

Lesen Sie das folgende Szenario und versuchen Sie, die Zahlen zu bestimmen, die im Raster enthalten sein sollen.

* &#x200B;11. April | Steve Downloads (Inhalt) - Erfolg
* &#x200B;22. April | Opportunity wird für 3.000 $ erstellt (sowohl Steve als auch Jason haben Rollen)
* &#x200B;25. April | Jason nimmt teil (Webinar) - Erfolg
* &#x200B;30. April | Opportunity ist abgeschlossen gewonnen

| Attributionsmetrik | (Inhalt) | (Webinar) |
|---|---|---|
| (MT) leer erstellt | `<pre>1</pre>` | `<pre>0</pre>` |
| (MT) Erstellte Pipeline | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Gewonnener Ertrag | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**Antworten anzeigen**

>[!NOTE]
>
>**Erläuterung**
>
>#3 der Attributionsregel speichern. Jason hatte Programmerfolg, NACHDEM das Opty erstellt wurde. Daher wird dem Webinar die Entstehung der Opportunity nicht angerechnet. Nur die Anerkennung für den Opty gewonnen.
>
>Daher erhält (Content) 100 % der Credits für die Opty-Erstellung und Pipeline, aber nur 50 % der Credits für den gewonnenen Opty.

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
>* [Attributionsbeispiel 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
