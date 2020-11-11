---
title: erwartet-Verhalten
description: Erwartetes Verhalten
translation-type: tm+mt
source-git-commit: 642fd57105afff1031f18883c5809206f136b7c6
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

* PA ist sowohl im Marketo Sky als auch im Marketo Classic-Erlebnis verfügbar. Die Verfügbarkeit spezifischer Funktionen ist wie folgt:
   * Prognostizierende Filter - [!DNL Sky/Classic]
   * Voraussichtliche Registrierungen - [!DNL Sky/Classic]
   * Prognosen zur Wahrscheinlichkeit auf Interessentenebene - [!DNL Sky/Classic]
   * Ziele und Verfolgung - [!DNL Sky] nur
   * Einblicke und Empfehlungen - [!DNL Sky] nur
* [Die anfängliche Aktivierung](/help/sky/getting-started-with-predictive-audiences.md) dauert **24-48 Stunden**, bis alle Prozesse abgeschlossen sind, nachdem PA aktiviert wurde. Sie sehen alle Funktionen für Predictive Audiencen und Predictive Filters auf der Benutzeroberfläche, aber es kann bis zu 24 Stunden dauern, bis diese Funktionen funktionieren.
* **Prognosen werden nur für neue Kampagnen generiert, die nach Aktivierung der Funktion erstellt werden.**

## Für prädiktive Filter gibt es einige zusätzliche Aspekte:

* Filter mit Registrierungs- und Teilnehmerwahrscheinlichkeit können nur mit Ereignis- oder Webinar-Programmen verwendet werden. Lookalike- und Unsubscribe-Filter können in E-Mail-, Ereignis- und Webinar-Programmen verwendet werden.
* Sie können prädiktive Filter auf eine intelligente Kampagne anwenden, selbst wenn das übergeordnete Programm erstellt wurde, bevor die Filter für die Vorhersage aktiviert wurden.
* Predictive Filter sind nicht für Auslöser-Kampagnen verfügbar.
* Um eine intelligente Kampagne auszuführen, müssen die Filter mit hoher Wahrscheinlichkeit zusammen mit anderen regulären Filtern verwendet werden.
* Die Funktion Gespeicherte Regeln steht nicht zur Verwendung in Kampagnen zur Verfügung, die prädiktive Filter enthalten.
* Sie können **bis zu 5** prädiktive Filter in einer intelligenten Liste verwenden.
* Predictive Filter können **maximal 1 Million qualifizierte Interessenten** verarbeiten.
* Sie können **bis zu 50 aktive Programm** mit prädiktiven Filtern haben. Ein aktives Programm ist jedes Programm, das vorhersagende Filter verwendet und mindestens einmal geplant wurde.

## Wann sind keine projizierten Registrierungen verfügbar?

In den folgenden Anwendungsfällen sind keine projizierten Registrierungen verfügbar:

* wenn das Programm vor dem Hinzufügen von Prognosen-Audiencen erstellt wurde
* wenn Programm-Status nicht den Systemstatus zugeordnet sind
* wenn keine Mitglieder im Programm vorhanden sind
* wenn in den letzten 6 Monaten keine ähnlichen Programm aufgetreten sind, die den erforderlichen Kriterien entsprechen
