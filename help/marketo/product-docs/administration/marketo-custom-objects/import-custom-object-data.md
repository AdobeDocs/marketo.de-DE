---
unique-page-id: 10099680
description: Schritte zum Importieren benutzerdefinierter Objektdaten mithilfe einer CSV-Datei, einschließlich der Auswahl des benutzerdefinierten Objekts, des Deduplizierungsmodus und der Feldzuordnung.
title: Importieren von benutzerdefinierten Objektdaten
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
feature: Custom Objects
TQID: https://experienceleague.adobe.com/eWVHHONaYWOgc8s6AuB-PpEr-m3G5ixHwf5IondqZKE
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 252
ht-degree: 4%

---

# Importieren von benutzerdefinierten Objektdaten {#import-custom-object-data}

Gehen Sie wie folgt vor, um benutzerdefinierte Objektdaten in Ihre Datenbank zu importieren. Wenn Sie benutzerdefinierte Objekte mit Unternehmen verwenden, finden Sie unter [Verwenden benutzerdefinierter Objekte mit Unternehmen](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) weitere Informationen.

1. Navigieren Sie in My Marketo zu **[!UICONTROL Datenbank]**.

   ![](assets/import-custom-object-data-1.png)

1. Klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Benutzerdefinierte Objektdaten importieren]**.

   ![](assets/import-custom-object-data-2.png)

1. Klicken Sie **[!UICONTROL Durchsuchen]**, um die Datendatei zu suchen. Wählen Sie das Dateiformat aus (in diesem Beispiel durch Komma getrennte Werte).

   ![](assets/import-custom-object-data-3.png)

1. Wählen Sie Ihr [!UICONTROL benutzerdefiniertes Objekt] aus.

   ![](assets/import-custom-object-data-4.png)

1. Wählen Sie [!UICONTROL Deduplizierungsmodus] aus der Dropdown-Liste aus. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >Verwenden Sie ein oder mehrere Deduplizierungsfelder als eindeutige Kennungen, wenn Sie benutzerdefinierte Objektdatensätze erstellen oder aktualisieren. In diesem Beispiel wird das Feld Deduplizierung des benutzerdefinierten **car**-Objekts - VIN (Vehicle ID Number) verwendet. Wenn Sie nur benutzerdefinierte Objektdatensätze aktualisieren, können Sie die [!UICONTROL Marketo-GUID] als [!UICONTROL Deduplizierungsmodus] auswählen.

1. Ordnen Sie jede Spalte einem Marketo-Feld zu, indem Sie sie aus der Dropdown-Liste auswählen.

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >Stellen Sie sicher, dass die Werte in Ihrer Datei mit dem Typ des Felds übereinstimmen, mit dem Sie sie abgleichen (z. B. Text, Ganzzahl usw.), da die Datei andernfalls zurückgewiesen wird.

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/import-custom-object-data-7.png)

1. Klicken Sie **[!UICONTROL Importieren]**.

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >Die Größenbeschränkung für benutzerdefinierte Objekte beträgt 100 MB.

   >[!TIP]
   >
   >Geben Sie in das Feld **[!UICONTROL Warnhinweis senden an]** Ihre E-Mail-Adresse ein. Marketo wird Ihnen eine E-Mail senden, sobald der Import abgeschlossen ist.

1. In der rechten oberen Ecke des Bildschirms wird eine Benachrichtigung angezeigt, während der Import ausgeführt wird, und die endgültigen Ergebnisse werden angezeigt, wenn er abgeschlossen ist.

   ![](assets/import-custom-object-data-9.png)

>[!MORELIKETHIS]
>
>[Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
