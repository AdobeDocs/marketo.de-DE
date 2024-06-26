---
description: Erwartetes Verhalten - Marketo-Dokumente - Produktdokumentation
title: Erwartetes Verhalten
hide: true
hidefromtoc: true
exl-id: d19130cf-186e-4aad-be32-6aad18c9d08b
source-git-commit: fb77478cdcd2b455e9f2359e16aca50143ce492c
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Erwartetes Verhalten {#expected-behavior}

In diesem Artikel finden Sie Informationen zum erwarteten Verhalten im Zusammenhang mit Predictive Audiences (PA).

## Aspekte zu Daten und Datenschutz

* Die gesamte für die KI/ML-Modelle erforderliche Datenverarbeitung findet in Nordamerika statt.
* KI-/ML-Modelle verwenden keine bestimmten Lead-Informationen wie Vor- oder Nachnamen, Geschlecht, E-Mails, Kontaktnummern usw. Modelle verwenden nur allgemeine Attribute, die aus firmographischen Daten und Aktivitätsprotokollen abgeleitet werden.

**Für Predictive Audiences ist folgendes Verhalten zu erwarten**

* Der Zugriff auf PA erfolgt sowohl über Marketo Sky als auch über das Marketo Classic-Erlebnis. Spezifische Funktionen sind wie folgt verfügbar:
   * Prädiktive Filter - [!DNL Sky/Classic]
   * Vorgeschlagene Registrierungen - [!DNL Sky/Classic]
   * Wahrscheinlichkeitsprognosen auf Lead-Ebene - [!DNL Sky/Classic]
   * Ziele und Tracking - [!DNL Sky] only
   * Einblicke und Empfehlungen - [!DNL Sky] only
* Die Erstaktivierung erfolgt **24-48 Stunden** für alle Prozesse abgeschlossen werden, nachdem PA aktiviert wurde. Auf der Benutzeroberfläche werden alle Funktionen für Predictive Audiences und Predictive Filters angezeigt. Es kann jedoch bis zu 24 Stunden dauern, bis diese Funktionen funktionieren.
* **Prognosen werden nur für neue Kampagnen generiert, die nach der Aktivierung der Funktion erstellt werden.**

**Für vorhersagekräftige Filter gibt es einige zusätzliche Aspekte**:

* Registrierungs- und Besuchswahrscheinlichkeitsfilter können nur mit Ereignis- oder Webinarprogrammen verwendet werden. Lookalike- und Unsubscribe-Filter können in E-Mail-, Ereignis- und Webinarprogrammen verwendet werden.
* Sie können auf eine Smart-Kampagne Predictive Filter anwenden, selbst wenn das übergeordnete Programm erstellt wurde, bevor Prädiktive Filter aktiviert wurden.
* Für Trigger-Kampagnen stehen keine Predictive Filter zur Verfügung.
* Um eine intelligente Kampagne durchzuführen, müssen Wahrscheinlichkeitsfilter zusammen mit anderen regulären Filtern verwendet werden.
* Die Funktion &quot;Gespeicherte Regeln&quot;ist nicht zur Verwendung in Kampagnen verfügbar, die Vorhersagefilter enthalten.
* Sie können **bis 5** Predictive Filter in einer Smart-Liste.
* Predictive Filter können eine **maximal 1 Million qualifizierte Leads**.
* Sie können **bis zu 50 aktive Programme** mit Prognosefiltern. Ein aktives Programm ist ein Programm, das prädiktive Filter verwendet und mindestens einmal geplant wurde.

## Wann sind die geplanten Registrierungen nicht verfügbar?

In den folgenden Anwendungsfällen sind keine geplanten Registrierungen verfügbar:

* wenn das Programm vor dem Hinzufügen von Predictive Audiences erstellt wurde
* wenn der Programmstatus nicht den Systemstatus zugeordnet ist
* wenn keine Mitglieder im Programm enthalten sind
* wenn es in den letzten 6 Monaten keine ähnlichen Programme gibt, die den erforderlichen Kriterien entsprechen
