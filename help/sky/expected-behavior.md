---
title: erwartet-Verhalten
description: Erwartetes Verhalten
exl-id: 8f6d12e4-851c-43d8-a5cf-053887517aaa
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Erwartetes Verhalten

<br> 

In diesem Artikel finden Sie Informationen zum erwarteten Verhalten in Verbindung mit Prädiktiven Audiencen (PA).

## Aspekte zu Daten und Datenschutz

* Die gesamte erforderliche Datenverarbeitung für die AI/ML-Modelle findet in Nordamerika statt.
* AI/ML-Modelle verwenden keine spezifischen Interessenteninformationen wie Vor- oder Nachnamen, Geschlecht, E-Mails, Kontaktnummern usw. Modelle verwenden nur allgemeine Attribute, die von firmografischen und Aktivitäten-Protokollen abgeleitet sind.

## Bei Predictive-Audiencen ist folgendes Verhalten zu erwarten:

* PA ist sowohl im Marketo Sky- als auch im Marketo Classic-Erlebnis verfügbar. Die Verfügbarkeit spezifischer Funktionen ist wie folgt:
   * Prognostische Filter - [!DNL Sky/Classic]
   * Projizierte Registrierungen - [!DNL Sky/Classic]
   * Prognosen zur Wahrscheinlichkeit auf Interessentenebene - [!DNL Sky/Classic]
   * Ziele und Verfolgung - nur [!DNL Sky]
   * Einblicke und Empfehlungen - nur [!DNL Sky]
* [Die anfängliche ](/help/sky/getting-started-with-predictive-audiences.md) Aktivierung dauert **24-48** Stunden, bis alle Prozesse abgeschlossen sind, nachdem PA aktiviert wurde. Sie sehen alle Funktionen für Predictive Audiencen und Predictive Filters auf der Benutzeroberfläche, aber es kann bis zu 24 Stunden dauern, bis diese Funktionen funktionieren.
* **Prognosen werden nur für neue Kampagnen generiert, die nach Aktivierung der Funktion erstellt werden.**

## Für prädiktive Filter gibt es einige zusätzliche Aspekte:

* Filter mit Registrierungs- und Teilnehmerwahrscheinlichkeit können nur mit Ereignis- oder Webinar-Programmen verwendet werden. Lookalike- und Unsubscribe-Filter können in E-Mail-, Ereignis- und Webinar-Programmen verwendet werden.
* Sie können prädiktive Filter auf eine intelligente Kampagne anwenden, selbst wenn das übergeordnete Programm erstellt wurde, bevor die Filter für die Vorhersage aktiviert wurden.
* Predictive Filter sind nicht für Trigger-Kampagnen verfügbar.
* Um eine intelligente Kampagne auszuführen, müssen die Filter mit hoher Wahrscheinlichkeit zusammen mit anderen regulären Filtern verwendet werden.
* Die Funktion Gespeicherte Regeln steht nicht zur Verwendung in Kampagnen zur Verfügung, die prädiktive Filter enthalten.
* Sie können in einer intelligenten Liste **bis zu 5** Vorhersagekräftige Filter verwenden.
* Predictive Filter können maximal 1 Million qualifizierte Interessenten verarbeiten.****
* Sie können bis zu 50 aktive Programm **mit prädiktiven Filtern haben.** Ein aktives Programm ist jedes Programm, das vorhersagende Filter verwendet und mindestens einmal geplant wurde.

## Wann sind keine projizierten Registrierungen verfügbar?

In den folgenden Anwendungsfällen sind keine projizierten Registrierungen verfügbar:

* wenn das Programm vor dem Hinzufügen von Prognosen-Audiencen erstellt wurde
* wenn Programm-Status nicht den Systemstatus zugeordnet sind
* wenn keine Mitglieder im Programm vorhanden sind
* wenn in den letzten 6 Monaten keine ähnlichen Programm aufgetreten sind, die den erforderlichen Kriterien entsprechen
