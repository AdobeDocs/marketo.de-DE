---
unique-page-id: 557312
description: Glossar zu Operatoren für intelligente Listenfilter - Marketo-Dokumente - Produktdokumentation
title: Glossar zu Operatoren für intelligente Listenfilter
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
feature: Smart Lists
source-git-commit: 4bf27f7eb534ec76983a898d020f0b8c336a36dc
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 13%

---

# Glossar zu Operatoren für intelligente Listenfilter {#smart-list-filter-operators-glossary}

Ein Operator ist Teil der Smart-Liste, die Ihnen hilft, bestimmte Kriterien zu erfüllen. Damit können Sie Ihren Trigger oder Filter in einfacher Sprache beschreiben. Die verfügbaren Operatoren unterscheiden sich je nach Feldtyp.

Im Folgenden finden Sie ein Glossar, in dem die einzelnen Operatoren beschrieben werden.

## Datumsfelder {#date-fields}

![](assets/smart-list-filter-operators-glossary-1.png)

Wenn Sie einen Operator auswählen, ändert sich die rechte Seite dynamisch.

<table><thead>
  <tr>
    <th>Benutzerin oder Benutzer</th>
    <th>Rechts Seite</th>
    <th>Beschreibung</th>
  </tr></thead>
<tbody>
  <tr>
    <td>ist</td>
    <td>Einzeldatum</td>
    <td>genaue Datumsübereinstimmung</td>
  </tr>
  <tr>
    <td>ist nicht</td>
    <td>Einzeldatum</td>
    <td>Jedes Datum außer dem angegebenen</td>
  </tr>
  <tr>
    <td>zwischen</td>
    <td>Zwei Datumsfelder</td>
    <td>Jedes Datum einschließlich und zwischen zwei angegebenen Daten</td>
  </tr>
  <tr>
    <td>in Vergangenheit</td>
    <td>Natürliche Spracheingabe*</td>
    <td>Siehe Diagramm unten</td>
  </tr>
  <tr>
    <td>in der Vergangenheit vor</td>
    <td>Natürliche Spracheingabe*</td>
    <td>Siehe Diagramm unten</td>
  </tr>
  <tr>
    <td>in der Zukunft</td>
    <td>Natürliche Spracheingabe*</td>
    <td>Siehe Diagramm unten</td>
  </tr>
  <tr>
    <td>in der Zukunft nach</td>
    <td>Natürliche Spracheingabe*</td>
    <td>Siehe Diagramm unten</td>
  </tr>
  <tr>
    <td>in Zeitrahmen</td>
    <td>Vorgaben (letztes Quartal, gestern usw.)</td>
    <td>Definiert in picklist</td>
  </tr>
  <tr>
    <td>nach</td>
    <td>Einzeldatum</td>
    <td>Alle Datensätze nach dem angegebenen Datum</td>
  </tr>
  <tr>
    <td>vor</td>
    <td>Einzeldatum</td>
    <td>Alle Datensätze vor dem angegebenen</td>
  </tr>
  <tr>
    <td>am oder nach</td>
    <td>Einzeldatum</td>
    <td>siehe "after", aber inklusive</td>
  </tr>
  <tr>
    <td>Am oder vor</td>
    <td>Einzeldatum</td>
    <td>siehe "before", aber inklusiv</td>
  </tr>
  <tr>
    <td>ist leer</td>
    <td>Keine</td>
    <td>Alle Datensätze ohne Datum</td>
  </tr>
  <tr>
    <td>ist nicht leer</td>
    <td>Keine</td>
    <td>Alle Datensätze mit beliebigem Datum</td>
  </tr>
</tbody></table>

**&#42;** Die natürliche Spracheingabe ist cool. Im Folgenden finden Sie einige der Muster, die Sie eingeben können:

* 1 Stunde
* 82 Tage
* 3 Wochen
* 14 Monate
* 1 Jahr

Geben Sie einfach die Nummer und Einheit zusammen und es wird funktionieren!

>[!NOTE]
>
>&quot;In der Vergangenheit&quot; _enthält_ den Tag (bis zur Zeit, nicht nach), an dem Sie Ihre Smart-Liste erstellen.

>[!CAUTION]
>
>Wenn Sie eine Smart-Liste mit einem Datumsfeldfilter erstellen (z. B. Geburtsdatum, SFDC-Erstellungsdatum) und die Begrenzungen **[!UICONTROL vor]**, **[!UICONTROL vor oder vor]** oder **[!UICONTROL in der Vergangenheit vor]** verwenden, enthält die Smart-Liste auch Personen, die in diesem Datumsfeld keinen Wert haben.

