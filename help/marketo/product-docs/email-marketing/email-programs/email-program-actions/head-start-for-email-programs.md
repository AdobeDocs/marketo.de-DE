---
unique-page-id: 10097202
description: Head Start for Email Programs - Marketo Docs - Product Documentation
title: Head Start for Email Programs
exl-id: f7c8b082-4d83-4e3b-8aa4-7b252e3dacd3
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Head Start for Email Programs {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[E-Mail-Programm erstellen](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

Wenn Sie ein Datum/eine Uhrzeit für ein E-Mail-Programm auswählen, bestimmt dies, wann das Programm mit der Verarbeitung beginnen wird. Wenn Sie möchten, dass Ihre E-Mails zum ausgewählten Zeitpunkt gestartet werden, bietet Ihnen Head Start diese Option, indem Sie das Programm im Voraus verarbeiten.

## Standardkopfstart {#standard-head-start}

1. Klicken Sie **Marketing-Aktivitäten**.

   ![](assets/one-1.png)

1. Suchen und wählen Sie Ihr E-Mail-Programm.

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Head Start kann nicht mit A/B-Tests verwendet werden.

1. Wählen Sie in der Kachel Zeitplan Ihre E-Mail aus und klicken Sie dann auf **Head Start**.

   ![](assets/three-1.png)

   Wenn „Head Start“ ausgewählt ist, beginnt das Programm etwa 12 Stunden vor der geplanten Zeit mit der Verarbeitung. Sobald die Verarbeitung beginnt, wird das Programm gesperrt.

   >[!CAUTION]
   >
   >Alle Personen aus Ihrer Zielgruppe, die sich nach der Programmsperre abmelden, erhalten weiterhin die E-Mail. Es wird empfohlen, die Abmelde-Benachrichtigung so anzupassen, dass die Bearbeitung von Abmeldungen 1-2 Werktage dauern kann.

1. Klicken Sie **Programm genehmigen**.

   ![](assets/four-1.png)

   Nach der Programmgenehmigung gibt es vier verschiedene Status, die auf der Kachel Genehmigung angezeigt werden können.

   * **Warten auf Ausführung:** Nachdem das Programm genehmigt wurde.
   * **Verarbeitung gestartet, wartet auf Ausführung:** Verarbeitung läuft.
   * **Verarbeitung abgeschlossen, wartet auf Ausführung:** Verarbeitung abgeschlossen, E-Mail wartet jetzt auf den geplanten Start.
   * **Beendet:** Programm abgeschlossen.

   >[!TIP]
   >
   >Möchten Sie den Vorgang abbrechen, nachdem das Programm gesperrt wurde, aber bevor die E-Mail gesendet wird? Kein Problem! Klicken Sie einfach **Programm abbrechen** unten rechts auf der Kachel Genehmigung .

   >[!NOTE]
   >
   >Wenn Sie die Genehmigung für Ihr E-Mail-Programm mit weniger als 12 Stunden vor der geplanten Laufzeit aufheben, aber dann Ihre Meinung ändern, müssen Sie ein neues Datum/eine neue Uhrzeit auswählen, das/die mindestens 12 Stunden vor der Genehmigung liegt.

## Head Start with Recipient Time Zone {#head-start-with-recipient-time-zone}

Unsere bestehende Head Start-Funktion erfordert, dass das Programm mindestens 12 Stunden im Voraus geplant wird. Was bedeutet dies für die Zeitzone des Empfängers? Erinnern Sie sich daran, dass wir, wenn die Zeitzone des Empfängers aktiv ist, das E-Mail-Programm um Mitternacht in der frühesten Zeitzone ausführen (UTC +14:00). Um also **sowohl** Kopfstart- als auch Empfängerzeitzone zu aktivieren, müssen Programme geplant werden **mindestens 12 Stunden vor der frühesten Zeitzone (UTC +14:00**).

Wenn Sie also in Amerika/Los Angeles sind und sowohl die Zeitzone „Head Start“ als auch die Zeitzone „Empfänger“ aktivieren möchten, müssen Sie das Programm **34 Stunden)**. Wie sind wir zu dieser Nummer gekommen?

![](assets/image2017-12-5-13-3a11-3a46.png)

[Weitere Informationen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) zum Planen von E-Mail-Programmen mit der Zeitzone des Empfängers.

>[!MORELIKETHIS]
>
>* [E-Mail-Programm planen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [Planen von E-Mail-Programmen mit Zeitzone des Empfängers](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Informationen zur Zeitzone des Empfängers](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
