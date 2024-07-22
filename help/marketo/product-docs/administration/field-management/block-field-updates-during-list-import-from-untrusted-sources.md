---
unique-page-id: 2360335
description: Feldaktualisierungen beim Listenimport aus nicht vertrauenswürdigen Quellen - Marketo Docs - Produktdokumentation
title: Feldaktualisierungen beim Listenimport aus nicht vertrauenswürdigen Quellen blockieren
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Feldaktualisierungen beim Listenimport aus nicht vertrauenswürdigen Quellen blockieren {#block-field-updates-during-list-import-from-untrusted-sources}

Sie können den Daten in einigen Listen mehr vertrauen als anderen. Manchmal verfügen Sie über fragwürdige Daten und möchten sie verwenden, wenn das Feld leer ist, jedoch nicht, wenn ein vorhandener Wert vorhanden ist. Sie können dies erreichen, indem Sie Feldaktualisierungen für Schlüsselfelder blockieren.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

## Blockieren von Feldaktualisierungen aus nicht vertrauenswürdigen Quellen {#blocking-field-updates-from-untrusted-sources}

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. Klicken Sie auf **[!UICONTROL Feldverwaltung]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. Suchen Sie das gewünschte Feld, wählen Sie es aus und klicken Sie dann unter **[!UICONTROL Feldaktionen]** auf **[!UICONTROL Feldaktualisierungen blockieren]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Aktivieren Sie die Option **[!UICONTROL Liste Importieren nicht vertrauenswürdiger Quellen]** und klicken Sie auf **[!UICONTROL Anwenden]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>Sie können Felder in allen Listen sicher halten, vertrauenswürdig und nicht vertrauenswürdig, indem Sie auch die Option **[!UICONTROL Liste Importieren vertrauenswürdiger Quellen]** aktivieren.

Wiederholen Sie die obigen Schritte für alle anderen Felder, die Sie vor nicht vertrauenswürdigen Listen schützen möchten.

## Ausführen eines nicht vertrauenswürdigen Listenimports {#running-an-untrusted-list-import}

1. Wählen Sie beim Ausführen des Listenimports **[!UICONTROL Nicht vertrauenswürdig]** aus, wenn alle Felder, die Sie im vorherigen Schritt eingerichtet haben, sicher sein sollen.

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

Detaillierte Anweisungen zum Importieren von Listen finden Sie unter [Importieren einer Personenliste](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Gut gemacht! Jetzt wissen Sie, wie Sie Schlüsselfelder vor nicht vertrauenswürdigen Listen schützen können.
