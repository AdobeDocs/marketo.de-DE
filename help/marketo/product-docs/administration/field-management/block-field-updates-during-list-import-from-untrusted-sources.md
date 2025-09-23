---
unique-page-id: 2360335
description: Blockieren von Feldaktualisierungen während des Listenimports aus nicht vertrauenswürdigen Quellen - Marketo-Dokumente - Produktdokumentation
title: Blockieren von Feldaktualisierungen während des Listenimports aus nicht vertrauenswürdigen Quellen
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 9%

---

# Blockieren von Feldaktualisierungen während des Listenimports aus nicht vertrauenswürdigen Quellen {#block-field-updates-during-list-import-from-untrusted-sources}

Sie können den Daten in einigen Listen mehr vertrauen als in anderen. Manchmal sind die Daten fragwürdig und das Feld sollte leer sein, aber nicht, wenn bereits ein Wert vorhanden ist. Sie können dies erreichen, indem Sie Feldaktualisierungen in Schlüsselfeldern blockieren.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

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

Gut gemacht! Jetzt wissen Sie, wie Sie Schlüsselfelder vor nicht vertrauenswürdigen Listen schützen können.
