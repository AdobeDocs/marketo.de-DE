---
unique-page-id: 7514126
description: Zuordnungsbeispiel 1 - Marketing-Dokumente - Produktdokumentation
title: Zuordnungsbeispiel 1
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---


# Zuordnungsbeispiel 1 {#attribution-example}

Lesen Sie das folgende Szenario und versuchen Sie, die Zahlen zu ermitteln, die im Raster angezeigt werden sollen.

* 11. April | Fred wird von (Tradeshow) erworben
* 15. April | Margo-Teilnehmer (Webinar) - Erfolg
* 22. April | Fred ist (Rolle) mit der Gelegenheit verbunden
* 22. April | Die Möglichkeit wird für 3.000 $ geschaffen

| Name des Programms | (Diashow) | (Webinar) |
|---|---|---|
| (FT) Option erstellt | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT) Pipeline erstellt | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT) Opty Won | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT) Umsatz gewinnt | `<pre>0</pre>` | `<pre>0</pre>` |

**Antworten anzeigen**

>[!NOTE]
>
>**Erläuterung**
>
>Erstens ist zu verstehen, dass einige Typen ZÄHLEN und andere WÄHRUNG sind. Option erstellt ist eine Zahl, eine Ganzzahl. Pipeline ist eine Währung. In Marketo entspricht die Währung den Einstellungen für das Gebietsschema Ihrer Administratoren.
>
>Der Grund, warum die Tradeshow alle Gutschriften erhalten hat, ist, weil Margo nicht mit einer Rolle in der Gelegenheit verbunden war. Keine Rolle, keine Gutschrift.

>[!NOTE]
>
>**Zuordnungsregeln**
>
>1. Die Gutschrift wird gleichmäßig aufgeteilt
>1. Du kannst dir nicht mehr gutschreiben, als du verdient hast
>1. Man kann etwas nicht für etwas verantwortlich machen, das in der Vergangenheit passiert ist


Probieren Sie alle Beispiele aus und Sie werden ein Zuordnungs-Pro!

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Zuordnungsbeispiel 2](attribution-example-2.md)
>* [Zuordnungsbeispiel 3](attribution-example-3.md)
>* [Zuordnungsbeispiel 4](attribution-example-4.md)

