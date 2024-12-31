---
unique-page-id: 2951877
description: Grundlegendes zum Bereich „Programm-Opportunity-Analyse“ - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zum Bereich „Programm-Opportunity-Analyse“
exl-id: 6105df93-b3de-4929-85e3-fd328372bd24
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 20%

---

# Grundlegendes zum Bereich „Programm-Opportunity-Analyse“ {#understanding-the-program-opportunity-analysis-area}

## Überblick {#overview}

Im Bereich Opportunity-Analyse des Programms können Sie die Effektivität einzelner Programme analysieren oder nach Programmkanal zusammengefasste Ergebnisse anzeigen.

**Beispielhafte Geschäftsfragen, die Sie mit diesem Analysebereich beantworten können, sind**:

Wie viele Opportunities waren mit einem bestimmten Programm verbunden und wie viele haben wir gewonnen?

![](assets/one-1.png)

Wie viel Umsatz hat ein bestimmtes Programm oder ein bestimmter Kanal generiert?

![](assets/two-1.png)

Wie hoch sind meine Einnahmen aus Investitionen für ein bestimmtes Programm oder einen bestimmten Kanal?

![](assets/three-1.png)

Welche Möglichkeiten hat ein bestimmtes Programm beeinflusst?

![](assets/four-1.png)

## Programm-Opportunity-Analyse Attributionsmaßnahmen (blaue Punkte) {#program-opportunity-analysis-attribution-measures-blue-dots}

Für die Analyse verfügbare Kennzahlen sind im Allgemeinen Zahlen und werden durch blaue Punkte dargestellt. Dimensionen sind Attribute, die unterschiedliche Auffassungen zu den Kennzahlen vermitteln und durch gelbe Punkte dargestellt werden.

Alle Kennzahlen (blaue Punkte) beziehen sich auf die Attribution - die „Gutschrift“ für die Lead-Akquise oder für den mit einem Lead verbundenen Verkaufserfolg.

![](assets/six.five.png) ![](assets/seven-1.png)

Es gibt drei Arten von Maßnahmen:

* Akquisitionsbezogene Kennzahlen, die eine Attribution auf Erstkontakt (First-Touch Attribution, FT) erhalten.
* Erfolgsbezogene Kennzahlen, die eine Multi-Touch-Attribution (MT) erhalten.
* Verschiedene programmbezogene Maßnahmen, einschließlich der durchschnittlichen Anzahl der Marketing-Kontakte vor der Erstellung oder dem Abschluss von Opportunities.

## Akquise und erfolgsbezogene Maßnahmen {#acquisition-and-success-related-measures}

Akquisitionsbezogene Maßnahmen verleihen dem Programm Anerkennung, über das die Kontaktinformationen eines Leads zunächst abgerufen werden. Ein Lead muss in einem Programm für die Vergabe von Akquisitionskrediten keinen Erfolg erzielen.

Der Wert der Akquise eines bestimmten Leads ändert sich im Laufe der Zeit. Es ist null, bis ein Kauf vom Lead getätigt wird. Sie kann dann mit zusätzlichen Käufen zunehmen.

Erfolgsbezogene Maßnahmen rechnen alle Programme an, die zum Fortschritt eines Leads im Hinblick auf einen Kauf beitragen.

Wie bei der Akquise ändert sich der Wert des Beitrags zu den Umsätzen, die an einem Lead getätigt werden, im Laufe der Zeit und beträgt null, bis ein Kauf vom Lead getätigt wird.

<table> 
 <tbody> 
  <tr> 
   <th>Attributionskennzahl - Opportunity-bezogen (FT oder MT)*</th> 
   <th>Beschreibung</th> 
  </tr> 
  <tr> 
   <td>Opportunity-Kosten</td> 
   <td>Der Teil der Kosten des Programms, der die Opportunity beeinflusst hat. Die Kosten können aufgeteilt werden, wenn mehrere Leads beteiligt waren.</td> 
  </tr> 
  <tr> 
   <td>Opportunities erstellt</td> 
   <td>Der Teil der Gutschrift, den das Programm für die Beeinflussung der Erstellung der Opportunity erhalten hat. Es kann sich um einen Bruchteil handeln, falls mehrere Leads beteiligt waren.</td> 
  </tr> 
  <tr> 
   <td>Gewonnene Chancen</td> 
   <td>Der Anteil des Werts, den das Programm für die Beeinflussung der gewonnenen Opportunity erhalten hat. Es kann sich um einen Bruchteil handeln, falls mehrere Leads beteiligt waren.</td> 
  </tr> 
  <tr> 
   <td>Pipeline erstellt</td> 
   <td>Der Gutschriftanteil (als Geldwert), den das Programm für seine Einflussnahme auf die Schaffung einer neuen Chance erhalten hat. Es kann sich um einen Bruchteil handeln, falls mehrere Leads beteiligt waren.</td> 
  </tr> 
  <tr> 
   <td>Pipeline erstellt - noch offen</td> 
   <td>Der Gutschriftanteil (als Geldwert), den das Programm für seine Einflussnahme auf die Schaffung der aktuell offenen Chance erhalten hat. Es kann sich um einen Bruchteil handeln, falls mehrere Leads beteiligt waren.</td> 
  </tr> 
  <tr> 
   <td>Erwarteter Umsatz</td> 
   <td>Der Gutschriftanteil (als Geldwert), den das Programm für seine Einflussnahme auf die Schaffung einer neuen Chance erhalten hat. Der erwartete Umsatz ist die Chancenwahrscheinlichkeit multipliziert mit dem Chancenwert. Es kann sich um einen Bruchteil handeln, falls mehrere Leads beteiligt waren.</td> 
  </tr> 
  <tr> 
   <td>Ertrag aus Investitionen</td> 
   <td>Dies ist das Verhältnis von Programmkosten zum Gutschriftanteil (als Geldwert), den das Programm für die Einflussnahme gewonnener Chancen erhalten hat.</td> 
  </tr> 
  <tr> 
   <td>Gewonnener Ertrag</td> 
   <td>Der Gutschriftanteil (als Geldwert), den das Programm für seine Einflussnahme erhalten hat, hat eine Chance gewonnen. Es kann sich um einen Bruchteil handeln, falls mehrere Leads beteiligt waren.</td> 
  </tr> 
 </tbody> 
