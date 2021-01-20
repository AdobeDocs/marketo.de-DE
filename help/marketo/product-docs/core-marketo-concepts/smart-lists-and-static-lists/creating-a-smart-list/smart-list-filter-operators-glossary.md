---
unique-page-id: 557312
description: Smart-Liste-Filteroperatoren - Glossar - Marketing Docs - Produktdokumentation
title: Glossar zu Operatoren für intelligente Liste
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---


# Filteroperatoren für intelligente Listen - Glossar {#smart-list-filter-operators-glossary}

Ein Operator ist ein Teil der intelligenten Liste, die Ihnen hilft, bestimmte Informationen zu erhalten. Damit können Sie Ihren Filter oder Trigger in einfacher Sprache beschreiben. Die verfügbaren Operatoren unterscheiden sich je nach Feldtyp.

Im Folgenden finden Sie ein Glossar, das die einzelnen Operatoren beschreibt.

## Datumsfelder {#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

Wenn Sie einen Operator auswählen, ändert sich die rechte Seite dynamisch.

| Operator | Rechts | Beschreibung |
|---|---|---|
| is | Einzeldatum | Genaue Datumsübereinstimmung |
| ist nicht | Einzeldatum | Jedes Datum außer dem angegebenen |
| between | Zwei Datumsfelder | Jedes Datum einschließlich und zwischen zwei angegebenen Daten |
| in der Vergangenheit | Natürliche Spracheingabe* | Siehe Diagramm unten |
| in der Vergangenheit | Natürliche Spracheingabe* | Siehe Diagramm unten |
| in Zukunft | Natürliche Spracheingabe* | Siehe Diagramm unten |
| in Zukunft nach | Natürliche Spracheingabe* | Siehe Diagramm unten |
| im Zeitrahmen | Vorgaben (letztes Quartal, gestern usw.) | Definiert in picklist |
| after | Einzeldatum | Alle Datensätze nach dem angegebenen Datum |
| before | Einzeldatum | Alle Datensätze vor dem angegebenen |
| on oder after | Einzeldatum | Wie &quot;after&quot;, aber inklusiv |
| am oder vor | Einzeldatum | Wie &quot;vorher&quot;, aber inklusiv |
| ist leer | Keines | Alle Datensätze ohne Datum |
| ist nicht leer | Keines | Alle Datensätze mit einem beliebigen Datum |

* Die natürliche Spracheingabe ist cool. Folgende Muster können Sie eingeben:

* 1 Stunde
* 82 Tage
* 3 Wochen
* 14 Monate
* 1 Jahr

Geben Sie einfach die Nummer und Einheit zusammen und es funktioniert!

>[!NOTE]
>
>&quot;In der Vergangenheit&quot; **bezieht** den Tag ein (bis zum Zeitpunkt, nicht danach), den Sie Ihre intelligente Liste erstellen.

>[!CAUTION]
>
>Wenn Sie eine intelligente Liste mit einem Datumsfeldfilter erstellen (z. B. Geburtsdatum, Erstellungsdatum des SFDC) und die **before**- oder **on- oder vor-**-Einschränkungen verwenden, umfasst die intelligente Liste auch Personen, die in diesem Datumsfeld keinen Wert haben.

Verwenden Sie das folgende Diagramm, um die Unterschiede zwischen den Datumsoperatoren zu verstehen.

![](assets/image2014-9-10-17-3a15-3a58.png)

>[!NOTE]
>
>**Beispiel**
>
>Datumsfelder können kompliziert werden, wenn Sie mit vergangenen und zukünftigen Ereignissen arbeiten. Hier sind einige Beispiele.
>
>**Früher**
>
>Für Ihre neue Promotion verwenden Sie diesen Operator, um E-Mails nur an Personen zu senden, die Ihren Dienst nicht innerhalb eines Jahres abonniert oder erneuert haben oder noch nie Abonnenten waren.
>
>**In Zukunft nach**
>
>Nehmen Sie an, Sie möchten Kunden sehen, die in 90 Tagen eine Verlängerung planen. Sie würden zwei separate Filter verwenden. Verwenden Sie zunächst &quot;In Zukunft nach 90 Tagen&quot; und dann &quot;In Zukunft 91 Tage&quot;. Dadurch würde erfasst werden, wer in 90 Tagen ein Datum hat.

## Zeichenfolgenfelder {#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| Operator | Beschreibung |
|---|---|
| is | Genaue Übereinstimmung (nicht zwischen Groß- und Kleinschreibung unterscheiden) |
| ist nicht | Alles außer genaue Übereinstimmung |
| beginn mit | Erste übereinstimmende Buchstaben einer Zeichenfolge |
| nicht Beginn mit | Erste Buchstaben der Zeichenfolge DO NOT match |
| contains | Alle Buchstaben in der Zeichenfolge stimmen überein (Beispiel: Kalifornien, Glück, also) |
| enthält nicht | Keine Buchstaben zusammen in der Zeichenfolge übereinstimmen. (Umkehrung von &quot;enthält&quot;) |
| ist leer | Datensätze ohne Wert (NULL) |
| ist nicht leer | Datensätze mit ANY-Werten |

>[!TIP]
>
>Verwenden Sie positive und negative Operatoren. &quot;Ist nicht&quot;-Filter müssen den gesamten Datensatz in Ihrer Instanz durchsuchen, was sehr zeitaufwendig sein kann. Positive &quot;is&quot;-Filter können effektivere Suchalgorithmen nutzen.

## Ganzzahlfelder {#integer-fields}

![](assets/image2014-9-10-17-3a16-3a14.png)

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Operator</th> 
   <th colspan="1" rowspan="1">Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1">is</td> 
   <td colspan="1" rowspan="1">Genaue Zahlenübereinstimmung ( = 0 gibt beide Leads mit 0 <em>und</em> NULL zurück)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">ist nicht</td> 
   <td colspan="1" rowspan="1">Alles außer exakte Zahlenübereinstimmung</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">between</td> 
   <td colspan="1" rowspan="1">Definieren Sie zwei Werte, um alle dazwischen zu finden (inklusive)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">größer als</td> 
   <td colspan="1" rowspan="1">Oberhalb der angegebenen</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">kleiner als</td> 
   <td colspan="1" rowspan="1">Kleiner als angegeben</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">mindestens</td> 
   <td colspan="1" rowspan="1">Über dem angegebenen (einschließlich)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">höchstens</td> 
   <td colspan="1" rowspan="1">Kleiner als die angegebene (einschließlich)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">ist leer</td> 
   <td colspan="1" rowspan="1">Datensätze ohne Wert (NULL) - null ist eine Zahl, es ist <em>nicht</em> NULL</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">ist nicht leer</td> 
   <td colspan="1" rowspan="1">Datensätze mit JEDEM Wert (einschließlich Null)</td> 
  </tr> 
 </tbody> 
</table>

Wie Sie sehen können, machen diese Operatoren es einfach, Marketo-ese mit Flauigkeit zu sprechen!
