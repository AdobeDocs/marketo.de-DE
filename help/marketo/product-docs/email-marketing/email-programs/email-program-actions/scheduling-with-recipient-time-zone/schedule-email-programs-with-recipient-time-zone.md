---
unique-page-id: 12982903
description: Planen von E-Mail-Programmen mit der Zeitzone der Empfänger - Marketo Docs - Produktdokumentation
title: E-Mail-Programme mit der Zeitzone der Empfänger planen
exl-id: d0c3f3c1-9f21-4081-818d-7c5cb1766915
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# E-Mail-Programme mit der Zeitzone der Empfänger planen {#schedule-email-programs-with-recipient-time-zone}

Es gibt zwei mögliche Szenarien bei der Planung eines E-Mail-Programms, während die Zeitzone des Empfängers aktiviert ist:

1. Planen der Ausführung von **innerhalb** in den nächsten 25 Stunden
1. Planen der zukünftigen Ausführung von **mehr** als 25 Stunden (d. h. nächste Woche) des Programms

## Szenario 1: Innerhalb von 25 Stunden {#scenario-within-hours}

Angenommen, Sie genehmigen ein E-Mail-Programm mit aktivierter Zeitzone der Empfänger und einer geplanten Versandzeit innerhalb der nächsten 25 Stunden. Möglicherweise befinden sich Personen in Ihrer intelligenten Liste in Zeitzonen, in denen die geplante Zeit bereits verstrichen ist.

In diesem Szenario können Sie entscheiden, was mit dieser Untergruppe qualifizierter Personen zu tun ist. Klicken Sie auf das Zahnradsymbol neben **Zeitzone des Empfängers** in der Kachel **Zeitplan** des E-Mail-Programms.

![](assets/image2017-12-5-10-3a46-3a42.png)

Zwei Optionen stehen zur Verfügung:

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Definition**
>
>* **Versenden Sie den folgenden Tag in der Zeitzone des Empfängers**: Wenn die E-Mail am Dienstag um 9:00 Uhr gesendet werden soll, erhalten qualifizierte Personen, die in Zeitzonen leben, in denen die geplante Zeit bereits verstrichen ist, die E-Mail am *Mittwoch* um 9:00 Uhr.
>
>* **Versand unter Verwendung der standardmäßigen Programmsetzeit**: Wenn die E-Mail am Dienstag um 9:00 Uhr gesendet werden soll, erhalten qualifizierte Personen, die in Zeitzonen leben, in denen die geplante Zeit bereits verstrichen ist, die E-Mail _basierend auf Ihren Zeitzoneneinstellungen für das Abonnement_. Wenn Sie also die Zeitzoneneinstellungen für Ihr [Abonnement ](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md) auf PDT America/Los Angeles setzen, erhalten diese Empfänger die E-Mail am Dienstag um 9:00 Uhr PDT (egal zu welcher Uhrzeit sie in ihrer eigenen Zeitzone liegen).

>[!NOTE]
>
>[Erfahren Sie mehr](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) darüber, wie Marketo Zeitzonen für Empfänger berechnet.

Betrachten wir dieses Szenario im Detail. Angenommen, Sie sind in San Francisco und planen eine E-Mail um 7:00 Uhr für einen Versand um 9:00 Uhr (1). **** In Ihrer intelligenten Liste befinden sich Personen aus den folgenden Regionen:

* San Francisco
* Texas
* New York
* Italien

![](assets/image2017-12-6-10-3a52-3a41.png)

9:00 Uhr in New York und Italien bereits vergangen, sodass qualifizierte Personen in diesen beiden Zeitzonen die E-Mail anhand der **Zeitzoneneinstellungen** erhalten:

* **Stellen Sie den folgenden Tag in der Zeitzone des Empfängers bereit:** Mittwoch um 9:00 Uhr in der jeweiligen Zeitzone, **ODER**

