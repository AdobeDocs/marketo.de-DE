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
>* Die Mitglieder der Marketing-Liste und der Marketing-Liste werden derzeit _nicht unterstützt_.

>[!IMPORTANT]
>
>Der Marketo Sync User benötigt Lesezugriff auf das benutzerdefinierte Objekt, um es aufzulisten und eine Synchronisierung durchzuführen.

1. Wechseln Sie zum Abschnitt **[!UICONTROL Admin]** .

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Wählen Sie **[!UICONTROL Microsoft Dynamics]** und klicken Sie auf **[!UICONTROL Synchronisierung deaktivieren]**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >Sie müssen die globale Synchronisierung vorübergehend deaktivieren, um eine benutzerdefinierte Entität zu aktivieren oder zu deaktivieren.

1. Klicken Sie unter &quot;Datenbankverwaltung&quot;auf **[!UICONTROL Synchronisation von Dynamics-Entitäten]**.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Klicken Sie auf **[!UICONTROL Schema synchronisieren]**.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Wählen Sie die Entität aus, die Sie synchronisieren möchten, und klicken Sie auf **[!UICONTROL Synchronisation aktivieren]**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Wählen Sie die Felder aus, die Sie synchronisieren oder als [Begrenzungen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) und/oder Trigger (für hinzugefügte Datensätze, _nicht_ aktualisiert) in Smart-Listen verwenden möchten. Klicken Sie abschließend auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Während des Synchronisierungsprozesses werden Sie möglicherweise feststellen, dass das Element &quot;[!UICONTROL Dynamische Entitäten synchronisieren]&quot; aus der Navigationsstruktur verschwindet. Dies ist das erwartete Verhalten und wird nach Abschluss der Synchronisierung wieder angezeigt.

1. Die Entität verfügt jetzt über ein grünes Häkchen.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. Vergessen Sie nicht, die globale Synchronisierung erneut zu aktivieren!

   ![](assets/enable-sync-for-a-custom-entity-8.png)
