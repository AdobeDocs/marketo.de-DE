---
unique-page-id: 12983291
description: Verstehen der Zeitzone der Empfänger - Marketo-Dokumente - Produktdokumentation
title: Die Zeitzone der Empfänger
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Die Zeitzone der Empfänger {#understanding-recipient-time-zone}

E-Mail- und Interaktionsprogramme können so konfiguriert werden, dass sie entsprechend der Zeitzone der Empfänger gesendet werden. So müssen nicht mehrere Programme erstellt werden - einmal senden und Marketo speichert die E-Mail automatisch bis zur korrekten Ortszeit.

>[!NOTE]
>
>Die Zeitzone der Empfänger funktioniert derzeit **nur** mit E-Mail-Inhalten. Sie funktioniert nicht für standardmäßige Interaktionsprogramme.

## E-Mail-Programme {#email-programs}

Es gibt zwei primäre Szenarien, in denen [ein E-Mail-Programm planen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md):

1. Planung der Programmausführung in den nächsten 25 Stunden.
1. Planung des Programms, das in Zukunft mehr als 25 Stunden laufen soll (d. h. nächste Woche).

Um jede Zeitzone zu berücksichtigen, starten E-Mail-Programme, die mit der Zeitzone des Empfängers geplant sind, um Mitternacht in der Zeitzone **first/frühestens** der Welt laufen (UTC +14:00).

## Engagementprogramme {#engagement-programs}

Wenn Sie [ einen Interaktionsprogramm-Stream ](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) planen und die Zeitzone des Empfängers aktiv ist, beginnt der Programmcast um Mitternacht in UTC +14:00. Wir fordern Sie auf, den ersten Abruf in Zukunft mindestens 25 Stunden (24 Stunden + etwas Zeit, um die Kampagne zu starten) zu planen, da sich Personen in jeder Zeitzone der Welt für die Absendung qualifizieren können. Der Beginn der Verarbeitung zu diesem Zeitpunkt in UTC +14:00 garantiert, dass wir die E-Mail zum geplanten Datum und zur geplanten Uhrzeit für jede Person senden, die sich für diese Wiedergabe qualifiziert.

## Berechnung der Zeitzone {#calculating-time-zone}

Marketo berechnet die Zeitzone anhand der Stadt, des Bundesstaates, des Landes oder der Postleitzahl einer Person. Wenn wir die Zeitzone eines Benutzers nicht aus diesen Werten berechnen können, kehren wir zu den Feldern &quot;Inferred City&quot;, &quot;Inferred State&quot;, &quot;Inferred Country&quot;und &quot;Inferred Postleitzahl&quot;zurück.

In den Fällen, in denen **nur** Land oder **nur** Status verfügbar ist:

* Für Länder mit drei oder weniger Zeitzonen wählen wir die mittlere Zeitzone aus.
* Für Staaten mit zwei Zeitzonen wählen wir die frühere von beiden aus.

Wenn wir die Zeitzone einer beliebigen Kombination dieser Felder immer noch nicht ermitteln können, weisen wir **nicht** eine Zeitzone zu und die E-Mail wird basierend auf Ihrer Marketo-Abonnementzeitzone gesendet. Wenn Ihr Programm also für 9:00 Uhr PDT geplant ist, erhalten Personen ohne zugewiesene Zeitzone die E-Mail um 9:00 Uhr PDT.

>[!NOTE]
>
>Marketo berechnet die Zeitzone einer Person automatisch neu, wenn sich eines der oben genannten Eingabefelder ändert.

>[!MORELIKETHIS]
>
>* [E-Mail-Programme mit der Zeitzone des Empfängers planen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Head Start für E-Mail-Programme](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [Planen von Interaktionsprogrammen mit der Zeitzone der Empfänger](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)
