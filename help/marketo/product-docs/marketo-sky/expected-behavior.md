---
description: Erwartetes Verhalten - Marketo-Dokumente - Produktdokumentation
title: Erwartetes Verhalten
hide: true
hidefromtoc: true
exl-id: d19130cf-186e-4aad-be32-6aad18c9d08b
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# Erwartetes Verhalten {#expected-behavior}

In diesem Artikel finden Sie Informationen zum erwarteten Verhalten im Zusammenhang mit [!UICONTROL Predictive Audiences] (PA).

## Überlegungen zu Daten und Datenschutz

* Die gesamte erforderliche Datenverarbeitung für die KI/ML-Modelle findet in Nordamerika statt.
* KI/ML-Modelle verwenden keine spezifischen Lead-Informationen wie Vor- oder Nachnamen, Geschlecht, E-Mails, Kontaktnummern usw. Die Modelle verwenden nur allgemeine Attribute, die aus Firmographie- und Aktivitätsprotokollen abgeleitet wurden.

**Bei [!UICONTROL Predictive Audiences] können Sie das folgende Verhalten erwarten**

* Die SPA ist sowohl in [!DNL Marketo Sky] als auch in der [!DNL Marketo Classic] verfügbar. Spezifische Funktionen sind wie folgt verfügbar:
   * Prädiktive Filter - [!DNL Sky/Classic]
   * Voraussichtliche Registrierungen - [!DNL Sky/Classic]
   * Prognosen der Lead-Ebene - [!DNL Sky/Classic]
   * Ziele und Tracking - nur [!DNL Sky]
   * Einblicke und Empfehlungen - nur [!DNL Sky]
* Die anfängliche Aktivierung dauert **24-48 Stunden** bis alle Prozesse abgeschlossen sind, nachdem PA aktiviert wurde. In der Benutzeroberfläche werden alle Funktionen für prädiktive Zielgruppen und prädiktive Filter angezeigt. Es kann jedoch bis zu 24 Stunden dauern, bis diese Funktionen funktionieren.
* **Prognosen werden nur für neue Kampagnen generiert, die nach Aktivierung der Funktion erstellt werden.**

**Es gibt einige zusätzliche Aspekte, die sich speziell auf prädiktive Filter beziehen**:

* Registrierungs- und Anwesenheitsfilter können nur mit Ereignis- oder Webinar-Programmen verwendet werden. Lookalike- und Abmelde-Filter können in E-Mail-, Ereignis- und Webinar-Programmen verwendet werden.
* Sie können auf eine intelligente Kampagne prädiktive Filter anwenden, selbst wenn das übergeordnete Programm erstellt wird, bevor prädiktive Filter aktiviert werden.
* Prädiktive Filter sind für Trigger-Kampagnen nicht verfügbar.
* Um eine intelligente Kampagne auszuführen, müssen Wahrscheinlichkeitsfilter in Verbindung mit anderen regulären Filtern verwendet werden.
* Die Funktion Gespeicherte Regeln ist nicht für die Verwendung in Kampagnen verfügbar, die prädiktive Filter enthalten.
* Sie können **bis zu 5 %** in einer Smart-Liste verwenden.
* Prädiktive Filter können **(maximal 1 Million qualifizierte Leads** verarbeiten.
* Sie können (**50 aktive Programme)** prädiktive Filter verwenden. Ein aktives Programm ist ein Programm, das prädiktive Filter verwendet und mindestens einmal geplant wurde.

## Wann sind geplante Registrierungen nicht verfügbar?

Voraussichtliche Registrierungen sind in den folgenden Anwendungsfällen nicht verfügbar:

* ob das Programm erstellt wurde, bevor prädiktive Zielgruppen hinzugefügt wurden
* Wenn Programmstatus nicht auf Systemstatus abgebildet werden
* Wenn das Programm keine Mitglieder enthält
* wenn es in den letzten sechs Monaten keine ähnlichen Programme in der Vergangenheit gibt, die den erforderlichen Kriterien entsprechen
