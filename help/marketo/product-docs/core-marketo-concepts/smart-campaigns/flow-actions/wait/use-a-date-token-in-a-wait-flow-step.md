---
unique-page-id: 1146997
description: Verwenden Sie ein Datums-Token in einem Wartezeitschritt - MarketingToDocs - Produktdokumentation
title: Verwenden eines Datums-Tokens in einem Wartezeitschritt
translation-type: tm+mt
source-git-commit: 728066ab05de82f6123bfaa1f0b05af8632e32b2
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Verwenden eines Datums-Tokens in einem Wartezeitschritt {#use-a-date-token-in-a-wait-flow-step}

Mit dem Schritt zum Warten können Sie die Reise einer Person durch eine intelligente Kampagne bis zu einem bestimmten Datum anhalten, das ein Datums-Token verwendet. Sie können das Enddatum auch um einige Tage ändern.

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>Dies gilt nur für auslösende Kampagnen. Sie können diese Funktion nicht in Batch-Kampagnen verwenden.

1. Ziehen Sie auf der Registerkarte &quot; **Fluss** intelligenter Kampagnen&quot;über den Schritt **&quot;Fluss** warten&quot;.

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. Klicken Sie auf das Zahnradsymbol rechts.

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. Wählen Sie aus der Dropdownliste **Typ** die Option **DatumsToken**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. Wählen Sie ein Datums-Token, um anzugeben, wann der Warten-Schritt enden soll:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. Wenn Sie bis zum nächsten Jahrestag des Datums im aktuellen oder nächsten Kalenderjahr warten möchten, markieren Sie das entsprechende Kästchen.

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >Verwenden Sie diese Option für Datums-Token, die sich auf Daten aus der Vergangenheit beziehen, wie z. B. ein Geburtstag oder ein Beginn.

1. Optional können Sie das Enddatum um eine angegebene Anzahl von Tagen ändern.

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >Sie können auch die Anzahl der Tage mit einem `{{lead.` oder einem `{{company.` Token angeben, das ein ganzzahliges Feld oder ein `{{my.` Token des Zahlentyps darstellt.

1. Klicken Sie auf Speichern.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!NOTE]
   >
   >**Verwandte Artikel**
   >
   >* [Verwenden einer Dauer in einem Wartezeitschritt](use-a-duration-in-a-wait-flow-step.md)
   >* [Verwenden eines bestimmten Datums in einem Schritt mit einem Wartefluss](use-a-specific-date-in-a-wait-flow-step.md)


