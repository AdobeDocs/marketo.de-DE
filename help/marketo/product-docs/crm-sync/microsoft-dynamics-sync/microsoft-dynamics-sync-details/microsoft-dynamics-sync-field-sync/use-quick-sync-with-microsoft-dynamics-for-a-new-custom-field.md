---
unique-page-id: 10098379
description: Verwenden der Schnellsynchronisierung mit Microsoft Dynamics für ein neues benutzerdefiniertes Feld - Marketo-Dokumente - Produktdokumentation
title: Verwenden der Schnellsynchronisierung mit Microsoft Dynamics für ein neues benutzerdefiniertes Feld
exl-id: c98f1443-c0dd-40e1-919b-f8110088b38a
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 1%

---

# Schnellsynchronisierung mit [!DNL Microsoft Dynamics] für ein neues benutzerdefiniertes Feld verwenden {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

Marketing oder Vertrieb möchten ein neues Feld. Oder vielleicht haben Sie einen in Ihrer ursprünglichen Feldauswahl vergessen. Oder Ihre Anforderungen haben sich geändert. In jedem Fall können Sie die Schnellsynchronisierung verwenden, um bestimmte Felder neu zu synchronisieren.

Normalerweise verwenden Sie die Schnellsynchronisierung, um ein neues Feld hinzuzufügen und Werte zu aktualisieren. Es gibt jedoch Fälle, in denen Sie ein vorhandenes Feld synchronisieren möchten. Sie können die Feldsynchronisierung auf der Grundlage eines aktualisierten oder erstellten Datumsbereichs einschränken. Weitere Informationen finden [ unter ](#Advanced_Sync_Options) Synchronisierungsoptionen.

Die Schnellsynchronisierung kann Nullwerte synchronisieren. Wenn Sie beispielsweise die Werte A und B verwenden und einen B-Wert in [!DNL Dynamics] auf null ändern, wird der Null-Wert mit Marketo synchronisiert.

## Schnellsynchronisierung für alle Datensätze {#quick-sync-for-all-records}

So synchronisieren Sie mit der Schnellsynchronisierung nach neuen Feldern neu.

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**.

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. Auf **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. Klicken Sie [!UICONTROL &#x200B; „Details zur &#x200B;]&quot; auf **[!UICONTROL Bearbeiten]**.

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. Wählen Sie die Felder für die Schnellsynchronisierung aus und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-15-3a26-3a11.png)

   >[!NOTE]
   >
   >Sie können Felder aus mehreren Entitäten auswählen.

1. Sie erhalten eine Benachrichtigung, sobald die Synchronisierung abgeschlossen ist.

   ![](assets/field-sync-update-notification.png)

   >[!CAUTION]
   >
   >Die Synchronisierung wird Seite an Seite mit anderen Synchronisierungen ausgeführt und kann je nach Größe der Datenbank lange dauern. Wenn sich ein Feld in einer Warteschlange für die Synchronisierung befindet, können Sie die Auswahl nicht aufheben.

## Erweiterte Synchronisierungsoptionen {#advanced-sync-options}

Was passiert, wenn Sie ein vorhandenes Feld synchronisieren möchten, dies aber nur für einen begrenzten Datensatz tun? So geht&#39;s.

1. Deaktivieren Sie das Kontrollkästchen für ein vorhandenes Feld. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. Öffnen Sie das Popup erneut und wählen Sie das Feld erneut aus.

   ![](assets/select-field-reselect-hand.png)

1. Klicken Sie **[!UICONTROL Erweiterte Synchronisierung]**.

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. Wählen Sie **[!UICONTROL Aktualisiert]** und wählen Sie mithilfe der Datumsauswahl einen Datumsbereich aus. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   Nur Datensätze, die zwischen 8/19/16 und 9/19/16 aktualisiert wurden, werden für das Feld schnell synchronisiert.

## Beheben von nicht synchronisierten Feldern {#fixing-out-of-sync-fields}

In den seltenen Fällen, in denen ein [!DNL Dynamics]- und ein Marketo-Feld nicht synchron sind, gibt es eine schnelle und einfache Möglichkeit, sie erneut zu synchronisieren.

1. Deaktivieren Sie das Feld und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. Markieren Sie das Feld erneut und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   Das sollte es richten!
