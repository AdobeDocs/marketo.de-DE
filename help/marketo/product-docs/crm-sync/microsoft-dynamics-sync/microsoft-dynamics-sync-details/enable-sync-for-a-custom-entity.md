---
unique-page-id: 2953384
description: Aktivieren der Synchronisierung für eine benutzerdefinierte Entität - Marketo-Dokumente - Produktdokumentation
title: Aktivieren der Synchronisierung für eine benutzerdefinierte Entität
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
feature: Microsoft Dynamics
source-git-commit: d522950af40c5e3e702a6522101ebe9550432be5
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Aktivieren der Synchronisierung für eine benutzerdefinierte Entität {#enable-sync-for-a-custom-entity}

Wenn Sie benutzerdefinierte Entitätsdaten aus Dynamics benötigen, um auf Marketo Engage verfügbar zu sein, finden Sie hier eine Möglichkeit, die Synchronisierung dafür zu aktivieren.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!NOTE]
>
>* Wenn Sie die Synchronisierung für eine benutzerdefinierte Entität aktivieren, führt Marketo eine erste Synchronisierung durch, um alle Daten für das benutzerdefinierte Objekt einzubringen.
>* Mitglieder der Marketingliste und der Marketingliste sind _nicht unterstützt_ zu diesem Zeitpunkt.

>[!IMPORTANT]
>
>Der Marketo Sync User benötigt Lesezugriff auf das benutzerdefinierte Objekt, um es aufzulisten und eine Synchronisierung durchzuführen.

1. Navigieren Sie zu **[!UICONTROL Admin]** Abschnitt.

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Auswählen **[!UICONTROL Microsoft Dynamics]** und klicken **[!UICONTROL Synchronisierung deaktivieren]**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >Sie müssen die globale Synchronisierung vorübergehend deaktivieren, um eine benutzerdefinierte Entität zu aktivieren oder zu deaktivieren.

1. Klicken Sie unter Datenbankverwaltung auf **[!UICONTROL Synchronisation von Dynamics-Entitäten]**.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Klicks **[!UICONTROL Schema synchronisieren]**.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Wählen Sie die zu synchronisierende Entität aus und klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Wählen Sie die Felder aus, die Sie synchronisieren oder als [Einschränkungen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) und/oder Trigger (für hinzugefügte Datensätze), _not_ aktualisiert) in Smart-Listen. Klicken Sie abschließend auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Während des Synchronisierungsprozesses wird möglicherweise Folgendes angezeigt:[!UICONTROL Synchronisierung dynamischer Entitäten]&quot; aus der Navigationsstruktur verschwindet. Dies ist das erwartete Verhalten und wird nach Abschluss der Synchronisierung wieder angezeigt.

1. Die Entität verfügt jetzt über ein grünes Häkchen.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. Vergessen Sie nicht, die globale Synchronisierung erneut zu aktivieren!

   ![](assets/enable-sync-for-a-custom-entity-8.png)
