---
description: Erfahren Sie, wie sich die Richtlinien zur Datenaufbewahrung von 25 Monaten und 90 Tagen von Marketo auf Analytics-Berichte auswirken, mit einer Aufschlüsselung pro Bericht und Tipps zur längeren Aufbewahrung von Daten.
title: Datenaufbewahrung
feature: Reporting
source-git-commit: 0828b4cb43dd18d02b80083ea5128e2f0e5e40d6
workflow-type: tm+mt
source-wordcount: '1084'
ht-degree: 5%

---

# Richtlinie zur Datenaufbewahrung in Marketo-Aktivitäten - Auswirkungen auf das Reporting

Marketo speichert Marketing-Aktivitätsdaten fortlaufend. Aktivitäts- und Kampagnenmitgliedschaftsdaten werden für rollierende 25 Monate nach dem Aktivitätsdatum gespeichert, und Aktivitätsdaten mit hohem Volumen werden standardmäßig für einen rollierenden Zeitraum von 90 Tagen nach dem Aktivitätsdatum gespeichert, der pro Benutzer angepasst werden kann. Nach Ablauf dieser Aufbewahrungsfristen sind die Daten nicht mehr über die Marketo-Benutzeroberfläche verfügbar.

## Marketo Analytics-Berichte

Da Aktivitätsdaten bis zu 25 Monate lang aufbewahrt werden, sind einige Marketo Analytics-Berichte von dieser Richtlinie betroffen, andere nicht. Berichte, die Daten aus Personenaktivitätsprotokollen verwenden, zeigen nur Daten für bis zu 25 Monate an. Berichte, die sich überhaupt nicht auf die Aktivität einer Person beziehen, sind davon nicht betroffen.

Allerdings können auch Berichte, die standardmäßig nicht auf die Personenaktivität verweisen, betroffen sein, wenn Filter zur Smart-Liste des Berichts hinzugefügt werden. Filter, die auf Personenattribute verweisen (Informationen in Feldern im Personendatensatz), bewirken keine Änderung am Bericht. Filter, die nach Aktivitäten suchen, die die Person durchgeführt hat, können nur auf Aktivitäten innerhalb des Aufbewahrungsfensters zugreifen. Wenn die Aktivität also länger zurückliegt, werden die Ergebnisse des Berichts geändert.

In der folgenden Tabelle ist zusammengefasst, wie sich jeder Bericht verhält, einschließlich gängiger Filterszenarien.

## Berichtreferenz

