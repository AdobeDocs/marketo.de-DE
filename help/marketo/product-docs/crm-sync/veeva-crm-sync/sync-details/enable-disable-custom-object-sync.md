---
description: Erfahren Sie, wie Sie die Synchronisierung benutzerdefinierter Objekte zwischen Veeva CRM und Marketo Engage aktivieren oder deaktivieren. Verwenden Sie Admin- und Veeva-Synchronisierungsobjekte, um benutzerdefinierte Objekte auszuwählen und zu synchronisieren.
title: Aktivieren/Deaktivieren der benutzerdefinierten Objektsynchronisierung
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
feature: Veeva CRM
TQID: 'https://experienceleague.adobe.com/nsmRk-zf-I5r0hfLxsOnGsTf66X-bYZ7OAUXHrPc-t0'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
    internal-label: Implementation
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
    internal-label: Smart lists
  - id: f141b8e0-5812-4581-b47d-7322a93e7f28
    internal-label: Veeva CRM
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 4%
---
# Aktivieren/Deaktivieren der benutzerdefinierten Objektsynchronisierung {#enable-disable-custom-object-sync}

Benutzerdefinierte Objekte, die in Ihrer [!DNL Veeva] CRM-Instanz erstellt wurden, können auch Teil von Marketo Engage sein. So richten Sie es ein.

## Aktivieren oder Deaktivieren der Synchronisierung benutzerdefinierter Objekte {#enable-or-disable-the-custom-object-sync}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]** und dann auf **[!UICONTROL Veeva Objects Sync]**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. Wenn dies das erste benutzerdefinierte Objekt ist, klicken Sie auf **[!UICONTROL Schema synchronisieren]**. Klicken Sie andernfalls auf **[!UICONTROL Schema aktualisieren]**, um sicherzustellen, dass Sie über die neueste Version verfügen.

   ![](assets/enable-disable-custom-object-sync-2.png)

1. Wenn die globale Synchronisierung ausgeführt wird, deaktivieren Sie sie, indem Sie auf **[!UICONTROL Globale Synchronisierung deaktivieren]** klicken.

   ![](assets/enable-disable-custom-object-sync-3.png)

   >[!NOTE]
   >
   >Eine Synchronisierung des [!DNL Veeva] benutzerdefinierten Objektschemas kann einige Minuten dauern.

1. Klicken Sie **[!UICONTROL Schema aktualisieren]**.

   ![](assets/enable-disable-custom-object-sync-4.png)

1. Wählen Sie das zu synchronisierende Objekt aus und klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/enable-disable-custom-object-sync-5.png)

   >[!TIP]
   >
   >Marketo kann ein benutzerdefiniertes Objekt nur synchronisieren, wenn es eine direkte Beziehung mit dem Kontakt- oder Kontoobjekt in [!DNL Veeva] CRM hat.

1. Klicken Sie erneut **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/enable-disable-custom-object-sync-6.png)

1. Wechseln Sie zurück zur Registerkarte [!UICONTROL Veeva] und klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/enable-disable-custom-object-sync-7.png)

## Verwenden benutzerdefinierter Objekte {#using-your-custom-objects}

>[!NOTE]
>
>Benutzerdefinierte Objekte können nicht in Smart-Kampagnen mit Triggern verwendet werden.

1. Ziehen Sie in [!UICONTROL Smart List] den Filter &quot;**[!UICONTROL Hat Opportunity]** auf und setzen Sie ihn auf **[!UICONTROL True]**.

   ![](assets/enable-disable-custom-object-sync-8.png)

1. Verwenden Sie optional Filtereinschränkungen, um den Fokus einzugrenzen.

   ![](assets/enable-disable-custom-object-sync-9.png)

Sie können jetzt die Daten dieses benutzerdefinierten Objekts in [!UICONTROL Smart-Kampagnen] und [!UICONTROL Smart-Listen] verwenden.

>[!MORELIKETHIS]
>
>[Benutzerdefiniertes Objektfeld als Smart-Listen-/Trigger-Einschränkungen hinzufügen/entfernen](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
