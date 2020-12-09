---
unique-page-id: 12982903
description: Planen von E-Mail-Programmen mit Empfänger-Zeitzone - Marketing-Dokumente - Produktdokumentation
title: E-Mail-Programm mit Zeitzone des Empfängers planen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---


# E-Mail-Programm mit Zeitzone des Empfängers planen {#schedule-email-programs-with-recipient-time-zone}

Beim Planen eines E-Mail-Programms während der Aktivierung der Zeitzone des Empfängers gibt es zwei potenzielle Szenarien:

1. Planen der Ausführung des Programms **innerhalb** der nächsten 25 Stunden
1. Planen der zukünftigen Ausführung des Programms **über** 25 Stunden (d.h. nächste Woche)

## Szenario 1: Innerhalb von 25 Stunden {#scenario-within-hours}

Angenommen, Sie genehmigen ein E-Mail-Programm mit aktivierter Zeitzone des Empfängers und einer geplanten Auslieferungszeit innerhalb der nächsten 25 Stunden. Möglicherweise befinden sich Personen in Ihrer intelligenten Liste in Zeitzonen, in denen die geplante Zeit bereits abgelaufen ist.

In diesem Szenario können Sie entscheiden, was mit dieser Untergruppe qualifizierter Personen zu tun ist. Klicken Sie auf das Zahnradsymbol neben der Zeitzone **des** Empfängers in der Kachel **Plan** des E-Mail-Programms.

![](assets/image2017-12-5-10-3a46-3a42.png)

Dies bietet zwei Optionen:

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Definition**
>
>* **Stellen Sie den folgenden Tag in der Zeitzone** des Empfängers bereit: Wenn die E-Mail am Dienstag um 9:00 Uhr ausgehen soll, erhalten qualifizierte Personen, die in Zeitzonen leben, in denen die geplante Zeit bereits abgelaufen ist, die E-Mail am *Mittwoch* um 9:00 Uhr.
   >
   >
* **Bereitstellung unter Verwendung der Standardeinstellung** des Programms: Wenn die E-Mail am Dienstag um 9:00 Uhr ausgehen soll, erhalten qualifizierte Personen, die in Zeitzonen leben, in denen die geplante Zeit bereits abgelaufen ist, die E-Mail *entsprechend Ihren Zeitzoneneinstellungen* des Abonnements. Wenn Sie also [die Zeitzoneneinstellungen](../../../../../product-docs/administration/settings/select-your-language-locale-and-time-zone.md) für die [Abonnementzeit](../../../../../product-docs/administration/settings/set-default-location-settings-for-a-subscription.md) auf PDT America/Los Angeles einstellen, erhalten diese Empfänger am Dienstag um 9:00 Uhr PDT die E-Mail (unabhängig davon, zu welchem Zeitpunkt sie sich in ihren eigenen Zeitzonen befinden).

>



