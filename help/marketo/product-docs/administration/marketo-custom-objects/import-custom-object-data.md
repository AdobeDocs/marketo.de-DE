---
unique-page-id: 10099680
description: Importieren benutzerdefinierter Objektdaten - Marketo Docs - Produktdokumentation
title: Benutzerdefinierte Objektdaten importieren
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 3%

---

# Benutzerdefinierte Objektdaten importieren {#import-custom-object-data}

Benutzerdefinierte Objektdaten lassen sich einfach in Ihre Datenbank importieren. Wenn Sie benutzerdefinierte Objekte mit Unternehmen verwenden, finden Sie weitere Informationen unter [Verwenden benutzerdefinierter Objekte für Unternehmen](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) für weitere Informationen.

1. Wechseln Sie in meiner Marketo zu **Datenbank**.

   ![](assets/db-1.png)

1. Klicken **Neu** und wählen Sie **Benutzerdefinierte Objektdaten importieren**.

   ![](assets/image2016-4-7-10-6-54.png)

1. Klicken **Durchsuchen** , um die Datendatei zu suchen. Wählen Sie das Dateiformat aus (in diesem Beispiel durch Komma getrennte Werte).

   ![](assets/image2016-4-13-14-3a21-3a53.png)

1. Wählen Sie das benutzerdefinierte Objekt aus.

   ![](assets/image2016-4-13-14-3a24-3a54.png)

1. Wählen Sie den Deduplizierungsmodus aus der Dropdown-Liste aus. Klicken **Nächste**.

   ![](assets/image2016-4-13-14-3a28-3a7.png)

   >[!NOTE]
   >
   >Verwenden Sie Deduplizierungsfelder als eindeutige Kennungen, wenn Sie benutzerdefinierte Objektdatensätze erstellen oder aktualisieren. In diesem Beispiel wird das Deduplizierungsfeld des **Auto** benutzerdefiniertes Objekt - vin (Fahrzeug-ID-Nummer). Wenn Sie nur benutzerdefinierte Objektdatensätze aktualisieren, können Sie das Marketo-Handbuch als Deduplizierungsmodus auswählen.

1. Ordnen Sie jede Spalte einem Marketo-Feld zu und wählen Sie es aus der Dropdown-Liste aus.

   ![](assets/image2016-4-13-14-3a36-3a57.png)

   >[!NOTE]
   >
   >Stellen Sie sicher, dass die Werte in Ihrer Datei mit dem Typ des Felds übereinstimmen, mit dem Sie sie abgleichen (z. B. Text, Ganzzahl usw.), da die Datei andernfalls abgelehnt wird.

1. Klicken **Nächste**.

   ![](assets/image2016-4-13-14-3a38-3a41.png)

1. Klicken **Import**.

   ![](assets/image2016-4-7-13-3a15-3a9.png)

   >[!NOTE]
   >
   >Die maximale Größe für benutzerdefinierte Objekte beträgt 100 MB.

   >[!TIP]
   >
   >Geben Sie Ihre E-Mail-Adresse im **Warnhinweis senden an:** und Marketo wird Ihnen eine E-Mail senden, wenn Sie Ihren Import abgeschlossen haben.

1. In der rechten oberen Ecke des Bildschirms sehen Sie eine Benachrichtigung, während der Import ausgeführt wird, und die Endergebnisse, wenn der Import abgeschlossen ist.

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   Ja!

>[!MORELIKETHIS]
>
>[Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