| Berichtstyp | Szenario filtern | Beeinflusst durch die Aufbewahrungsrichtlinie? |
|---|---|---|
| **Revenue Cycle Explorer-Berichte** | Keine Filter verfügbar | Nein - Benutzende von Revenue Cycle Explorer und Advanced Analytics sind vollständig von diesen Aufbewahrungsbeschränkungen befreit. RCE-Daten werden über Nacht an einen separaten Datenbank-Server gesendet, der RCE-Berichte verwaltet. Da die Berichte separat und nicht in persönlichen Aktivitätsprotokollen gespeichert werden, sind diese Berichte von dieser Richtlinie nicht betroffen. Der Umsatzzyklus-Explorer ruft Daten nicht direkt aus der Personendatenbank ab, sodass keine Filter verfügbar sind. |
| **Leistungsbericht für Personen** | Keine Filter für Smart-Listen | Nein |
| | Filter für Personenattribute (z. B.: Vorname) | Nein |
| | Filter der Aktivitäten von Personen in den letzten 25 Monaten | Nein |
| | Filter für Personenaktivitäten ohne Datumsbeschränkung | Ja |
| **Personen nach Status** | Keine Filter für Smart-Listen | Nein |
| | Filter für Personenattribute (z. B.: Vorname) | Nein |
| | Filter der Aktivitäten von Personen in den letzten 25 Monaten | Nein |
| | Filter für Personenaktivitäten ohne Datumsbeschränkung | Ja |
| **Personen nach Umsatzstufe** | Keine Filter für Smart-Listen | Nein |
| | Filter für Personenattribute (z. B.: Vorname) | Nein |
| | Filter der Aktivitäten von Personen in den letzten 25 Monaten | Nein |
| | Filter für Personenaktivitäten ohne Datumsbeschränkung | Ja |
| **Success Path Analyzer** | Enthält keine Smart-Listen | n.z |
| **Bericht zum sozialen Einfluss** | Keine Filter für Smart-Listen | Ja |
| | Filter für Personenattribute (z. B.: Vorname) | Ja |
| | Filter der Aktivitäten von Personen in den letzten 25 Monaten | Ja |
| | Filter für Personenaktivitäten ohne Datumsbeschränkung | Ja |
| **Opportunity Influence Analyzer** | Enthält keine Smart-Listen | Nein |
| **E-Mail-Leistung** | Keine Filter für Smart-Listen | Nein |
| | Filter für Personenattribute (z. B.: Vorname) | Nein |
| | Filter der Aktivitäten von Personen in den letzten 25 Monaten | Nein |
| | Filter für Personenaktivitäten ohne Datumsbeschränkung | Ja |
| **E-Mail-Link-Leistung** | Keine Filter für Smart-Listen | Nein |
| | Filter für Personenattribute (z. B.: Vorname) | Nein |
| | Filter der Aktivitäten von Personen in den letzten 25 Monaten | Nein |
| | Filter für Personenaktivitäten ohne Datumsbeschränkung | Ja |
| **E-Mail-Insights** | Keine Smart-Listen verwenden | Nein |
| **Sales Insight E-Mail-Performance** | Keine Filter für Smart-Listen | Nein |
| | Filter für Personenattribute (z. B.: Vorname) | Nein |
| | Filter der Aktivitäten von Personen in den letzten 25 Monaten | Nein |
| | Filter für Personenaktivitäten ohne Datumsbeschränkung | Ja |
| **Leistung der Landingpage** | Keine Filter für Smart-Listen | Nein - Landingpage-Leistungsdaten werden auf unbestimmte Zeit aufbewahrt und unterliegen nicht der Aufbewahrungsrichtlinie. |
| | Filter für Personenattribute (z. B.: Vorname) | Nein |
| | Filter der Aktivitäten von Personen in den letzten 25 Monaten | Nein |
| | Filter für Personenaktivitäten ohne Datumsbeschränkung | Nein |
| **Web-Seitenaktivität** | Keine Filter für Smart-Listen | Ja — vorbehaltlich der standardmäßigen Aufbewahrungsfrist von 90 Tagen (je Benutzer anpassbar) |
| | Filter für Personenattribute (z. B.: Vorname) | Ja |
| | Filter der Aktivitäten von Personen in den letzten 25 Monaten | Ja |
| | Filter für Personenaktivitäten ohne Datumsbeschränkung | Ja |
| **Unternehmens-Web-Aktivität** | Keine Filter für Smart-Listen | Ja |
| | Filter für Personenattribute (z. B.: Vorname) | Ja |
| | Filter der Aktivitäten von Personen in den letzten 25 Monaten | Ja |
| | Filter für Personenaktivitäten ohne Datumsbeschränkung | Ja |
| **Programm-Performance** | Keine Filter für Smart-Listen | Nein |
| | Filter für Personenattribute (z. B.: Vorname) | Nein |
| | Filter der Aktivitäten von Personen in den letzten 25 Monaten | Nein |
| | Filter für Personenaktivitäten ohne Datumsbeschränkung | Ja |
| **Engagement Stream-Leistung** | Keine Filter für Smart-Listen | Nein |
| | Filter für Personenattribute (z. B.: Vorname) | Nein |
| | Filter der Aktivitäten von Personen in den letzten 25 Monaten | Nein |
| | Filter für Personenaktivitäten ohne Datumsbeschränkung | Ja |
| **Programm-Analysator** | Keine Smart-Listen verwenden | Nein |
| **Kampagnenaktivität** | Keine Filter für Smart-Listen | Nein |
| | Filter für Personenattribute (z. B.: Vorname) | Nein |
| | Filter der Aktivitäten von Personen in den letzten 25 Monaten | Nein |
| | Filter für Personenaktivitäten ohne Datumsbeschränkung | Ja |
| **Kampagnen-E-Mail-Leistung** | Keine Filter für Smart-Listen | Ja |
| | Filter für Personenattribute (z. B.: Vorname) | Ja |
| | Filter der Aktivitäten von Personen in den letzten 25 Monaten | Ja |
| | Filter für Personenaktivitäten ohne Datumsbeschränkung | Ja |

## Problemumgehungen bei Berichten

Aktivitätsdaten, die älter als das Aufbewahrungsfenster sind, können von vielen Benutzern als veraltet angesehen werden. Es kann jedoch sein, dass diese Informationen in einem Anwendungsfall benötigt werden. Im Folgenden finden Sie Möglichkeiten, diese Daten über die standardmäßige Aufbewahrungsfrist hinaus aufzubewahren.

## Exportieren der Daten

Marketo bietet die [Bulk Extract REST-API](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/bulk-extract/bulk-extract), mit der Sie Personenaktivitäten exportieren und lokal speichern können. Sobald die Daten über die API extrahiert wurden, können Sie sie speichern und sortieren, wie Sie dies für Ihren Anwendungsfall benötigen.

>[!TIP]
>
>Exportieren Sie Ihre Personendaten nach einem regulären Zeitplan, nicht nur einmal. Die Personenaktivitäten werden in einem rollierenden 25-monatigen Zyklus beibehalten. Legen Sie eine Erinnerung fest _die Sie_ Ende dieses 25-monatigen Zeitraums erneut exportieren möchten.

## Benutzerdefinierte Felder verwenden

Die Werte der Personenfelder sind von der Richtlinie zur Datenaufbewahrung nicht betroffen. Sie können intelligente Kampagnen verwenden, um benutzerdefinierte Felder basierend auf den Aktivitäten Ihrer Mitarbeiter mit Werten zu füllen. Auf diese Weise können Sie Personen nach diesen Personenattributen (die nicht der Aufbewahrungsrichtlinie unterliegen) und nicht nach den Aktivitäten selbst (die der Aufbewahrungsrichtlinie unterliegen) filtern.

Ein weiterer Vorteil dieses Ansatzes besteht darin, dass die Suche nach Personenattributen schneller ist als die Suche in Personenaktivitätsprotokollen.
