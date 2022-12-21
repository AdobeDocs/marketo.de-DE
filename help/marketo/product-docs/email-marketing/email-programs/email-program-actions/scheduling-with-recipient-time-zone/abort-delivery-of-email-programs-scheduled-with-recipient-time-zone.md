---
unique-page-id: 13795727
description: Abbruch des Versands von E-Mail-Programmen, die mit der Zeitzone der Empfänger geplant sind - Marketo Docs - Produktdokumentation
title: Abbruch des Versands von E-Mail-Programmen, die mit der Zeitzone des Empfängers geplant sind
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Abbruch des Versands von E-Mail-Programmen, die mit der Zeitzone des Empfängers geplant sind {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

In Notfällen können Sie den Versand eines E-Mail-Programms abbrechen, das bereits mit aktivierter Zeitzone für Empfänger gestartet wurde.

Da E-Mail-Programme, die mit der Zeitzone der Empfänger geplant sind, bis zu 24 Stunden lang laufen können, werden nach dem Abbruch des Programmversands alle nachfolgenden Sendungen abgebrochen.

1. Wählen Sie das E-Mail-Programm aus, das Sie abbrechen möchten, und klicken Sie auf **Auslieferung abbrechen** unter der Kachel Genehmigung im Bedienfeld.

   ![](assets/ptz-abortdelivery.png)

1. Vergewissern Sie sich, dass Sie den Versand abbrechen möchten, indem Sie auf **Abbruch**.

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. Nach dem Abbruch wird die **Ergebnisse** Das Raster Ihres E-Mail-Programms sieht ungefähr wie das unten stehende aus. Alle nachfolgenden Sendungen werden abgebrochen und als &quot;E-Mail Bounce Soft&quot; im **Aktivitätstyp** Spalte.

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >Abgebrochene E-Mails werden **not** als Softbounce anzeigen *bis* der Zeitpunkt, zu dem die Auslieferung ursprünglich in der jeweiligen Zeitzone geplant war. Bis zu diesem Zeitpunkt werden sie weiterhin als &quot;E-Mail senden&quot;angezeigt.

1. Im Raster können Sie auf eine beliebige E-Mail klicken, um Aktivitätsdetails anzuzeigen. Bei einem abgebrochenen Versand sieht das Popup-Fenster mit Details wie folgt aus:

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [Verstehen der Zeitzone eines Empfängers](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [E-Mail-Programme mit der Zeitzone der Empfänger planen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)

