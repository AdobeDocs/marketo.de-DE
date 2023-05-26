---
unique-page-id: 2360335
description: Feldaktualisierungen beim Listenimport aus nicht vertrauenswürdigen Quellen - Marketo Docs - Produktdokumentation
title: Feldaktualisierungen beim Listenimport aus nicht vertrauenswürdigen Quellen blockieren
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
source-git-commit: 20c41143d1e7839352dddbfea0951c2633987692
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 3%

---

# Feldaktualisierungen beim Listenimport aus nicht vertrauenswürdigen Quellen blockieren {#block-field-updates-during-list-import-from-untrusted-sources}

Sie können den Daten in einigen Listen mehr vertrauen als anderen. Manchmal verfügen Sie über fragwürdige Daten und möchten sie verwenden, wenn das Feld leer ist, jedoch nicht, wenn ein vorhandener Wert vorhanden ist. Sie können dies erreichen, indem Sie Feldaktualisierungen für Schlüsselfelder blockieren.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

## Blockieren von Feldaktualisierungen aus nicht vertrauenswürdigen Quellen {#blocking-field-updates-from-untrusted-sources}

1. Navigieren Sie zum **[!UICONTROL Admin]**-Bereich.

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. Klicken **[!UICONTROL Feldverwaltung]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. Suchen Sie das gewünschte Feld, wählen Sie es aus und klicken Sie dann unter **[!UICONTROL Feldaktionen]** klicken **[!UICONTROL Blockfeldaktualisierungen]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Überprüfen **[!UICONTROL Liste Importieren nicht vertrauenswürdiger Quellen]** und klicken Sie auf **[!UICONTROL Anwenden]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>Sie können Felder in allen Listen sicher halten, vertrauenswürdig und nicht vertrauenswürdig, indem Sie auch die Option **[!UICONTROL Liste Importieren vertrauenswürdiger Quellen]**.

Wiederholen Sie die obigen Schritte für alle anderen Felder, die Sie vor nicht vertrauenswürdigen Listen schützen möchten.

## Ausführen eines nicht vertrauenswürdigen Listenimports {#running-an-untrusted-list-import}

1. Wählen Sie beim Ausführen des Listenimports die Option **[!UICONTROL Nicht vertrauenswürdig]** , wenn alle Felder, die Sie im vorherigen Schritt eingerichtet haben, sicher sein sollen.

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

Detaillierte Anweisungen zum Importieren von Listen finden Sie unter [Eine Personenliste importieren](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Gut gemacht! Jetzt wissen Sie, wie Sie Schlüsselfelder vor nicht vertrauenswürdigen Listen schützen können.