Verwenden Sie das folgende Diagramm, um die Unterschiede zwischen den Datumsoperatoren zu verstehen.

![](assets/smart-list-filter-operators-glossary-2.png)

>[!NOTE]
>
>**Beispiel**
>
>Datumsfelder können schwierig werden, wenn Sie mit vergangenen und zukünftigen Ereignissen arbeiten. Hier sind einige Beispiele.
>
>**[!UICONTROL In vergangener Zeit vor]**
>
>Verwenden Sie diesen Operator, um für Ihre neue Werbeaktion E-Mails nur an Personen zu senden, die Ihren Dienst nicht innerhalb eines Jahres abonniert oder erneuert haben oder noch nie Abonnenten waren.
>
>**[!UICONTROL In Zukunft nach]**
>
>Nehmen Sie an, Sie möchten Kunden sehen, die in 90 Tagen eine Verlängerung beantragen. Sie würden zwei separate Filter verwenden. Verwenden Sie zunächst &quot;In der Zukunft nach 90 Tagen&quot;und dann &quot;In den kommenden 91 Tagen&quot;. Dadurch würde erfasst, wer in 90 Tagen ein Datum hat.

## Zeichenfolgenfelder {#string-fields}

![](assets/smart-list-filter-operators-glossary-3.png)

<table><thead>
  <tr>
    <th>Benutzerin oder Benutzer</th>
    <th>Beschreibung</th>
  </tr></thead>
<tbody>
  <tr>
    <td>ist</td>
    <td>Exakte Übereinstimmung (nicht zwischen Groß- und Kleinschreibung unterscheiden)</td>
  </tr>
  <tr>
    <td>ist nicht</td>
    <td>Alles außer exakter Übereinstimmung</td>
  </tr>
  <tr>
    <td>beginnt mit</td>
    <td>Erste Buchstaben der Zeichenfolge stimmen überein</td>
  </tr>
  <tr>
    <td>beginnt nicht mit</td>
    <td>Erste Buchstaben der Zeichenfolge stimmen NICHT überein</td>
  </tr>
  <tr>
    <td>enthält</td>
    <td>Alle Buchstaben zusammen in der Zeichenfolgenübereinstimmung (Beispiel: california, vermögen, also)</td>
  </tr>
  <tr>
    <td>enthält nicht</td>
    <td>Keine Buchstaben zusammen in der Zeichenfolge stimmen überein. (Umkehrung von "enthält")</td>
  </tr>
  <tr>
    <td>ist leer</td>
    <td>Datensätze ohne Wert (NULL)</td>
  </tr>
  <tr>
    <td>ist nicht leer</td>
    <td>Datensätze mit ANY-Wert</td>
  </tr>
</tbody>
</table>

>[!TIP]
>
>Verwenden Sie positive gegenüber negative Operatoren. &quot;Ist nicht&quot;Filter müssen den gesamten Datensatz in Ihrer Instanz durchsuchen, was sehr zeitaufwendig sein kann. Positive &quot;is&quot;-Filter können effektivere Suchalgorithmen nutzen.

## Ganzzahlfelder {#integer-fields}

![](assets/smart-list-filter-operators-glossary-4.png)

<table><thead>
  <tr>
    <th>Benutzerin oder Benutzer</th>
    <th>Beschreibung</th>
  </tr></thead>
<tbody>
  <tr>
    <td>ist</td>
    <td>Genaue Zahlenübereinstimmung ( = 0 gibt beide Leads mit 0 und NULL zurück.</td>
  </tr>
  <tr>
    <td>ist nicht</td>
    <td>Alles außer exakter Zahlenübereinstimmung</td>
  </tr>
  <tr>
    <td>zwischen</td>
    <td>Definieren Sie zwei Werte, um alle zwischen (einschließlich) zu finden.</td>
  </tr>
  <tr>
    <td>größer als</td>
    <td>Oberhalb der angegebenen</td>
  </tr>
  <tr>
    <td>kleiner als</td>
    <td>Kleiner als angegeben</td>
  </tr>
  <tr>
    <td>mindestens</td>
    <td>Oberhalb des angegebenen (einschließlich)</td>
  </tr>
  <tr>
    <td>höchstens</td>
    <td>Niedriger als der angegebene (einschließlich)</td>
  </tr>
  <tr>
    <td>ist leer</td>
    <td>Datensätze ohne Wert (NULL) - null ist eine Zahl, nicht NULL</td>
  </tr>
  <tr>
    <td>ist nicht leer</td>
    <td>Datensätze mit ANY-Wert (einschließlich Null)</td>
  </tr>
</tbody>
</table>

Wie Sie sehen können, machen diese Operatoren es einfach, Marketo-ese mit Flut zu sprechen!
