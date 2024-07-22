---
unique-page-id: 2951884
description: Grundlegendes zur Opportunity Analysis in Revenue Explorer - Marketo Docs - Produktdokumentation
title: Grundlegendes zur Opportunity Analysis in Umsatz-Explorer
exl-id: 2ef45d3e-7640-4c47-86ae-d7ae45ed1dd4
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 10%

---

# Grundlegendes zur Opportunity Analysis in Umsatz-Explorer {#understanding-opportunity-analysis-in-revenue-explorer}

Die Opportunity Analysis im Umsatz Explorer ermöglicht es Ihnen, Ihre Möglichkeiten auf einer tieferen Ebene zu untersuchen. Ordnen Sie die Daten basierend auf beliebigen Lead-/Firmenattributen wie Lead-Quelle, Branche oder Geografie zu. Analysieren Sie die Opportunitätserstellung und das Schließen anhand des Namens, der Phase oder der Wahrscheinlichkeit. Erfahren Sie mehr über die Marketing-Beiträge zur Pipeline.

## Beispielanalyse {#example-analysis}

Im Folgenden finden Sie einige Berichte, die Sie im Bereich Opportunity Analysis erstellen können.

1. Marketing-Einfluss auf erstellte Chancen

   Welchen Anteil der Pipeline Ihres Unternehmens haben Ihre Marketingprogramme beeinflusst? Dieser Bericht gibt Ihnen die Antwort. Die folgenden Tortendiagramme veranschaulichen den Prozentsatz der Anzahl aller Möglichkeiten und den Opportunitätsbetrag, die durch ein Marketingprogramm erworben wurden.

   ![](assets/image2015-7-21-16-3a21-3a4.png)

1. Marketing-Einfluss auf Chancen geschlossen und gewonnen

   Dieser Bericht zeigt, wie viel Umsatz durch das Marketing erzielt und beeinflusst wurde, nach Anzahl und Betrag.

   ![](assets/image2015-7-21-16-3a41-3a55.png)

1. Opportunity closed by Lead Source

   In diesem Bericht werden alle durch die Lead-Quelle geschlossenen Möglichkeiten aufgegliedert und Sie erhalten einen klaren Überblick darüber, welche Quellen funktionieren und welche nicht.

   ![](assets/image2015-7-21-10-3a34-3a50.png)

1. Zeit bis zum Schließen durch Source

   Dieser Bericht zeigt die Beziehung zwischen den durchschnittlichen Tagen, in denen eine Gelegenheit geschlossen wird, und der Hauptursache.

   ![](assets/image2015-7-21-10-3a35-3a3.png)

1. Open Opportunity and Staging

   Dieser Bericht zeigt, wie viele Möglichkeiten in den einzelnen Phasen des Umsatzzyklus offen sind.

   ![](assets/image2015-7-21-10-3a35-3a32.png)

1. Anzahl der Möglichkeiten nach Jahr nach Branche

   Dieser Bericht beantwortet die Frage: &quot;Erhalten wir von bestimmten Branchen Jahr für Jahr mehr oder weniger Möglichkeiten?&quot;

   ![](assets/image2015-7-21-10-3a35-3a45.png)

## Dimensionen und Maßnahmen zur Opportunitätsanalyse {#opportunity-analysis-dimensions-and-measures}

Die Opportunity Analysis bietet Ihnen Zugriff auf alle Lead-, Unternehmens- und Opportunity-bezogenen Dimensionen und Opportunity-bezogenen Maßnahmen. Nutzen Sie diese Dimensionen und Maßnahmen zur Opportunitätsanalyse, um spezifische Fragen in Ihrem Bericht zu beantworten.

1. Unternehmensattribute

   | Abmessung | Beschreibung |
   |---|---|
   | Jahresumsatz | Jahresumsatz des Unternehmens |
   | Ort | Die Stadt, in der das Unternehmen seinen Sitz hat |
   | Land | Der Bezirk, in dem sich das Unternehmen befindet |
   | Branche | Die Branche, in der sich das Unternehmen befindet |
   | Unternehmensname | Name des Unternehmens |
   | Anzahl der Mitarbeiter | Anzahl der Mitarbeiter im Unternehmen |
   | Postleitzahl | Postleitzahl des Unternehmens |
   | SIC-Code | SIC-Code des Unternehmens |
   | Bundesland | Der Staat, in dem sich das Unternehmen befindet |

1. Lead-Attribute

   | Abmessung | Beschreibung |
   |---|---|
   | Auf der Sperrliste | Der Blei wird auf die Blockierungsliste gesetzt |
   | In Chancen konvertiert | Der Lead wird in eine Chance umgewandelt |
   | E-Mail-Adresse ungültig | Gibt an, ob der Lead über eine gültige E-Mail-Adresse verfügt |
   | Marketing eingestellt | Wird der Lead von Marketing-E-Mails ausgesetzt? |
   | E-Mail-Adresse | E-Mail-Adresse des Interessenten |
   | Jobtitel | Berufsbezeichnung des Leiters |
   | Vollständiger Name | Vollständiger Name des Interessenten |
   | Ursprünglicher Quellentyp | Ursprünglicher Quelltyp des Leads |
   | Source Type registrieren | Der registrierte Quellentyp des Leads |
   | E-Mail-Adresse des Lead-Eigentümers | E-Mail-Adresse des Lead-Eigentümers |
   | Position des Lead-Eigentümers | Berufsbezeichnung des leitenden Eigentümers |
   | Name des Lead-Eigentümers | Name des Lead-Eigentümers |
   | Lead-Quelle | Lead-Quelle |
   | Lead-Status | Lead-Status |

