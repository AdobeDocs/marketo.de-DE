---
unique-page-id: 12983291
description: Informationen zur Zeitzone der Empfänger - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zur Zeitzone der Empfängerin bzw. des Empfängers
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 3%

---

# Grundlegendes zur Zeitzone der Empfängerin bzw. des Empfängers {#understanding-recipient-time-zone}

E-Mail- und Interaktionsprogramme können so konfiguriert werden, dass sie entsprechend den Zeitzonen der Empfängerinnen und Empfänger bereitgestellt werden. So entfällt die Notwendigkeit, mehrere Programme zu erstellen - einmal senden und Marketo speichert die E-Mail automatisch bis zur korrekten Ortszeit.

>[!NOTE]
>
>[!UICONTROL Zeitzone des Empfängers] funktioniert derzeit **nur** E-Mail-Inhalt. Bei standardmäßigen Interaktionsprogrammen funktioniert dies nicht.

## E-Mail-Programme {#email-programs}

Beim Planen eines E-Mail[Programms gibt es zwei primäre Szenarien](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md):

1. Planung der Programmausführung innerhalb der nächsten 25 Stunden.
1. Planung der Programmausführung für mehr als 25 Stunden in der Zukunft (d. h. nächste Woche).

Um jede Zeitzone zu berücksichtigen, werden E-Mail-Programme, die mit [!UICONTROL Zeitzone des Empfängers] geplant sind, ab Mitternacht in der **ersten/frühesten** Zeitzone der Welt ausgeführt (UTC +14:00).

## Interaktionsprogramme {#engagement-programs}

Wenn Sie [Interaktionsprogramm-Stream planen](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) und die [!UICONTROL Zeitzone des Empfängers] aktiv ist, beginnt die Programmbesetzung um Mitternacht in UTC +14 :00. Wir verlangen, dass Sie die erste Besetzung mindestens 25 Stunden in der Zukunft (24 Stunden + einige Zeit, um die Kampagne zu starten) planen, da Personen sich für die Besetzung in jeder Zeitzone auf der ganzen Welt qualifizieren können. Der Beginn der Verarbeitung zu diesem Zeitpunkt in UTC +14:00 garantiert, dass die E-Mail zum geplanten Datum und zur geplanten Uhrzeit für jede Person gesendet wird, die sich für diese Besetzung qualifiziert.

## Zeitzone wird berechnet {#calculating-time-zone}

Marketo berechnet die Zeitzone basierend auf der Stadt, dem Bundesland, dem Land oder der Postleitzahl einer Person. Wenn wir die Zeitzone einer Person aus diesen Werten nicht berechnen können, kehren wir zu den Feldern Abgeleitete Stadt, Abgeleiteter Staat, Abgeleitetes Land und Abgeleitete Postleitzahl zurück.

In Fällen, in denen wir **nur** Land oder **nur** verfügbar haben:

* Für Länder mit drei oder weniger Zeitzonen wählen wir die mittlere Zeitzone.
* Für Staaten mit zwei Zeitzonen wählen wir den früheren der beiden Zeitzonen aus.

Wenn wir aus einer Kombination dieser Felder immer noch nicht die Zeitzone einer Person ermitteln können, wird **nicht** eine Zeitzone zugewiesen und die E-Mail wird basierend auf der Zeitzone Ihres Marketo-Abonnements gesendet. Wenn Ihr Programm also für 9.:00am PDT geplant ist, werden Personen ohne zugewiesene Zeitzone die E-Mail um 9.:00am PDT erhalten.

>[!NOTE]
>
>Marketo berechnet die Zeitzone einer Person automatisch neu, wenn sich eines der oben genannten Eingabefelder ändert.

>[!MORELIKETHIS]
>
>* [Planen von E-Mail-Programmen mit [!UICONTROL Zeitzone des Empfängers]](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Head Start für E-Mail-Programme](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [Planen von Interaktionsprogrammen mit [!UICONTROL Zeitzone des Empfängers]](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)