* **Versand mit der Standardeinstellung des Programms**: Dienstag um 9:00 Uhr PDT (New York - 22:00 Uhr EDT und Italien - 18:00 Uhr CET).

Sobald Sie Ihr Programm validieren, wird es innerhalb von 15 Minuten ausgeführt.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Obwohl das Programm den _Prozess_ des Versands von E-Mails in 15 Minuten startet, werden E-Mails zu diesem Zeitpunkt nicht _zugestellt_. Die Empfänger erhalten weiterhin E-Mails, die auf den von Ihnen gewählten **Zeitzoneneinstellungen** basieren.

## Szenario 2: Mehr als 25 Stunden {#scenario-more-than-hours}

In diesem zweiten Szenario genehmigen Sie ein E-Mail-Programm mit aktivierter **Zeitzone des Empfängers** und einer geplanten Versandzeit von mehr als 25 Stunden in der Zukunft. In diesem Fall beginnt das Programm zur geplanten Zeit in der Zeitzone **frühestens** der Welt (UTC + 14:00). Es kann Personen geben, die sich für Ihre Smart-Liste in jeder Zeitzone auf der ganzen Welt qualifizieren. Deshalb können wir mit der frühesten Zeitzone die E-Mail zum geplanten Datum/zur geplanten Uhrzeit an alle Empfänger in ihrer jeweiligen Zeitzone senden.

**Head Start**

Sprechen wir nun darüber, wie [Head Start](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) mit **Recipient Time Zone** funktioniert. Für unsere bestehende Head Start-Funktion muss das Programm mindestens 12 Stunden im Voraus geplant werden. Was bedeutet das für die Zeitzone der Empfänger? Wenn die Zeitzone des Empfängers aktiviert ist, starten wir die Ausführung des E-Mail-Programms zum geplanten Zeitpunkt in der frühesten Zeitzone (UTC +14:00). Um also **sowohl** Head Start als auch die Zeitzone des Empfängers zu aktivieren, müssen E-Mail-Programme in UTC +14:00 **mindestens 12 Stunden vor der geplanten Zeit geplant werden.**

Wenn Sie sich also in Amerika/Los Angeles befinden und sowohl die Head Start- als auch die Recipient Time Zone aktivieren möchten, müssen Sie das Programm **34 Stunden** im Voraus planen. Wie sind wir auf diese Zahl gekommen?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

Kurz gesagt, E-Mail-Programme, die mit der Zeitzone des Empfängers geplant sind, müssen zur geplanten Zeit in der frühesten Zeitzone ausgeführt werden (d. h., wo sie zuerst Mitternacht erreichen), um jede Zeitzone aufzunehmen. Wenn Sie also ein E-Mail-Programm planen...

* **bei einer Bereitstellungszeit _innerhalb von_ 25 Stunden** beginnt das Programm innerhalb von 15 Minuten. Empfänger, die die geplante Zeit bereits überschritten haben, erhalten die E-Mail entsprechend den von Ihnen ausgewählten Zeitzoneneinstellungen.
* **bei einer Versandzeit von _mehr als_ 25 Stunden in der Zukunft** beginnt das Programm zur geplanten Zeit in der frühesten Zeitzone (UTC +14:00).
* **Mit Head Start** beginnt das Programm 12 Stunden vor der geplanten Zeit in der frühesten Zeitzone (UTC +14:00).

>[!CAUTION]
>
>Jeder, der sich zwischen dem Beginn des E-Mail-Versands und dem tatsächlichen Versand abmeldet, erhält weiterhin die E-Mail. Es wird empfohlen, Ihre Abmelde-Benachrichtigung so anzupassen, dass die Verarbeitung von Abmeldungen 1-2 Werktage dauern kann.

>[!MORELIKETHIS]
>
>* [Verstehen der Zeitzone des Empfängers](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Head Start für E-Mail-Programme](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Abbruch des Versands von E-Mail-Programmen, die mit der Zeitzone des Empfängers geplant sind](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)
