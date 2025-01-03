---
unique-page-id: 12982903
description: Planen von E-Mail-Programmen mit der Zeitzone des Empfängers - Marketo-Dokumente - Produktdokumentation
title: Planen von E-Mail-Programmen mit Zeitzone des Empfängers
exl-id: d0c3f3c1-9f21-4081-818d-7c5cb1766915
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Planen von E-Mail-Programmen mit Zeitzone des Empfängers {#schedule-email-programs-with-recipient-time-zone}

Wenn die Zeitzone des Empfängers für ein E-Mail-Programm aktiviert ist, gibt es zwei mögliche Szenarien:

1. Planen der Ausführung des Programms **innerhalb** nächsten 25 Stunden
1. Planung der Programmausführung (**25** in der Zukunft (d. h. nächste Woche)

## Szenario 1: Innerhalb von 25 Stunden {#scenario-within-hours}

Angenommen, Sie genehmigen ein E-Mail-Programm mit aktivierter Zeitzone des Empfängers und geplanter Versandzeit innerhalb der nächsten 25 Stunden. In Ihrer Smart-Liste befinden sich möglicherweise Personen, die in Zeitzonen leben, in denen die geplante Zeit bereits vergangen ist.

In diesem Szenario können Sie entscheiden, was mit dieser Untergruppe qualifizierter Personen getan werden soll. Klicken Sie auf das Zahnradsymbol neben **Zeitzone des Empfängers** in der Kachel **Zeitplan** des E-Mail-Programms.

![](assets/image2017-12-5-10-3a46-3a42.png)

Dies bietet Ihnen zwei Optionen:

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Definition**
>
>* **Versand am folgenden Tag in der Zeitzone des Empfängers**: Wenn die E-Mail für Dienstag um 9:00 Uhr geplant ist, erhalten qualifizierte Personen, die in Zeitzonen leben, in denen die geplante Zeit bereits verstrichen ist, die E-Mail am *Mittwoch* um 9:00 Uhr.
>
>* **Versand über die im Programm standardmäßig festgelegte Zeit**: Wenn die E-Mail am Dienstag um 9:00 Uhr veröffentlicht werden soll, erhalten qualifizierte Personen, die in Zeitzonen leben, in denen die geplante Zeit bereits verstrichen ist, die E-Mail _basierend auf Ihren Einstellungen für die Zeitzone Ihres Abonnements_. Wenn Ihre [Zeitzoneneinstellungen des Abonnements](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md) also auf PDT America/Los Angeles eingestellt sind, erhalten diese Empfänger die E-Mail immer noch am Dienstag um 9:00 Uhr PDT (unabhängig von der Zeit, die in ihren eigenen Zeitzonen liegt).

>[!NOTE]
>
>[Weitere Informationen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) wie Marketo die Zeitzonen für Empfänger berechnet.

Betrachten wir dieses Szenario genauer. Angenommen, Sie sind in San Francisco und planen eine E-Mail um 7:00 Uhr für einen **9:00**. In Ihrer Smart-Liste befinden sich Personen aus den folgenden Regionen:

* San Francisco
* Texas
* New York
* Italien

![](assets/image2017-12-6-10-3a52-3a41.png)

9:00 Uhr ist in New York und Italien bereits vergangen, sodass qualifizierte Personen in diesen beiden Zeitzonen die E-Mail auf der Grundlage der **Zeitzoneneinstellungen** erhalten:

* **Versand am folgenden Tag in der Zeitzone des Empfängers:** Mittwoch um 9:00 Uhr in der jeweiligen Zeitzone, **OR**

* **Versand erfolgt über die standardmäßig eingestellte Zeit des Programms**: Dienstag um 9:00 Uhr PDT (New York - 12:00 Uhr EDT und Italien - 18:00 Uhr CET).

Sobald Sie Ihr Programm genehmigt haben, wird es innerhalb von 15 Minuten ausgeführt.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Obwohl das Programm den _Prozess_ des E-Mail-Versands in 15 Minuten startet, werden E-Mails zu _Zeitpunkt_ zugestellt. Die Empfänger erhalten weiterhin E-Mails auf der Grundlage **von Ihnen** Zeitzoneneinstellungen.

## Szenario 2: Mehr als 25 Stunden {#scenario-more-than-hours}

In diesem zweiten Szenario genehmigen Sie ein E-Mail-Programm mit **Zeitzone des Empfängers** und einer geplanten Versandzeit, die mehr als 25 Stunden in der Zukunft liegt. In diesem Fall startet das Programm zur geplanten Zeit in der (**)** Zeitzone der Welt (UTC + 14:00 Uhr). Es kann Personen geben, die sich für Ihre Smart-Liste qualifizieren, und zwar in jeder Zeitzone auf der ganzen Welt. Wenn wir also in der frühesten Zeitzone beginnen, können wir die E-Mail zum geplanten Datum/zur geplanten Uhrzeit an alle Empfänger in ihren jeweiligen Zeitzonen senden.

**Kopfstart**

Sprechen wir nun darüber, wie [Kopfstart](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) mit der **Zeitzone des Empfängers“**. Unsere bestehende Head Start-Funktion erfordert, dass das Programm mindestens 12 Stunden im Voraus geplant wird. Was bedeutet das nun für die Zeitzone des Empfängers? Denken Sie daran, dass wir bei aktivierter Zeitzone des Empfängers das E-Mail-Programm zum geplanten Zeitpunkt in der frühesten Zeitzone ausführen (UTC +14:00). Um also (**)**- und Empfängerzeitzone zu aktivieren, müssen E-Mail-Programme geplant werden **mindestens 12 Stunden vor der geplanten Zeit in UTC +14:00.**

Wenn Sie also in Amerika/Los Angeles sind und sowohl die Zeitzone „Head Start“ als auch die Zeitzone „Empfänger“ aktivieren möchten, müssen Sie das Programm **34 Stunden)**. Wie sind wir zu dieser Nummer gekommen?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

Kurz gesagt: E-Mail-Programme, die mit der Zeitzone des Empfängers geplant sind, müssen zur geplanten Zeit in der frühesten Zeitzone ausgeführt werden (d. h. dort, wo sie zuerst Mitternacht erreichen), um jede Zeitzone aufzunehmen. Wenn Sie also ein E-Mail-Programm planen…

* **Mit einer Lieferzeit _innerhalb_ 25 Stunden** beginnt das Programm innerhalb von 15 Minuten zu laufen. Empfänger, die die geplante Zeit bereits überschritten haben, erhalten die E-Mail entsprechend den von Ihnen gewählten Zeitzoneneinstellungen.
* **mit einer Lieferzeit _mehr als_ 25 Stunden in der Zukunft** beginnt das Programm zur geplanten Zeit in der frühesten Zeitzone (UTC +14:00) zu laufen.
* **Mit Head Start** beginnt das Programm mit der Verarbeitung 12 Stunden vor der geplanten Zeit in der frühesten Zeitzone (UTC +14:00).

>[!CAUTION]
>
>Jeder, der sich zwischen dem Beginn des E-Mail-Versands und dem tatsächlichen Versand abmeldet, erhält weiterhin die E-Mail. Es wird empfohlen, die Abmelde-Benachrichtigung so anzupassen, dass die Bearbeitung von Abmeldungen 1-2 Werktage dauern kann.

>[!MORELIKETHIS]
>
>* [Informationen zur Zeitzone des Empfängers](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Head Start für E-Mail-Programme](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Abbruch des Versands von E-Mail-Programmen mit geplanter Zeitzone des Empfängers](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)
