---
unique-page-id: 10098379
description: Verwenden Sie die Schnellsynchronisierung mit Microsoft Dynamics für ein neues benutzerdefiniertes Feld - Marketo Docs - Produktdokumentation
title: Verwenden der Schnellsynchronisierung mit Microsoft Dynamics für ein neues benutzerdefiniertes Feld
exl-id: c98f1443-c0dd-40e1-919b-f8110088b38a
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 1%

---

# Verwenden der Schnellsynchronisierung mit Microsoft Dynamics für ein neues benutzerdefiniertes Feld {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

Marketing oder Vertrieb möchten ein neues Feld erstellen. Oder vielleicht haben Sie eines in Ihrer ersten Feldauswahl vergessen. Oder Ihre Bedürfnisse haben sich geändert. In jedem Fall können Sie die Schnellsynchronisierung verwenden, um bestimmte Felder neu zu synchronisieren.

Normalerweise verwenden Sie die Schnellsynchronisierung, um ein neues Feld hinzuzufügen und die Werte zu aktualisieren. Es gibt jedoch Fälle, in denen Sie möglicherweise ein vorhandenes Feld synchronisieren möchten. Sie können die Feldsynchronisierung anhand eines aktualisierten oder erstellten Datumsbereichs einschränken. Weitere Informationen finden Sie unten unter [Erweiterte Synchronisierungsoptionen](#Advanced_Sync_Options) .

Die Schnellsynchronisierung kann Null-Werte synchronisieren. Wenn Sie beispielsweise die Werte A und B verwenden und einen B-Wert in Dynamics auf null ändern, wird der Nullwert mit Marketo synchronisiert.

## Schnellsynchronisierung für alle Datensätze {#quick-sync-for-all-records}

Hier erfahren Sie, wie Sie die Schnellsynchronisierung verwenden, um für neue Felder neu zu synchronisieren.

1. Klicken Sie unter Marketo Engage auf **[!UICONTROL Admin]**.

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. Klicken Sie auf **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. Klicken Sie in den Details zur Feldsynchronisierung auf **[!UICONTROL Bearbeiten]**.

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. Wählen Sie die Felder aus, die schnell synchronisiert werden sollen, und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-15-3a26-3a11.png)

   >[!NOTE]
   >
   >Sie können Felder aus mehreren Entitäten auswählen.

1. Sie erhalten eine Benachrichtigung, wenn die Synchronisation abgeschlossen ist.

   ![](assets/field-sync-update-notification.png)

   >[!CAUTION]
   >
   >Die Synchronisierung wird parallel mit anderen Synchronisierungen ausgeführt. Je nach Größe der Datenbank kann es lange dauern, bis sie abgeschlossen ist. Wenn sich ein Feld in einer Warteschlange zur Synchronisierung befindet, können Sie die Auswahl nicht aufheben.

## Erweiterte Synchronisierungsoptionen {#advanced-sync-options}

Was passiert, wenn Sie ein vorhandenes Feld synchronisieren möchten, dies aber nur für einen begrenzten Datensatz tun? So geht es.

1. Deaktivieren Sie das Kontrollkästchen für ein vorhandenes Feld. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. Öffnen Sie das Popup erneut und wählen Sie das Feld erneut aus.

   ![](assets/select-field-reselect-hand.png)

1. Klicken Sie auf **[!UICONTROL Erweiterte Synchronisation]**.

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. Wählen Sie **[!UICONTROL Aktualisiert]** und wählen Sie mithilfe der Datumsauswahl einen Datumsbereich aus. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   Nur Datensätze, die zwischen dem 19.08.2016 und dem 19.09.2016 aktualisiert wurden, werden für das Feld schnell synchronisiert.

## Beheben von nicht synchronisierten Feldern {#fixing-out-of-sync-fields}

In seltenen Fällen, in denen ein Dynamics- und Marketo-Feld nicht synchron ist, gibt es eine schnelle und einfache Möglichkeit, sie neu zu synchronisieren.

1. Heben Sie die Auswahl des Felds auf und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. Wählen Sie das Feld erneut aus und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   Das sollte es reparieren!
