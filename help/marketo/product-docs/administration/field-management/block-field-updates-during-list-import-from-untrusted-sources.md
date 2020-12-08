---
unique-page-id: 2360335
description: Feldaktualisierungen während des Listen-Imports aus nicht vertrauenswürdigen Quellen - Marketing to Docs - Produktdokumentation blockieren
title: Feldaktualisierungen während des Listen-Imports aus nicht vertrauenswürdigen Quellen blockieren
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---


# Feldaktualisierungen während des Listen-Imports aus nicht vertrauenswürdigen Quellen blockieren {#block-field-updates-during-list-import-from-untrusted-sources}

Sie können den Daten in einigen Listen mehr vertrauen als in anderen. Manchmal verfügen Sie über fragwürdige Daten und möchten diese bei leerem Feld verwenden, nicht jedoch bei vorhandenem Wert. Dies können Sie erreichen, indem Sie Feldaktualisierungen in Schlüsselfeldern blockieren.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Blockieren von Feldaktualisierungen aus nicht vertrauenswürdigen Quellen {#blocking-field-updates-from-untrusted-sources}

1. Gehen Sie zu **Admin** und klicken Sie auf **Feldverwaltung**.

   ![](assets/image2014-9-19-9-3a38-3a38.png)

1. Suchen Sie das gewünschte Feld, wählen Sie es aus und klicken Sie dann unter **Feldaktionen** auf Feldaktualisierungen **blockieren**.

   ![](assets/image2014-9-19-9-3a39-3a40.png)

1. Markieren Sie **Liste Nicht vertrauenswürdige Quelle** importieren und klicken Sie auf **Übernehmen**.

   ![](assets/blockupdates.png)

>[!TIP]
>
>Sie können die Felder vor allen Listen schützen (vertrauenswürdig und nicht vertrauenswürdig), indem Sie auch die Option **Liste Importieren vertrauenswürdiger Quelle** aktivieren.

Wiederholen Sie diese Schritte für alle anderen Felder, die vor nicht vertrauenswürdigen Listen geschützt sein sollen.

## Ausführen eines Imports nicht vertrauenswürdiger Listen {#running-an-untrusted-list-import}

1. Wählen Sie beim Ausführen des Listen-Imports **Nicht vertrauenswürdig **aus, wenn alle im vorherigen Schritt eingerichteten Felder sicher sein sollen.

   ![](assets/importpersondetails.jpg)

Detaillierte Anweisungen zum Importieren von Listen finden Sie unter Liste von Personen [importieren](../../../getting-started/quick-wins/import-a-list-of-people.md).

Gute Arbeit! Jetzt wissen Sie, wie Sie Schlüsselfelder vor nicht vertrauenswürdigen Listen schützen können.
