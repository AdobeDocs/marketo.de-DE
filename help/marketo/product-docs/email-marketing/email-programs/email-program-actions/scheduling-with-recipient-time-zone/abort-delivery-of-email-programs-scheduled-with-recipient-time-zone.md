---
unique-page-id: 13795727
description: Abbruch des Versands von E-Mail-Programmen, die mit der Zeitzone der Empfänger geplant sind - Marketo Docs - Produktdokumentation
title: Abbruch des Versands von E-Mail-Programmen mit Zeitzone des Empfängers
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Abbruch des Versands von E-Mail-Programmen mit Zeitzone des Empfängers {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

In Notfällen können Sie den Versand eines E-Mail-Programms abbrechen, das bereits mit aktivierter Zeitzone für Empfänger gestartet wurde.

Da E-Mail-Programme, die mit der Zeitzone der Empfänger geplant sind, bis zu 24 Stunden lang laufen können, werden nach dem Abbruch des Programmversands alle nachfolgenden Sendungen abgebrochen.

1. Wählen Sie das E-Mail-Programm aus, das Sie abbrechen möchten, und klicken Sie dann unter der Kachel Genehmigung im Control Panel auf **Versand abbrechen** .

   ![](assets/ptz-abortdelivery.png)

1. Bestätigen Sie, dass Sie den Versand abbrechen möchten, indem Sie auf **Abbruch** klicken.

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. Nach dem Abbruch sieht das Raster **Ergebnisse** Ihres E-Mail-Programms ungefähr so aus: Alle nachfolgenden Sendungen werden abgebrochen und in der Spalte **Aktivitätstyp** als &quot;E-Mail-Bounce Soft&quot; angezeigt.

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >Abgebrochene E-Mails werden **nicht** als Softbounce *angezeigt, bis* der Zeitpunkt erreicht ist, zu dem sie ursprünglich in ihrer jeweiligen Zeitzone zur Auslieferung geplant waren. Bis zu diesem Zeitpunkt werden sie weiterhin als &quot;E-Mail senden&quot;angezeigt.

1. Im Raster können Sie auf eine beliebige E-Mail klicken, um Aktivitätsdetails anzuzeigen. Bei einem abgebrochenen Versand sieht das Popup-Fenster mit Details wie folgt aus:

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [Verstehen der Zeitzone des Empfängers](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [E-Mail-Programme mit der Zeitzone des Empfängers planen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
