---
unique-page-id: 2953384
description: Aktivieren der Synchronisierung für eine benutzerdefinierte Entität - Marketo Docs - Produktdokumentation
title: Aktivieren der Synchronisierung für eine benutzerdefinierte Entität
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
translation-type: tm+mt
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# Aktivieren der Synchronisierung für eine benutzerdefinierte Entität {#enable-sync-for-a-custom-entity}

Wenn Sie benutzerdefinierte Entitätsdaten von Dynamics benötigen, um in Marketo verfügbar zu sein, können Sie die Synchronisierung aktivieren:

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!NOTE]
>
>Wenn Sie die Synchronisierung für eine benutzerdefinierte Entität aktivieren, führt Marketo eine anfängliche Synchronisierung durch, um alle Daten für das benutzerdefinierte Objekt einzubringen.

1. Gehen Sie zum Abschnitt **Admin**.

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. Wählen Sie **Microsoft Dynamics** und klicken Sie auf **Synchronisierung deaktivieren**.

   Sie müssen die globale Synchronisierung vorübergehend deaktivieren, um eine benutzerdefinierte Entität zu aktivieren oder zu deaktivieren.

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. Klicken Sie unter &quot;Datenbankverwaltung&quot;auf den Link **Dynamics Entities Sync**.

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. Klicken Sie auf den Link **Schema synchronisieren**.

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. Wählen Sie die Entität aus, die Sie synchronisieren möchten, und klicken Sie auf **Synchronisierung aktivieren**.

   ![](assets/image2015-11-10-9-3a44-3a35.png)

1. Wählen Sie die zu synchronisierenden oder als [constraints](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) und/oder Trigger in intelligenten Listen zu verwendenden Felder aus. Klicken Sie abschließend auf **Synchronisierung aktivieren**.

   ![](assets/image2014-10-20-14-3a32-3a55.png)

   >[!NOTE]
   >
   >Während des Synchronisierungsprozesses wird möglicherweise festgestellt, dass das Element &quot;Dynamische Entitäten synchronisieren&quot;aus der Navigationsstruktur verschwindet. Dieses Verhalten wird erwartet und nach Abschluss der Synchronisierung erneut angezeigt.

1. Die Entität hat jetzt ein grünes Häkchen darauf.

   ![](assets/image2014-10-20-14-3a33-3a4.png)

1. Vergessen Sie nicht, die globale Synchronisierung erneut zu aktivieren!

   ![](assets/image2015-11-10-9-3a48-3a35.png)

Oh ja! Leistungsstarkes Zeug.
