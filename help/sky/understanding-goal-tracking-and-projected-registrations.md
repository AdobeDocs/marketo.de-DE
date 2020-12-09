---
title: understand-target-tracking-and-projiziert-registrations
description: Erläuterung der Zielverfolgung und der geplanten Registrierungen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 0%

---


# Erläuterung der Zielverfolgung und der geplanten Registrierungen

<br> 

Nach der [Festlegung von Ereignis-Zielen](/help/sky/setting-event-goals.md)und dem Senden von Einladungen durch eine [intelligente Kampagne](/help/sky/create-a-smart-campaign.md), hier ist, wie Sie Ihren Zielfortschritt verfolgen und Marketos Prognosen verstehen.

>[!NOTE]
>
>Wenn ein Ereignis-Programm im Marketing Classic-Erlebnis erstellt wird, ist das Ereignis-Beginn derzeit standardmäßig auf das Erstellungsdatum des Ereignisses eingestellt. Da bei den projizierten Registrierungen die Zeit vor dem Beginn eines Ereignisses berücksichtigt wird, sind diese Zahlen möglicherweise nicht korrekt, wenn das Beginn- und Erstellungsdatum identisch sind (sofern sie nicht absichtlich festgelegt wurden).

## Zielverfolgung und geplante Registrierungen

1. Details zur Zielverfolgung finden Sie auf der Registerkarte &quot; **[!UICONTROL Berichte]** &quot;Ihres Ereignis-Programms. In diesem speziellen Beispiel gibt es bisher 150 registrierte Mitglieder gegen das Ziel von 200 (75 %).

   ![Bild eins](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-1.png)

Sie sehen auch Ihre **[!UICONTROL geplanten]** Registrierungen. Bewegen Sie den Mauszeiger über das Infosymbol, um eine Aufschlüsselung dieser Zahl nach Segment &quot;Wahrscheinlichkeit&quot;anzuzeigen.

![Bild zwei](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-2.png)

>[!NOTE]
>
>Das Diagramm &quot;Geplant&quot;und &quot;Höhere&quot;bleiben bis zum Ereignis leer.

1. Klicken Sie auf den Diagrammschalter, um nach der Registrierungswahrscheinlichkeit zu einer Aufschlüsselung Ihrer Mitglieder zu wechseln. Sie sehen die aktuellen Registrierungsprozentsätze für jedes Segment im Vergleich zum durchschnittlichen Segmentprozentsatz in den letzten Programmen.

   ![Bild drei](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-3.png)

Alle Mitglieder (registriert und noch nicht registriert) werden nach ihrer Registrierungswahrscheinlichkeit kategorisiert. Bewegen Sie den Mauszeiger über das Infosymbol, um zu sehen, wie diese Kategorien definiert werden.

![Bild vier](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-4.png)

>[!NOTE]
>
>Prognosen werden alle 24 Stunden bis zum Ereignis aktualisiert. Alle Mitglieder, die als _Verarbeitung_ aufgeführt sind, werden in den nächsten Berechnungszyklus einbezogen.

## Ähnliche Programm

Sie können einen Einblick in Ihr aktuelles Ereignis erhalten, indem Sie sich ansehen, wie ähnliche Programm in der Vergangenheit funktioniert haben. Dieser Abschnitt zeigt Ihnen bis zu 5 ähnliche Programm aus den letzten 6 Monaten mit der Anzahl/dem Prozentsatz der _registrierten_ oder höher Mitglieder.

Bei der Berechnung ähnlicher Programm werden unter anderem folgende Faktoren berücksichtigt:

* Programm
* Programm Kanal
* Audience
* Programm-Tags
* Zeitdauer von der Erstellung des Ereignisses bis zum Beginn des Ereignisses
* Dauer des Ereignisses

   ![Bild fünf](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-5.png)

## Recommendations

Oben auf der Seite &quot;Berichte&quot;finden Sie AI/ML-basierte Empfehlungen, die auf Ihrem Fortschritt basieren. Schauen Sie regelmäßig vorbei, um hilfreiche Tipps und Einblicke zu erhalten!

![Bild sechs](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-6.png)

## PERSONALENBERECHTIGUNGEN

Klicken Sie auf die Registerkarte **[!UICONTROL Mitglieder]** , um alle Programm-Mitglieder Ansicht. Bewegen Sie den Mauszeiger über die Leisten **[!UICONTROL Registrierungswahrscheinlichkeit]** oder **[!UICONTROL Anwesenheitswahrscheinlichkeit]** , um genaue Prozentsätze und Kategorien anzuzeigen. Sie können dann Maßnahmen gegen Mitglieder in einer bestimmten Kategorie ergreifen (z.B. für alle in der &quot;Weniger wahrscheinlich&quot;, um Kategorie zu registrieren), und insbesondere Zielgruppe sie, um Ihre Registrierungsnummern potenziell zu erhöhen.

![Bild sieben](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-7.png)

>[!NOTE]
>
>Die individuelle Wahrscheinlichkeit berücksichtigt 40+ Personenfaktoren, einschließlich Profil- und Personenattributen, Aktivität sowie eingeladene/registrierte/besuchte Aktivitäten.

