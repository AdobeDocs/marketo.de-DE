---
unique-page-id: 4719287
description: Erste Feldzuordnungen bearbeiten - Marketing-Dokumente - Produktdokumentation
title: Zuordnungen von Anfangsfeldern bearbeiten
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Zuordnungen von Anfangsfeldern bearbeiten {#edit-initial-field-mappings}

>[!NOTE]
>
>**Erinnerung**
>
>Diese Funktion steht erst vor der ersten Synchronisierung mit Salesforce zur Verfügung! Wenn die Schaltfläche Jetzt **synchronisieren** gedrückt wird, kann dies nicht mehr durchgeführt werden.

Während der anfänglichen Synchronisierung mit Salesforce kombiniert Marketo automatisch gleichnamige benutzerdefinierte Felder in einem Feld auf der Marketo-Seite, um sicherzustellen, dass die Daten mit Lead- und Kontaktobjekten im CRM ausgetauscht werden können. In diesem Artikel wird beschrieben, wie Sie diese Zuordnungen anpassen.

## Nicht zugeordnete Felder zuordnen {#map-unmapped-fields}

Wenn ein Feld im Ordner &quot;Nicht zugeordnete Felder&quot;angezeigt wird, bedeutet dies, dass es keinem ähnlichen Feld im Feld &quot;Interessent&quot;oder &quot;Kontakt&quot;in Salesforce zugeordnet ist. Du kannst das reparieren.

1. Klicken Sie auf Zuordnungen bearbeiten.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. Öffnen Sie den Ordner &quot; **Nicht zugeordnete benutzerdefinierte Felder** &quot;.

   ![](assets/two.png)

1. Ziehen Sie ein nicht zugewiesenes benutzerdefiniertes Feld auf ein anderes, um es miteinander zu verknüpfen.

   >[!NOTE]
   >
   >Sie können nur benutzerdefinierte Feldzuordnungen bearbeiten. Standardfeldzuordnungen können nicht geändert werden.

   ![](assets/three.png)

1. Klicken Sie auf **Zuordnungen** beenden, wenn Sie fertig sind.

   ![](assets/four.png)

## Vorhandene Zuordnung umbrechen {#break-existing-mapping}

Wenn Sie gleichnamige Felder auf dem Interessenten- und Kontaktobjekt haben, werden sie von Marketo automatisch zugeordnet. Sie können davon ausgehen, dass sie unterschiedlich sind und unterschiedliche Daten enthalten. Unterbrechen Sie die Zuordnung so.

1. Klicken Sie auf Zuordnungen **bearbeiten**.

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. Markieren Sie ein zugewiesenes Feld und klicken Sie auf **Zuordnung** umbrechen, um die Felder zu trennen.

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. Klicken Sie auf **Zuordnungen** beenden, wenn Sie fertig sind.

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   Schön! Sie sind fast mit der anfänglichen Synchronisierung fertig.

## Schema zurücksetzen {#reset-schema}

1. Wenn Sie beim Bearbeiten der Zuordnungen Änderungen am Schema in Salesforce vornehmen, können Sie die Änderungen durch Klicken auf Schema **zurücksetzen** ziehen.

   * Alle Zuordnungsänderungen werden zurückgesetzt!
   * Durch Zurücksetzen des Schemas werden nur Felder hinzugefügt, nicht jedoch entfernt (auch wenn Sie sie vom Synchronisierungsbenutzer ausblenden).

   ![](assets/image2014-12-9-13-3a32-3a8.png)

