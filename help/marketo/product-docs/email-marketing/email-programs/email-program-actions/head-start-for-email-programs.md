---
unique-page-id: 10097202
description: Head Beginn für E-Mail-Programme - Marketing Docs - Produktdokumentation
title: Beginn für E-Mail-Programme
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---


# Head-Beginn für E-Mail-Programm {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>* [E-Mail-Programm erstellen](../../../../product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

>



Wenn Sie ein Datum/eine Uhrzeit für ein E-Mail-Programm auswählen, wird festgelegt, wann das Programm mit der Verarbeitung beginnt. Wenn Sie möchten, dass Ihre E-Mails zum ausgewählten Zeitpunkt gestartet werden, gibt Ihnen Head Beginn diese Option, indem Sie das Programm im Voraus verarbeiten.

## Beginn der Standardüberschrift {#standard-head-start}

1. Klicken Sie auf **Marketing-Aktivitäten**.

   ![](assets/one-1.png)

1. Suchen und wählen Sie Ihr E-Mail-Programm aus.

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Head-Beginn kann nicht mit A/B-Tests verwendet werden.

1. Planen Sie in der Kachel Plan Ihre E-Mail und wählen Sie dann das Feld **Überschrift Beginn**.

   ![](assets/three-1.png)

   Bei Auswahl des Head-Beginns beginnt das Programm etwa 12 Stunden vor der geplanten Zeit mit der Verarbeitung. Nach der Verarbeitung von Beginn ist das Programm gesperrt.

   >[!CAUTION]
   >
   >Jeder von Ihrer Audience, der sich nach dem Sperren des Programms abmeldet, erhält die E-Mail noch. Es wird empfohlen, die Benachrichtigung zum Abbestellen des Abonnements so anzupassen, dass die Verarbeitung von Abbestellungen 1-2 Werktage dauern kann.

1. Klicken Sie auf **Programm genehmigen**.

   ![](assets/four-1.png)

   Nach der Genehmigung durch das Programm befinden sich vier verschiedene Statusangaben auf der Genehmigungskachel.

   * **Warten auf Ausführung:** Nachdem das Programm genehmigt wurde.
   * **Verarbeitung gestartet und wartet auf Ausführung:** Verarbeitung wird ausgeführt.
   * **Verarbeitung abgeschlossen, auf Ausführung warten:** Verarbeitung abgeschlossen, E-Mail wartet jetzt auf geplante Zeit zum Starten.
   * **Fertig gestellt:** Programm abgeschlossen.

   >[!TIP]
   >
   >Möchten Sie den Vorgang abbrechen, nachdem das Programm gesperrt wurde, aber bevor die E-Mail gesendet wird? Kein Problem! Klicken Sie einfach unten rechts in der Genehmigungskachel auf **Programm abbrechen**.

   >[!NOTE]
   >
   >Wenn Sie Ihr E-Mail-Programm weniger als 12 Stunden vor der geplanten Laufzeit ablehnen und dann Ihre Meinung ändern, müssen Sie ein neues Datum/eine neue Uhrzeit auswählen, das mindestens 12 Stunden vor der Genehmigung liegt.

## Head-Beginn mit Empfänger-Zeitzone {#head-start-with-recipient-time-zone}

Für unsere bestehende Kopfzeilenfunktion ist es erforderlich, dass das Programm mindestens 12 Stunden im Voraus geplant wird. Was bedeutet das für die Zeitzone des Empfängers? Denken Sie daran, dass, wenn die Zeitzone des Empfängers aktiv ist, wir Beginn das E-Mail-Programm um Mitternacht in der frühesten Zeitzone (UTC +14:00) ausführen. Um **beide** Überschrift- und Empfänger-Zeitzone zu aktivieren, müssen Programm daher mindestens 12 Stunden vor der frühesten Zeitzone geplant werden (UTC +14:00 **).**

Das bedeutet, dass Sie, wenn Sie in Amerika/Los Angeles sind und sowohl Head-Beginn als auch Empfänger-Zeitzone aktivieren möchten, das Programm **34 Stunden** im Voraus planen müssen. Wie sind wir zu dieser Zahl gekommen?

![](assets/image2017-12-5-13-3a11-3a46.png)

[Erfahren Sie ](scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) mehr darüber, wie Sie E-Mail-Programm mit der Zeitzone des Empfängers planen.

>[!MORELIKETHIS]
>
>* [Planen Ihres E-Mail-Programms](schedule-your-email-program.md)
>* [E-Mail-Programm mit Zeitzone des Empfängers planen](scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Die Zeitzone des Empfängers](scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)

>



