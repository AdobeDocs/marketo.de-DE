---
unique-page-id: 10099680
description: Importieren benutzerdefinierter Objektdaten - Marketo Docs - Produktdokumentation
title: Benutzerdefinierte Objektdaten importieren
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 3%

---

# Benutzerdefinierte Objektdaten importieren {#import-custom-object-data}

Benutzerdefinierte Objektdaten lassen sich einfach in Ihre Datenbank importieren. Wenn Sie benutzerdefinierte Objekte mit Unternehmen verwenden, finden Sie weitere Informationen unter [Verwenden benutzerdefinierter Objekte mit Unternehmen](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) .

1. Wechseln Sie in My Marketo zu **[!UICONTROL Database]**.

   ![](assets/import-custom-object-data-1.png)

1. Klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Benutzerdefinierte Objektdaten importieren]** aus.

   ![](assets/import-custom-object-data-2.png)

1. Klicken Sie auf **[!UICONTROL Durchsuchen]** , um die Datendatei zu suchen. Wählen Sie das Dateiformat aus (in diesem Beispiel durch Komma getrennte Werte).

   ![](assets/import-custom-object-data-3.png)

1. Wählen Sie Ihr [!UICONTROL benutzerdefiniertes Objekt] aus.

   ![](assets/import-custom-object-data-4.png)

1. Wählen Sie den [!UICONTROL Deduplizierungsmodus] aus der Dropdownliste aus. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >Verwenden Sie Deduplizierungsfelder als eindeutige Kennungen, wenn Sie benutzerdefinierte Objektdatensätze erstellen oder aktualisieren. In diesem Beispiel wird das Deduplizierungsfeld des benutzerdefinierten Objekts **car** - vin (Fahrzeug-ID-Nummer) verwendet. Wenn Sie nur benutzerdefinierte Objektdatensätze aktualisieren, können Sie das [!UICONTROL Marketo-Handbuch] als [!UICONTROL Deduplizierungsmodus] auswählen.

1. Ordnen Sie jede Spalte einem Marketo-Feld zu und wählen Sie es aus der Dropdownliste aus.

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >Stellen Sie sicher, dass die Werte in Ihrer Datei mit dem Typ des Felds übereinstimmen, mit dem Sie sie abgleichen (z. B. Text, Ganzzahl usw.), da die Datei andernfalls abgelehnt wird.

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/import-custom-object-data-7.png)

1. Klicken Sie auf **[!UICONTROL Importieren]**.

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >Die maximale Größe für benutzerdefinierte Objekte beträgt 100 MB.

   >[!TIP]
   >
   >Geben Sie Ihre E-Mail-Adresse in das Feld **[!UICONTROL Warnhinweis senden an]** ein, und Marketo wird Sie per E-Mail benachrichtigen, wenn Ihr Import abgeschlossen ist!

1. In der rechten oberen Ecke des Bildschirms sehen Sie eine Benachrichtigung, während der Import ausgeführt wird, und die Endergebnisse, wenn der Import abgeschlossen ist.

   ![](assets/import-custom-object-data-9.png)

   Ja!

>[!MORELIKETHIS]
>
>[Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
