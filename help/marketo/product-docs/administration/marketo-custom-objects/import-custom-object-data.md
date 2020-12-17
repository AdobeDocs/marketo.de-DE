---
unique-page-id: 10099680
description: Importieren benutzerdefinierter Objektdaten - Marketing to Docs - Produktdokumentation
title: Benutzerspezifische Objektdaten importieren
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Benutzerspezifische Objektdaten importieren {#import-custom-object-data}

Benutzerdefinierte Objektdaten lassen sich problemlos in Ihre Datenbank importieren. Wenn Sie benutzerdefinierte Objekte mit Firmen verwenden, finden Sie weitere Informationen unter [Verwenden von benutzerdefinierten Objekten mit Firmen](http://docs.marketo.com/display/DOCS/Understanding+Marketo+Custom+Objects#UnderstandingMarketoCustomObjects-customcompanyUsingCustomObjectswithCompanies).

1. Wechseln Sie in &quot;My Marketo&quot;zu **Database**.

   ![](assets/db-1.png)

1. Klicken Sie auf **Neu** und wählen Sie **Benutzerspezifische Objektdaten importieren**.

   ![](assets/image2016-4-7-10-6-54.png)

1. Klicken Sie auf **Durchsuchen**, um die Datendatei zu suchen. Wählen Sie das Dateiformat aus (in diesem Beispiel durch Kommas getrennte Werte).

   ![](assets/image2016-4-13-14-3a21-3a53.png)

1. Wählen Sie Ihr benutzerdefiniertes Objekt aus.

   ![](assets/image2016-4-13-14-3a24-3a54.png)

1. Wählen Sie den Deduplizierungsmodus aus der Dropdownliste. Klicken Sie auf **Weiter**.

   ![](assets/image2016-4-13-14-3a28-3a7.png)

   >[!NOTE]
   >
   >Verwenden Sie Deduplizierungsfelder als eindeutige Bezeichner, wenn Sie benutzerdefinierte Objektdatensätze erstellen oder aktualisieren. In diesem Beispiel wird das Deduplizierungsfeld des benutzerdefinierten Objekts **car** - vin (Fahrzeug-ID-Nummer) verwendet. Wenn Sie nur benutzerdefinierte Objektdatensätze aktualisieren, können Sie als Deduplizierungsmodus die Marker-Hilfslinie auswählen.

1. Ordnen Sie jede Spalte einem Marker-Feld zu und wählen Sie es aus der Dropdownliste aus.

   ![](assets/image2016-4-13-14-3a36-3a57.png)

   >[!NOTE]
   >
   >Vergewissern Sie sich, dass die Werte in Ihrer Datei mit dem Typ des Felds übereinstimmen, mit dem Sie sie abgleichen (z. B. Text, Ganzzahl usw.). Andernfalls wird die Datei abgelehnt.

1. Klicken Sie auf **Weiter**.

   ![](assets/image2016-4-13-14-3a38-3a41.png)

1. Klicken Sie auf **Import**.

   ![](assets/image2016-4-7-13-3a15-3a9.png)

   >[!NOTE]
   >
   >Die maximale Größe für benutzerdefinierte Objekte beträgt 100 MB.

   >[!TIP]
   >
   >Geben Sie Ihre E-Mail-Adresse in das Feld **Warnung senden an:** ein, und Marketo wird Ihnen eine E-Mail senden, wenn Ihr Import abgeschlossen ist!

1. In der oberen rechten Ecke des Bildschirms sehen Sie eine Benachrichtigung, während der Import ausgeführt wird, und die Endergebnisse, sobald der Import abgeschlossen ist.

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   Jay!

>[!MORELIKETHIS]
>
>* [Erläuterungen zu benutzerdefinierten Objekten](understanding-marketo-custom-objects.md)

>