>[!NOTE]
>
>[Erfahren Sie mehr](https://docs.marketo.com/display/DOCS/Understanding+Recipient+Time+Zone#UnderstandingRecipientTimeZone-CalculatingTimeZone) darüber, wie Marketo Zeitzonen für Empfänger berechnet.

Betrachten wir dieses Szenario genauer. Angenommen, Sie sind in San Francisco und planen eine E-Mail um 7:00 Uhr für einen **9:00 Uhr** -Versand. In Ihrer intelligenten Liste gibt es Menschen aus den folgenden Regionen:

* San Francisco
* Texas
* New York
* Italien

![](assets/image2017-12-6-10-3a52-3a41.png)

9:00 Uhr morgens ist bereits in New York und Italien vergangen, sodass qualifizierte Personen in diesen beiden Zeitzonen die E-Mail erhalten, basierend auf den **Zeitzoneneinstellungen**:

* **Stellen Sie den folgenden Tag in der Zeitzone des Empfängers bereit:** Mittwoch um 9:00 Uhr in den jeweiligen Zeitzonen, **ODER**

* **Bereitstellung unter Verwendung der Standardeinstellung** des Programms: Dienstag um 9:00 Uhr PDT (New York - 22:00 Uhr EDT und Italien - 18:00 Uhr MEZ).

Nachdem Sie Ihr Programm genehmigt haben, wird es innerhalb von 15 Minuten ausgeführt.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Obwohl das Programm den *Versand* von E-Mails in 15 Minuten Beginn, werden E-Mails zu diesem Zeitpunkt nicht *zugestellt* . Empfänger erhalten weiterhin E-Mails, die auf den von Ihnen gewählten **Zeitzoneneinstellungen** basieren.

## Szenario 2: Mehr als 25 Stunden {#scenario-more-than-hours}

In diesem zweiten Szenario genehmigen Sie ein E-Mail-Programm mit aktivierter **Empfänger-Zeitzone** und einer geplanten Auslieferungszeit von mehr als 25 Stunden. In diesem Fall wird das Programm zur geplanten Zeit in der **frühesten** Zeitzone der Welt ausgeführt (UTC + 14:00). Es kann Leute geben, die sich für Ihre intelligente Liste in jeder Zeitzone auf der ganzen Welt qualifizieren, sodass wir ab der frühesten Zeitzone die E-Mail zum geplanten Datum/zur Uhrzeit an alle Empfänger in ihren jeweiligen Zeitzonen senden können.

Beginn

Sprechen wir nun darüber, wie [Head-Beginn](../../../../../product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) mit **Empfänger-Zeitzone** funktioniert. Für unsere bestehende Kopfzeilenfunktion ist es erforderlich, dass das Programm mindestens 12 Stunden im Voraus geplant wird. Was bedeutet das für die Zeitzone des Empfängers? Denken Sie daran, dass bei aktivierter Zeitzone für Empfänger der Beginn, der das E-Mail-Programm zur geplanten Zeit in der frühesten Zeitzone ausführt (UTC +14:00). Um also **sowohl** Head-Beginn als auch Empfänger-Zeitzone zu aktivieren, müssen E-Mail-Programm in UTC +14:00 **mindestens 12 Stunden vor dem geplanten Zeitpunkt geplant werden.**

Wenn Sie also in Amerika/Los Angeles sind und sowohl Head-Beginn als auch Empfänger-Zeitzone aktivieren möchten, müssen Sie das Programm **34 Stunden** im Voraus planen. Wie sind wir zu dieser Zahl gekommen?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

Kurz gesagt, E-Mail-Programm, die mit der Zeitzone des Empfängers geplant sind, müssen zur planmäßigen Zeit in der frühesten Zeitzone (d. h. dort, wo sie zuerst Mitternacht erreicht werden) ausgeführt werden, um jede Zeitzone unterzubringen. Wenn Sie also ein E-Mail-Programm planen...

* **mit einer Versand-Zeit *innerhalb* von 25 Stunden**, die Programm-Beginn innerhalb von 15 Minuten laufen. Empfänger, die die geplante Zeit bereits überschritten haben, erhalten die E-Mail entsprechend den von Ihnen gewählten Zeitzoneneinstellungen.
* **mit einer Versand-Zeit von *mehr* *als* 25 Stunden in der Zukunft**, die Programm-Beginn, die zur geplanten Zeit in der frühesten Zeitzone laufen (UTC +14:00).
* **mit Head-Beginn** die Programm-Beginn, die 12 Stunden vor der geplanten Uhrzeit in der frühesten Zeitzone (UTC +14:00) verarbeiten.

>[!CAUTION]
>
>Jeder, der sich zwischen dem Beginn des E-Mail-Versands und dem Zeitpunkt der tatsächlichen Auslieferung abmeldet, erhält weiterhin die E-Mail. Es wird empfohlen, die Benachrichtigung zum Abbestellen des Abonnements so anzupassen, dass die Verarbeitung von Abbestellungen 1-2 Werktage dauern kann.

>[!MORELIKETHIS]
>
>* [Die Zeitzone des Empfängers](understanding-recipient-time-zone.md)
>* [Beginn für E-Mail-Programme](../../../../../product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Abbruch des Versands von E-Mail-Programmen, die mit der Zeitzone des Empfängers geplant sind](abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)

>



