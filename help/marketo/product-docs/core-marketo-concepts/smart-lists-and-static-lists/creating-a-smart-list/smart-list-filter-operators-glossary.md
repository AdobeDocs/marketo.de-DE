---
unique-page-id: 557312
description: Glossar zu Operatoren für intelligente Listenfilter - Marketo-Dokumente - Produktdokumentation
title: Glossar zu Operatoren für intelligente Listenfilter
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 12%

---

# Glossar zu Operatoren für intelligente Listenfilter {#smart-list-filter-operators-glossary}

Ein Operator ist Teil der Smart-Liste, mit der Sie bestimmte Kriterien erfüllen können. Damit können Sie Ihren Trigger oder Filter in einfacher Sprache beschreiben. Die verfügbaren Operatoren unterscheiden sich je nach Feldtyp.

Im Folgenden finden Sie ein Glossar, in dem die einzelnen Operatoren beschrieben werden.

## Datumsfelder {#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

Wenn Sie einen Operator auswählen, ändert sich die rechte Seite dynamisch.

| Benutzerin oder Benutzer | Rechts Seite | Beschreibung |
|---|---|---|
| ist | Einzeldatum | genaue Datumsübereinstimmung |
| ist nicht | Einzeldatum | Jedes Datum außer dem angegebenen |
| zwischen | Zwei Datumsfelder | Jedes Datum einschließlich und zwischen zwei angegebenen Daten |
| in der Vergangenheit | Natürliche Spracheingabe&#42; | Siehe Diagramm unten |
| in der Vergangenheit vor | Natürliche Spracheingabe&#42; | Siehe Diagramm unten |
| in der Zukunft | Natürliche Spracheingabe&#42; | Siehe Diagramm unten |
| in der Zukunft nach | Natürliche Spracheingabe&#42; | Siehe Diagramm unten |
| in Zeitrahmen | Vorgaben (letztes Quartal, gestern usw.) | Definiert in picklist |
| nach | Einzeldatum | Alle Datensätze nach dem angegebenen Datum |
| vor | Einzeldatum | Alle Datensätze vor dem angegebenen |
| am oder nach | Einzeldatum | siehe &quot;after&quot;, aber inklusive |
| am oder vor | Einzeldatum | siehe &quot;before&quot;, aber inklusiv |
| ist leer | Keine | Alle Datensätze ohne Datum |
| ist nicht leer | Keine | Alle Datensätze mit beliebigem Datum |

&#42; Die natürliche Spracheingabe ist cool. Im Folgenden finden Sie einige der Muster, die Sie eingeben können:

* 1 Stunde
* 82 Tage
* 3 Wochen
* 14 Monate
* 1 Jahr

Geben Sie einfach die Nummer und Einheit zusammen und es wird funktionieren!

>[!NOTE]
>
>&quot;In der Vergangenheit&quot; **does** den Tag (bis zur Uhrzeit, nicht nach), an dem Sie Ihre Smart-Liste erstellen.

>[!CAUTION]
>
>Wenn Sie eine intelligente Liste mit einem Datumsfeldfilter erstellen (z. B. Geburtsdatum, SFDC-Erstellungsdatum) und die Begrenzungen verwenden **before**, **auf oder vor** oder **früher**, werden in die intelligente Liste auch Personen aufgenommen, die in dem Datumsfeld keinen Wert haben.

Verwenden Sie das folgende Diagramm, um die Unterschiede zwischen den Datumsoperatoren zu verstehen.

![](assets/image2014-9-10-17-3a15-3a58.png)

>[!NOTE]
>
>**Beispiel**
>
>Datumsfelder können schwierig werden, wenn Sie mit vergangenen und zukünftigen Ereignissen arbeiten. Hier sind einige Beispiele.
>
>**In der Vergangenheit**
>
>Verwenden Sie diesen Operator, um für Ihre neue Werbeaktion E-Mails nur an Personen zu senden, die Ihren Dienst nicht innerhalb eines Jahres abonniert oder erneuert haben oder noch nie Abonnenten waren.
>
>**In Zukunft nach**
>
>Nehmen Sie an, Sie möchten Kunden sehen, die in 90 Tagen eine Verlängerung beantragen. Sie würden zwei separate Filter verwenden. Verwenden Sie zunächst &quot;In der Zukunft nach 90 Tagen&quot;und dann &quot;In den kommenden 91 Tagen&quot;. Dadurch würde erfasst, wer in 90 Tagen ein Datum hat.

## Zeichenfolgenfelder {#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| Benutzerin oder Benutzer | Beschreibung |
|---|---|
| ist | Exakte Übereinstimmung (nicht zwischen Groß- und Kleinschreibung unterscheiden) |
| ist nicht | Alles außer exakter Übereinstimmung |
| beginnt mit | Erste Buchstaben der Zeichenfolge stimmen überein |
| beginnt nicht mit | Erste Buchstaben der Zeichenfolge stimmen NICHT überein |
| enthält | Alle Buchstaben zusammen in der Zeichenfolgenübereinstimmung (Beispiel: california, vermögen, also) |
| enthält nicht | Keine Buchstaben zusammen in der Zeichenfolge stimmen überein. (Umkehrung von &quot;enthält&quot;) |
| ist leer | Datensätze ohne Wert (NULL) |
| ist nicht leer | Datensätze mit ANY-Wert |

>[!TIP]
>
>Verwenden Sie positive gegenüber negative Operatoren. &quot;Ist nicht&quot;Filter müssen den gesamten Datensatz in Ihrer Instanz durchsuchen, was sehr zeitaufwendig sein kann. Positive &quot;is&quot;-Filter können effektivere Suchalgorithmen nutzen.

## Ganzzahlfelder {#integer-fields}

![](assets/image2014-9-10-17-3a16-3a14.png)

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Benutzerin oder Benutzer</th> 
   <th colspan="1" rowspan="1">Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1">ist</td> 
   <td colspan="1" rowspan="1">Exakte Zahlenübereinstimmung ( = 0 gibt beide Leads mit 0 zurück <em>und</em> NULL)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">ist nicht</td> 
   <td colspan="1" rowspan="1">Alles außer exakter Zahlenübereinstimmung</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">zwischen</td> 
   <td colspan="1" rowspan="1">Definieren Sie zwei Werte, um alle zwischen (einschließlich) zu finden.</td> 
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
   <td colspan="1" rowspan="1">Oberhalb des angegebenen (einschließlich)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">höchstens</td> 
   <td colspan="1" rowspan="1">Niedriger als der angegebene (einschließlich)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">ist leer</td> 
   <td colspan="1" rowspan="1">Datensätze ohne Wert (NULL) - null ist eine Zahl, es ist <em>not</em> NULL</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">ist nicht leer</td> 
   <td colspan="1" rowspan="1">Datensätze mit ANY-Wert (einschließlich Null)</td> 
  </tr> 
 </tbody> 
</table>

Wie Sie sehen können, machen diese Operatoren es einfach, Marketo-ese mit Flut zu sprechen!