</table>

_&#42;(FT) = Erstkontakt-Attribution, verwendet für Messwerte der Lead-Akquise; (MT) = Mehrkontakt-Attribution, verwendet für Messwerte des Lead-Erfolgs_

Im Folgenden finden Sie ein Szenario, das beschreibt, wie Opportunity-Einheiten berechnet werden, wenn es zwei Programme gibt, die Leads generiert haben, die jedoch zu einer Opportunity aus demselben Konto führen.

**Programm 1**

* Erzeugt einen Lead: Lead 1
* Lead 1 stammt aus Konto 1

**Programm 2**

* Erstellt einen weiteren Lead: Lead 2
* Lead 2 stammt auch von Konto 1

**Konto 1**

* Erzeugt eine Opportunity: Opportunity 1

Marketo schreibt Chancen angemessen zu, ohne sie programmübergreifend zu verdoppeln. In diesem Fall erhält also jedes Programm 0,5 Opportunity-Einheiten. Das heißt, jedes Programm erhält die Hälfte der Gutschrift für die generierte Opportunity. Außerdem wird jedem Programm die Hälfte des mit der Opportunity verbundenen Umsatzes zugewiesen.

## Verschiedene programmbezogene Maßnahmen {#miscellaneous-program-related-measures}

Die anderen verfügbaren Maßnahmen spiegeln die Gesamtleistung des Programms wider.

<table> 
 <tbody> 
  <tr> 
   <th>Attributionsmaßnahme - programmbezogen</th> 
   <th>Beschreibung</th> 
  </tr> 
  <tr> 
   <td>Anzahl der mit dem Programm verknüpften Opportunitys</td> 
   <td><p>Die Gesamtzahl der Opportunitys, die einem Programm irgendeine Art von Attribution zugeschrieben hatten. Opportunities können durch eine oder mehrere Leads und ein oder mehrere Programme beeinflusst werden.</p></td> 
  </tr> 
  <tr> 
   <td>Durchschn. Anzahl der Erfolge pro abgeschlossener Opportunity</td> 
   <td>Die durchschnittliche Anzahl der Programmerfolge vor Abschluss der Opportunity. <br></td> 
  </tr> 
  <tr> 
   <td>Durchschn. Anzahl der Erfolge pro erstellter Opportunity</td> 
   <td>Die durchschnittliche Anzahl der Programmerfolge vor der Erstellung der Opportunity.</td> 
  </tr> 
  <tr> 
   <td>Neue Namen</td> 
   <td>Die Gesamtzahl der neuen Namen, d. h. neuen Leads, die vom Programm erworben wurden.</td> 
  </tr> 
  <tr> 
   <td>Programmkosten</td> 
   <td>Gesamtkosten des Programms.</td> 
  </tr> 
  <tr> 
   <td>Erfolg (Summe)</td> 
   <td>Die Gesamtzahl der Programmmitglieder, die erfolgreich waren.</td> 
  </tr> 
 </tbody> 
</table>

## Dimensionen zur Analyse von Programmchancen (gelbe Punkte) {#program-opportunity-analysis-dimensions-yellow-dots}

Während Kennzahlen (blaue Punkte) berechnet werden und etwas Nachdenken und Erklärungen erfordern, sind Dimensionen (gelbe Punkte) beschreibend. Im Folgenden finden Sie die verfügbaren Dimensionen.

<table> 
 <tbody> 
  <tr> 
   <th>Kategorie</th> 
   <th>Vermerk anzeigen</th> 
  </tr> 
  <tr> 
   <td>Opportunity-Attribute</td> 
   <td>Opportunity geschlossen<br>Opportunity-Name*<br>Opportunity-Eigentümername<br>Opportunity-Stadium<br>Opportunity-Typ</td> 
  </tr> 
  <tr> 
   <td>Opportunity-Zeitrahmen</td> 
   <td>Opportunity geschlossen Jahr/Quartal/Monat<br>Opportunity erstellt Jahr/Quartal/Monat</td> 
  </tr> 
  <tr> 
   <td>Programmattribute</td> 
   <td>Programmkanal<br>Programmname</td> 
  </tr> 
  <tr> 
   <td>Zeitrahmen der Programmkosten</td> 
   <td>Kosten Jahr/Quartal/Monat</td> 
  </tr> 
 </tbody> 
</table>

*&#42;Alle Opportunities, die einem Programm eine beliebige Art von Attribution zugeschrieben haben. Opportunities können durch eine oder mehrere Leads und ein oder mehrere Programme beeinflusst werden.*

>[!MORELIKETHIS]
>
>[Erstellen eines Revenue Explorer-Berichts](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
