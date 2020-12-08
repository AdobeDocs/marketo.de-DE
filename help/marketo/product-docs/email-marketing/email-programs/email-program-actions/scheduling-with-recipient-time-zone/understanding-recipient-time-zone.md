---
unique-page-id: 12983291
description: Die Zeitzone des Empfängers - Marketing Docs - Produktdokumentation
title: Die Zeitzone des Empfängers
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---


# Die Zeitzone des Empfängers {#understanding-recipient-time-zone}

E-Mail- und Interaktions-Programm können entsprechend den Zeitzonen der Empfänger konfiguriert werden, sodass nicht mehr mehrere Programm erstellt werden müssen. Senden Sie einmal und Marketing hält die E-Mail automatisch bis zur richtigen Ortszeit.

>[!NOTE]
>
>Die Zeitzone des Empfängers funktioniert derzeit **nur** mit E-Mail-Inhalten. Es funktioniert nicht für standardmäßige Interaktionsmodule.

## E-Mail-Programme {#email-programs}

Beim [Planen eines E-Mail-Programms](schedule-email-programs-with-recipient-time-zone.md)gibt es zwei primäre Szenarien:

1. Planen der Ausführung des Programms innerhalb der nächsten 25 Stunden.
1. Planen der zukünftigen Ausführung des Programms um mehr als 25 Stunden (d.h. nächste Woche).

Um jede Zeitzone aufzunehmen, senden Sie E-Mail-Programms, die mit dem Empfänger Time Zone Beginn geplant sind, der um Mitternacht in der **ersten/frühesten** Zeitzone der Welt läuft (UTC +14:00).

## Interaktions-Programme {#engagement-programs}

Wenn Sie einen Interaktions-Programm-Stream [](../../../../../product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) planen und die Zeitzone des Empfängers aktiv ist, wird der Programm-Guss um Mitternacht in UTC +14:00 ausgeführt. Wir verlangen, dass Sie den ersten Guss mindestens 25 Stunden in der Zukunft planen (24 Stunden + etwas Zeit, um die Kampagne zu starten), weil Menschen sich für die Besetzung in jeder Zeitzone der Welt qualifizieren können. Die Verarbeitung in UTC +14:00 beginnt zu diesem Zeitpunkt und garantiert, dass wir die E-Mail zum vorgesehenen Zeitpunkt für jede Person, die sich für diese Besetzung qualifiziert, senden.

## Berechnung der Zeitzone {#calculating-time-zone}

Marketo berechnet die Zeitzone anhand des Codes für Stadt, Staat, Land oder Postleitzahl einer Person. Wenn wir die Zeitzone eines Benutzers nicht aus diesen Werten berechnen können, kehren wir zu unseren Feldern &quot;Inferred City&quot;, &quot;Inferred State&quot;, &quot;Inferred Country&quot;und &quot;Inferred Zip Code&quot;zurück.

In den Fällen, in denen **nur **Land oder **nur** Staat verfügbar ist:

* Für Länder mit drei oder weniger Zeitzonen wählen wir die mittlere Zeitzone aus.
* Bei Staaten mit zwei Zeitzonen wählen wir die frühere Version aus.

Wenn wir die Zeitzone eines Benutzers noch immer nicht aus einer Kombination dieser Felder ermitteln können, weisen wir **keine** Zeitzone zu und die E-Mail wird basierend auf Ihrer MarketingTo-Abonnement-Zeitzone gesendet. Wenn Ihr Programm also für 9:00 Uhr PDT geplant ist, erhalten Personen ohne zugewiesene Zeitzone die E-Mail um 9:00 Uhr PDT.

>[!NOTE]
>
>Marketo berechnet die Zeitzone einer Person automatisch, wenn sich eines der oben genannten Eingabefelder ändert.

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [E-Mail-Programm mit Zeitzone des Empfängers planen](schedule-email-programs-with-recipient-time-zone.md)
>* [Beginn für E-Mail-Programme](../../../../../product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)

   >
   >
* [Planen von Programmen mit Interaktion mit der Zeitzone des Empfängers](../../../../../product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

>



