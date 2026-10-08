---
unique-page-id: 2360335
description: Blockieren Sie das Überschreiben von Schlüsselfeldern bei Listenimporten aus nicht vertrauenswürdigen Quellen, um vorhandene Daten zu schützen.
title: Blockieren von Feldaktualisierungen während des Listenimports aus nicht vertrauenswürdigen Quellen
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
feature: Field Management
TQID: 'https://experienceleague.adobe.com/cT1pOoWjR-UdHLqNJwhwgR9R12ciIa95q1xHPTf7rBY'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: f5e85a9b-a883-40d0-8759-f3651efb32e9
    internal-label: Field management
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 10%
---
# Blockieren von Feldaktualisierungen während des Listenimports aus nicht vertrauenswürdigen Quellen {#block-field-updates-during-list-import-from-untrusted-sources}

Sie können den Daten in einigen Listen mehr vertrauen als in anderen. Manchmal gibt es fragwürdige Daten, und Sie möchten die Daten akzeptieren, wenn das Feld leer ist, aber nicht, wenn ein Wert vorhanden ist. Sie können dies erreichen, indem Sie Feldaktualisierungen in Schlüsselfeldern blockieren.

>[!NOTE]
>
>**Admin-Berechtigungen erforderlich**

## Blockieren von Feldaktualisierungen aus nicht vertrauenswürdigen Quellen {#blocking-field-updates-from-untrusted-sources}

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. Klicken Sie **[!UICONTROL Feldverwaltung]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. Suchen Sie das gewünschte Feld, wählen Sie es aus und klicken Sie dann unter **[!UICONTROL Feldaktionen]** auf **[!UICONTROL Feldaktualisierungen blockieren]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Markieren Sie **[!UICONTROL Liste nicht vertrauenswürdige Quelle importieren]** und klicken Sie auf **[!UICONTROL Anwenden]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>Sie können Felder vor allen Listen (vertrauenswürdige und nicht vertrauenswürdige) schützen, indem Sie auch die Option **[!UICONTROL Vertrauenswürdige Quelle importieren]** aktivieren.

Wiederholen Sie die obigen Schritte für alle anderen Felder, die Sie vor nicht vertrauenswürdigen Listen schützen möchten.

## Ausführen eines nicht vertrauenswürdigen Listenimports {#running-an-untrusted-list-import}

1. Wählen Sie beim Import Ihrer Liste **[!UICONTROL Nicht vertrauenswürdig]**, wenn alle Felder, die Sie im vorherigen Schritt eingerichtet haben, sicher sein sollen.

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

Detaillierte Anweisungen zum Importieren von Listen finden Sie [Importieren einer Personenliste](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Schlüsselfelder sind jetzt vor nicht vertrauenswürdigen Listenimporten geschützt.
