---
unique-page-id: 4719287
description: Bearbeiten von anfänglichen Feldzuordnungen - Marketo-Dokumente - Produktdokumentation
title: anfängliche Feldzuordnungen bearbeiten
exl-id: 320613d1-3845-4e05-a704-0db0f8027dc8
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# anfängliche Feldzuordnungen bearbeiten {#edit-initial-field-mappings}

>[!NOTE]
>
>Auf diese Funktion kann nur vor der ersten Synchronisierung mit Salesforce zugegriffen werden. Einmal die **[!UICONTROL Jetzt synchronisieren]** -Taste gedrückt wird, kann dies nicht mehr durchgeführt werden.

Bei der ersten Synchronisation mit Salesforce kombiniert Marketo Engage automatisch ähnlich benannte benutzerdefinierte Felder in einem Feld auf der Marketo-Seite, um sicherzustellen, dass die Daten mit Lead- und Kontaktobjekten im CRM ausgetauscht werden können. In diesem Artikel wird erläutert, wie Sie diese Zuordnungen anpassen können.

## Nicht zugeordnete Felder zuordnen {#map-unmapped-fields}

Wenn ein Feld im [!UICONTROL Nicht zugeordnete Felder] -Ordner, bedeutet dies, dass er keinem ähnlichen Feld auf dem Lead oder Kontakt in Salesforce zugeordnet ist. Du kannst das reparieren.

1. Klicks **[!UICONTROL Zuordnungen bearbeiten]**.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. Öffnen Sie die **[!UICONTROL Nicht zugeordnete benutzerdefinierte Felder]** Ordner.

   ![](assets/two.png)

1. Ziehen Sie ein nicht zugewiesenes benutzerdefiniertes Feld auf ein anderes, um es einander zuzuordnen.

   >[!NOTE]
   >
   >Sie können nur benutzerdefinierte Feldzuordnungen bearbeiten. Standardfeldzuordnungen können nicht geändert werden.

   ![](assets/three.png)

1. Klicks **[!UICONTROL Abschließen von Zuordnungen]** wenn Sie fertig sind.

   ![](assets/four.png)

## Vorhandene Zuordnung unterbrechen {#break-existing-mapping}

Wenn Sie ähnlich benannte Felder auf dem Lead und Kontaktobjekt haben, ordnet Marketo sie automatisch zu. Sie können davon ausgehen, dass sie unterschiedlich sind und unterschiedliche Daten enthalten. Brechen Sie die Zuordnung wie folgt ab.

1. Klicks **[!UICONTROL Zuordnungen bearbeiten]**.

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. Markieren Sie ein zugeordnetes Feld und klicken Sie auf **[!UICONTROL Break Mapping]** , um die Felder zu trennen.

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. Klicks **[!UICONTROL Abschließen von Zuordnungen]** wenn Sie fertig sind.

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   Gut! Sie sind fast mit der ersten Synchronisierung fertig.

## Schema zurücksetzen {#reset-schema}

1. Wenn Sie beim Bearbeiten der Zuordnungen Änderungen am Schema in Salesforce vornehmen, können Sie die Änderungen abrufen, indem Sie auf **[!UICONTROL Schema zurücksetzen]**.

   * Alle Änderungen der Zuordnung werden zurückgesetzt!
   * Durch das Zurücksetzen des Schemas werden nur Felder hinzugefügt, nicht entfernt (auch wenn Sie sie für den Synchronisierungsbenutzer ausblenden).

   ![](assets/image2014-12-9-13-3a32-3a8.png)
