---
unique-page-id: 2953384
description: Aktivieren der Synchronisierung für eine benutzerdefinierte Entität - Marketo-Dokumente - Produktdokumentation
title: Aktivieren der Synchronisierung für eine benutzerdefinierte Entität
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
source-git-commit: 79cfb0396f690a370cdce4e4df3a23c7439c252e
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# Aktivieren der Synchronisierung für eine benutzerdefinierte Entität {#enable-sync-for-a-custom-entity}

Wenn Sie benutzerdefinierte Entitätsdaten aus Dynamics benötigen, um in Marketo verfügbar zu sein, können Sie hier die Synchronisierung aktivieren.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!NOTE]
>
>* Wenn Sie die Synchronisierung für eine benutzerdefinierte Entität aktivieren, führt Marketo eine erste Synchronisierung durch, um alle Daten für das benutzerdefinierte Objekt einzubringen.
>* Mitglieder der Marketing-Liste und der Marketing-Liste sind **nicht unterstützt** zu diesem Zeitpunkt.


>[!IMPORTANT]
>
>Der Marketo Sync User benötigt Lesezugriff auf das benutzerdefinierte Objekt, um es aufzulisten und eine Synchronisierung durchzuführen.

1. Navigieren Sie zu **Admin** Abschnitt.

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Auswählen **Microsoft Dynamics** und klicken Sie auf **Synchronisierung deaktivieren**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >Sie müssen die globale Synchronisierung vorübergehend deaktivieren, um eine benutzerdefinierte Entität zu aktivieren oder zu deaktivieren.

1. Klicken Sie unter &quot;Datenbankverwaltung&quot;auf die **Synchronisation von Dynamics-Entitäten** Link.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Klicken Sie auf **Schema synchronisieren** Link.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Wählen Sie die Entität aus, die Sie synchronisieren möchten, und klicken Sie auf **Synchronisierung aktivieren**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Wählen Sie die Felder aus, die Sie synchronisieren oder als [Einschränkungen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) und/oder Trigger in Smart-Listen. Wenn Sie fertig sind, klicken Sie auf **Synchronisierung aktivieren**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Während des Synchronisierungsprozesses wird möglicherweise festgestellt, dass das Element &quot;Synchronisierung dynamischer Entitäten&quot;aus der Navigationsstruktur verschwindet. Dies ist das erwartete Verhalten und wird nach Abschluss der Synchronisierung wieder angezeigt.

1. Die Entität enthält jetzt ein grünes Häkchen.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. Vergessen Sie nicht, die globale Synchronisierung erneut zu aktivieren!

   ![](assets/enable-sync-for-a-custom-entity-8.png)
