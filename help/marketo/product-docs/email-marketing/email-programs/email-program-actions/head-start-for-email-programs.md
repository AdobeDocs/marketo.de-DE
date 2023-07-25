---
unique-page-id: 10097202
description: Head Start für E-Mail-Programme - Marketo-Dokumente - Produktdokumentation
title: Abteilungsstart für E-Mail-Programme
exl-id: f7c8b082-4d83-4e3b-8aa4-7b252e3dacd3
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Abteilungsstart für E-Mail-Programme {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[E-Mail-Programm erstellen](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

Wenn Sie ein Datum/eine Uhrzeit für ein E-Mail-Programm auswählen, wird festgelegt, wann die Verarbeitung des Programms beginnt. Wenn Ihre E-Mails zum ausgewählten Zeitpunkt gestartet werden sollen, bietet Ihnen Head Start diese Option, indem Sie das Programm im Voraus verarbeiten.

## Standardkopfzeilenstart {#standard-head-start}

1. Klicken **Marketingaktivitäten**.

   ![](assets/one-1.png)

1. Wählen Sie Ihr E-Mail-Programm aus.

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Head Start kann nicht mit A/B-Tests verwendet werden.

1. Planen Sie Ihre E-Mail in der Kachel Planung und wählen Sie dann die **Head Start** ankreuzen.

   ![](assets/three-1.png)

   Wenn Head Start ausgewählt ist, beginnt das Programm etwa 12 Stunden vor der geplanten Zeit mit der Verarbeitung. Sobald die Verarbeitung beginnt, wird das Programm gesperrt.

   >[!CAUTION]
   >
   >Jeder, der sich von Ihrer Audience abmeldet, nachdem das Programm gesperrt wurde, erhält weiterhin die E-Mail. Es wird empfohlen, Ihre Abmelde-Benachrichtigung so anzupassen, dass die Verarbeitung von Abmeldungen 1-2 Werktage dauern kann.

1. Klicken **Programm genehmigen**.

   ![](assets/four-1.png)

   Nach der Programmgenehmigung gibt es vier verschiedene Status, die Sie auf der Kachel Genehmigung sehen können.

   * **Warten auf Ausführung:** Nach Genehmigung des Programms.
   * **Die Verarbeitung wurde gestartet und wartet auf die Ausführung:** Die Verarbeitung wird ausgeführt.
   * **Verarbeitung abgeschlossen, Warten auf Ausführung:** Verarbeitung abgeschlossen, E-Mail wartet nun auf die geplante Startzeit.
   * **Abgeschlossen:** Programm abgeschlossen.

   >[!TIP]
   >
   >Möchten Sie abbrechen, nachdem das Programm gesperrt wurde, aber bevor die E-Mail gesendet wird? Kein Problem! Einfaches Klicken **Programm abbrechen** rechts unten in der Kachel Genehmigung .

   >[!NOTE]
   >
   >Wenn Sie die Genehmigung Ihres E-Mail-Programms weniger als 12 Stunden vor der geplanten Laufzeit aufheben, sich dann aber anders entscheiden, müssen Sie ein neues Datum/eine neue Uhrzeit auswählen, das mindestens 12 Stunden vor der Genehmigung liegt.

## Head Start mit Zeitzone des Empfängers {#head-start-with-recipient-time-zone}

Für unsere bestehende Head Start-Funktion muss das Programm mindestens 12 Stunden im Voraus geplant werden. Was bedeutet das für die Zeitzone der Empfänger? Denken Sie daran, dass wir, wenn die Zeitzone des Empfängers aktiv ist, mit der Ausführung des E-Mail-Programms um Mitternacht in der frühesten Zeitzone beginnen (UTC +14:00). Um **both** Start- und Zeitzone der Empfänger, Programme müssen geplant werden **mindestens 12 Stunden vor der frühesten Zeitzone (UTC +14:00**.

Wenn Sie sich also in Amerika/Los Angeles befinden und sowohl Head Start als auch Recipient Time Zone aktivieren möchten, müssen Sie das Programm planen **34 Stunden** im Voraus. Wie sind wir auf diese Zahl gekommen?

![](assets/image2017-12-5-13-3a11-3a46.png)

[Weitere Infos](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) Informationen zur Planung von E-Mail-Programmen mit der Zeitzone der Empfänger.

>[!MORELIKETHIS]
>
>* [E-Mail-Programm planen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [E-Mail-Programme mit der Zeitzone der Empfänger planen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Verstehen der Zeitzone eines Empfängers](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