1. Lead erstellter Zeitrahmen

   | Abmessung | Beschreibung |
   |---|---|
   | Lead erstellt Jahr | Das Jahr der Erstellung des Leads |
   | Lead Created Quarter | Das Quartal, in dem der Lead erstellt wurde |
   | Lead hat Monat erstellt | Der Monat der Lead-Erstellung |
   | Lead hat Woche erstellt | Die Woche, in der der Lead erstellt wird |
   | Lead Erstellungsdatum | Das Datum der Erstellung des Leads |

1. Opportunity-Attribute

   | Abmessung | Beschreibung |
   |---|---|
   | Geschlossene Chancen | Ist die Gelegenheit zu schließen? |
   | Opportunity-Prognosekategorie | Kategorie der Opportunity-Prognose |
   | Opportunity-Name | Opportunity name |
   | Opportunity-Stadium | Opportunity stage |
   | Opportunity-Typ | Opportunity-Typ |
   | Opportunity – Gewonnen | Ist diese Gelegenheit geschlossen und gewonnen? |
   | Von Marketing beeinflusste Chancen | Diese Markierung gibt an, ob einer der Lead/Kontakte von einem Marketingprogramm erworben wurde oder erfolgreich war. Es werden nur Programme berücksichtigt, deren Kosten für einen bestimmten Zeitraum festgelegt wurden. |

1. Opportunity Closed Timeframe

   | Abmessung | Beschreibung |
   |---|---|
   | Chancen - abgeschlossenes Jahr | Das Jahr, in dem die Gelegenheit geschlossen wird |
   | Geschlossenes Opportunity-Quartal | Das Quartal, in dem die Gelegenheit geschlossen wurde |
   | Chancen - Abgeschlossener Monat | Der Monat, in dem die Gelegenheit beendet wird |
   | Opportunity Closed Week | Die Woche, in der die Gelegenheit geschlossen wird |
   | Opportunity Closed Date | Das Datum, an dem die Gelegenheit geschlossen wird |

1. Erstellter Opportunity-Zeitrahmen

   | Abmessung | Beschreibung |
   |---|---|
   | Chancen - Erstellungsjahr | Das Jahr, in dem die Gelegenheit geschaffen wird |
   | Erstelltes Opportunity-Quartal | Das Quartal, in dem die Gelegenheit erstellt wurde |
   | Opportunity hat Monat erstellt | Der Monat, in dem die Gelegenheit erstellt wurde |
   | Opportunity hat Woche erstellt | Die Woche, in der die Gelegenheit geschaffen wird |
   | Opportunity-Erstellungsdatum | Das Datum, an dem die Gelegenheit erstellt wurde |

1. Kennzahlen

   | Messung | Beschreibung |
   |---|---|
   | Durchschnittliche Tage, um Chancen zu schließen | Durchschnittliche Anzahl der Tage, um eine Gelegenheit zu schließen |
   | Durchschnittliche Tage, um Chancen zu schließen (verloren) | Durchschnittliche Anzahl der Tage bis zu einer verlorenen Gelegenheit |
   | Durchschnittliche Tage, um Chancen zu schließen (Won) | Durchschnittliche Anzahl von Tagen bis zu einer gewesenen Gelegenheit |
   | Anzahl aller Möglichkeiten | Gesamtzahl aller Möglichkeiten |
   | Anzahl der Möglichkeiten (geschlossen) | Gesamtzahl der geschlossenen (erlittenen oder verlorenen) Gelegenheiten |
   | Anzahl der Möglichkeiten (Verloren) | Gesamtzahl der verlorenen Gelegenheiten |
   | Anzahl der Möglichkeiten (Öffnungen) | Gesamtzahl der noch offenen Möglichkeiten |
   | Anzahl der Möglichkeiten (in Mio.) | Gesamtzahl der gewinnten Gelegenheiten |
   | Opportunity-Betrag | Gesamtbetrag der Opportunität. Wenn mehr als ein Lead mit einer Chance verknüpft ist, basiert der Zuordnungsbetrag auf dem Lead-Wert. |
   | Opportunity Amount (Lost) | Gesamtbetrag für verlorene Gelegenheiten. Wenn mehr als ein Lead mit einer Chance verknüpft ist, basiert der Zuordnungsbetrag auf dem Lead-Wert. |
   | Opportunity Amount (Open) | Gesamtbetrag der offenen Möglichkeiten. Wenn mehr als ein Lead mit einer Chance verknüpft ist, basiert der Zuordnungsbetrag auf dem Lead-Wert. |
   | Opportunity Amount (Won) | Gesamtsumme für die eigenen Gelegenheiten. Wenn mehr als ein Lead mit einer Chance verknüpft ist, basiert der Zuordnungsbetrag auf dem Lead-Wert. |

>[!MORELIKETHIS]
>
>* [Erstellen eines Berichts zum Umsatz-Explorer](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
>* [Hinzufügen von Feldern zu einem Umsatz-Explorer-Bericht](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/adding-fields-to-a-revenue-explorer-report.md)
>* [Abonnieren eines Berichts über den Umsatz-Explorer](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/subscribe-to-a-revenue-explorer-report.md)
