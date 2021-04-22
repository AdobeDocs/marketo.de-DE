---
unique-page-id: 10099680
description: Benutzerspezifische Objektdaten importieren - Marketo Docs - Produktdokumentation
title: Benutzerdefinierte Objektdaten importieren
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 3%

---

# Benutzerdefinierte Objektdaten importieren {#import-custom-object-data}

Benutzerdefinierte Objektdaten lassen sich problemlos in Ihre Datenbank importieren. Wenn Sie benutzerdefinierte Objekte mit Firmen verwenden, finden Sie weitere Informationen unter [Verwenden von benutzerdefinierten Objekten mit Firmen](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies).

1. Wechseln Sie in &quot;Mein Marketo&quot;zu **Datenbank**.

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
   >Verwenden Sie Deduplizierungsfelder als eindeutige Bezeichner, wenn Sie benutzerdefinierte Objektdatensätze erstellen oder aktualisieren. In diesem Beispiel wird das Deduplizierungsfeld des benutzerdefinierten Objekts **car** - vin (Fahrzeug-ID-Nummer) verwendet. Wenn Sie nur benutzerdefinierte Objektdatensätze aktualisieren, können Sie die Marketo-Hilfslinie als Deduplizierungsmodus auswählen.

1. Ordnen Sie jede Spalte einem Marketo-Feld zu und wählen Sie es aus der Dropdownliste aus.

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
   >Geben Sie Ihre E-Mail-Adresse in das Feld **Warnung senden an:** ein, und Marketo wird Sie per E-Mail benachrichtigen, wenn Ihr Import abgeschlossen ist!

1. In der oberen rechten Ecke des Bildschirms sehen Sie eine Benachrichtigung, während der Import ausgeführt wird, und die Endergebnisse, sobald der Import abgeschlossen ist.

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   Jay!

>[!MORELIKETHIS]
>
>[Benutzerdefinierte Marketo-Objekte](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