## Häufig gestellte Fragen

**Q: Was ist das Segment?**

A: Die Wahrscheinlichkeit zu registrieren ist ein Wert von 0 bis 100. Jeder, der Mitglied des Ereignis-Programms ist, erhält einen Wahrscheinlichkeitswert zwischen 0 und 100.

Die Werte für die Wahrscheinlichkeit werden in drei Segmente unterteilt:

* Wahrscheinlichkeit der Registrierung > 50% = Hochwahrscheinliches Segment
* Wahrscheinlichkeit der Registrierung > 25% bis &lt;50% = Wahrscheinliches Segment
* Wahrscheinlichkeit der Registrierung &lt; 25 % = Segment mit geringerer Wahrscheinlichkeit

Wenn eine Person die Wahrscheinlichkeit der Registrierung erhält, fällt die Prognose in eines dieser Segmente (jede Person, die Mitglied eines Programms ist, fällt in eines davon). Wenn beispielsweise ein Ereignis-Programm 1000 Mitglieder hat, die auf den Wahrscheinlichkeitsvorhersagen basieren, würden diese 1000 in _Hochgradig wahrscheinliche_, _wahrscheinliche_ oder _weniger wahrscheinliche_ Segmente verteilt.

Daher haben Personen, die in das Segment &quot;Sehr wahrscheinlich&quot;fallen, eine höhere Chance, sich für das Ereignis zu registrieren.

Konversion in Registrierung = Anzahl der registrierten Personen in Segment geteilt durch Anzahl der Personen, die in das Segment fallen (z. B. - wenn 100 Personen in das Segment mit hoher Wahrscheinlichkeit fallen und 60 von ihnen registriert sind, beträgt der Konversionsrate 60 %).

Die Umrechnung in % zur Registrierung erfolgt nach folgendem Muster: Sehr wahrscheinlich > Wahrscheinlich > Weniger wahrscheinlich.

**Q: Wie verwende ich die Einblicke?**

A: Die bewährte Praxis umfasst Folgendes:

i. Sie erstellen ein Programm und dann verwendet eine Smart-Kampagne vorhersagende Filter mit &quot;größer als X&quot;, was zu einer bestimmten Anzahl von Personen führen würde (z. B. 1000) und Sie führen die Kampagne aus.

ii. Nach 24 Stunden können Sie auf der Registerkarte &quot; [!UICONTROL Berichte] &quot;die projizierten Registrierungen sehen, die auf der Grundlage der Wahrscheinlichkeit berechnet werden, Werte aller Personen zu registrieren, die derzeit eingeladen werden.

iii. Wenn die geplanten Registrierungen unter dem Ziel liegen, müssen Sie mehr Personen einladen. An diesem Punkt können Sie die Einblicke sehen, die Ihnen sagen, was der Schwellenwert war, der in den letzten Programmen funktioniert hat.

![Bild acht](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-8.png)

iv. Sie können eine neue intelligente Kampagne mit diesem Schwellenwert erstellen, um weitere Personen einzuladen.

v. Wenn Sie verstehen möchten, warum eine projizierte Audience angezeigt wird, können Sie jederzeit die Segmentverteilung, ihre Konversionsraten aus der Vergangenheit und ihre Anwendung auf die aktuelle Audience anzeigen (siehe Screenshot unten).

**Q: Was ist das Diagramm Segmente nach Registrierung?**

A: Drei Balken, von denen jeder ein Segment darstellt (Hochwahrscheinlich, Wahrscheinlich, weniger wahrscheinlich).

**Lila gepunktete Linie:** Durchschnittliche Konversationsrate für die Registrierung in diesem Segment, basierend auf früheren ähnlichen Programmen.

**Blaue Leiste:** Registrierungsprozentsatz aller Personen in diesem Segment.

![Bild neun](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-9.png)

Nehmen wir beispielsweise an, 100 Personen haben die Wahrscheinlichkeit, sich über 50 % und 60 der 100 registrierten Personen zu registrieren. Mit hoher Wahrscheinlichkeit werden 60 % konvertiert. So erhalten alle zum Programm hinzugefügten Mitglieder die Wahrscheinlichkeit, Werte zu registrieren, dann werden sie in Segmente eingefügt und je nachdem, wie viele Personen in jedem Segment Konversionsrat registriert sind, wird berechnet.

**Q: Was bedeutet &quot;Registered and Higher&quot;?**

A: Jede Person, die als registriert aufgeführt ist, oder jeder andere Status mit einer gleichen oder einer höheren Stufenzahl.

Sie können neue Statusangaben für ein Ereignis-Programm erstellen, aber wir ordnen diese Status den Standardstatus zu. Betrachten wir einen Fall, in dem eine Person von eingeladen zu erinnert wird, was ein höherer Schritt als die Registrierung ist. Diese Person wird auch als registriert und in der Zielverfolgung angezeigt.

![Bild 1](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-10.png)

**Q: Wie werden die projizierten Registrierungen berechnet?**

A: Siehe unten.

![Bild 1](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-11.png)
