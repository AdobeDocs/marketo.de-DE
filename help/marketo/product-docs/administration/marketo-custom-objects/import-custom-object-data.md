---
unique-page-id: 10099680
description: Importieren benutzerdefinierter Objektdaten - Marketo Docs - Produktdokumentation
title: Benutzerdefinierte Objektdaten importieren
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
source-git-commit: 99b11e17e9c2255a19c658b166e7b38c45cf1001
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 3%

---

# Benutzerdefinierte Objektdaten importieren {#import-custom-object-data}

Benutzerdefinierte Objektdaten lassen sich einfach in Ihre Datenbank importieren. Wenn Sie benutzerdefinierte Objekte mit Unternehmen verwenden, finden Sie weitere Informationen unter [Verwenden benutzerdefinierter Objekte für Unternehmen](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) für weitere Informationen.

1. Wechseln Sie in meiner Marketo zu **Datenbank**.

   ![](assets/import-custom-object-data-1.png)

1. Klicken **Neu** und wählen Sie **Benutzerdefinierte Objektdaten importieren**.

   ![](assets/import-custom-object-data-2.png)

1. Klicken **Durchsuchen** , um die Datendatei zu suchen. Wählen Sie das Dateiformat aus (in diesem Beispiel durch Komma getrennte Werte).

   ![](assets/import-custom-object-data-3.png)

1. Wählen Sie das benutzerdefinierte Objekt aus.

   ![](assets/import-custom-object-data-4.png)

1. Wählen Sie den Deduplizierungsmodus aus der Dropdown-Liste aus. Klicken **Nächste**.

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >Verwenden Sie Deduplizierungsfelder als eindeutige Kennungen, wenn Sie benutzerdefinierte Objektdatensätze erstellen oder aktualisieren. In diesem Beispiel wird das Deduplizierungsfeld des **Auto** benutzerdefiniertes Objekt - vin (Fahrzeug-ID-Nummer). Wenn Sie nur benutzerdefinierte Objektdatensätze aktualisieren, können Sie das Marketo-Handbuch als Deduplizierungsmodus auswählen.

1. Ordnen Sie jede Spalte einem Marketo-Feld zu und wählen Sie es aus der Dropdown-Liste aus.

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >Stellen Sie sicher, dass die Werte in Ihrer Datei mit dem Typ des Felds übereinstimmen, mit dem Sie sie abgleichen (z. B. Text, Ganzzahl usw.), da die Datei andernfalls abgelehnt wird.

1. Klicken **Nächste**.

   ![](assets/import-custom-object-data-7.png)

1. Klicken **Import**.

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >Die maximale Größe für benutzerdefinierte Objekte beträgt 100 MB.

   >[!TIP]
   >
   >Geben Sie Ihre E-Mail-Adresse im **Warnhinweis senden an:** und Marketo wird Ihnen eine E-Mail senden, wenn Sie Ihren Import abgeschlossen haben.

1. In der rechten oberen Ecke des Bildschirms sehen Sie eine Benachrichtigung, während der Import ausgeführt wird, und die Endergebnisse, wenn der Import abgeschlossen ist.

   ![](assets/import-custom-object-data-9.png)

   Ja!

>[!MORELIKETHIS]
>
>[Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
