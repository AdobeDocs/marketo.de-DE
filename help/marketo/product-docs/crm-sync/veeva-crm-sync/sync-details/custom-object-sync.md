---
description: Erfahren Sie, wie Sie die Synchronisierung benutzerdefinierter Objekte von Veeva CRM mit Marketo Engage einrichten. Aktivieren Sie benutzerdefinierte Objekte in Admin und verwenden Sie sie in Smart-Listen und Triggern.
title: Synchronisierung benutzerdefinierte Objekte
hide: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
feature: Veeva CRM
TQID: https://experienceleague.adobe.com/RmyCIMm3TKbcO3nPcqyZqbWZl1dnJ6Au4HsuURJjcKU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 217
ht-degree: 2%

---

# Synchronisierung benutzerdefinierte Objekte {#custom-object-sync}

Benutzerdefinierte Objekte, die in Ihrer [!DNL Veeva] CRM-Instanz erstellt wurden, können auch Teil von Marketo Engage sein. So richten Sie es ein.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!PREREQUISITES]
>
>Um ein benutzerdefiniertes Objekt zu verwenden, muss es mit einem Kontakt- oder Kontoobjekt in [!DNL Veeva] CRM verknüpft sein.

## Benutzerdefiniertes Objekt aktivieren {#enable-custom-object}

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]** und dann auf **[!UICONTROL Veeva Objects Sync]**.

   ![](assets/custom-object-sync-1.png)

1. Wenn dies das erste benutzerdefinierte Objekt ist, klicken Sie auf **[!UICONTROL Schema synchronisieren]**.

   ![](assets/custom-object-sync-2.png)

1. Klicken Sie **[!UICONTROL Globale Synchronisierung deaktivieren]**.

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >Die Erstsynchronisierung des [!DNL Veeva] benutzerdefinierten Objektschemas kann einige Minuten dauern.

1. Ziehen Sie das benutzerdefinierte Objekt, das Sie synchronisieren möchten, auf die Arbeitsfläche.

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >Benutzerdefinierte Objekte müssen eindeutige Namen haben. Marketo unterstützt nicht zwei verschiedene benutzerdefinierte Objekte mit demselben Namen.

1. Klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/custom-object-sync-5.png)

1. Klicken Sie erneut **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/custom-object-sync-6.png)

1. Kehren Sie zur Registerkarte &quot;**[!UICONTROL &quot;]**.

   ![](assets/custom-object-sync-7.png)

1. Klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/custom-object-sync-8.png)

1. Um alle Ihre [!DNL Veeva] benutzerdefinierten Objekte anzuzeigen, klicken Sie auf **[!UICONTROL Admin]** und **[!UICONTROL Veeva-]**.

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo unterstützt nur benutzerdefinierte Entitäten, die mit Standardelementen verknüpft sind, die eine bis zwei Ebenen tief sind.

Ausgezeichnet! Sie können jetzt Daten aus diesem benutzerdefinierten Objekt in Smart-Kampagnen und Smart-Listen verwenden.

>[!MORELIKETHIS]
>
>* [Meldungen zu Aufrufen und Aufrufen synchronisieren](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
>* [Benutzerdefiniertes Objektfeld als Smart-Listen-/Trigger-Einschränkungen hinzufügen/entfernen](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
