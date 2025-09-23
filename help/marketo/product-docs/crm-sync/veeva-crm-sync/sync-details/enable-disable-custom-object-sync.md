---
description: Aktivieren/Deaktivieren der Synchronisierung benutzerdefinierter Objekte - Marketo-Dokumente - Produktdokumentation
title: Aktivieren/Deaktivieren der benutzerdefinierten Objektsynchronisierung
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
feature: Veeva CRM
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 4%

---

# Aktivieren/Deaktivieren der benutzerdefinierten Objektsynchronisierung {#enable-disable-custom-object-sync}

Benutzerdefinierte Objekte, die in Ihrer [!DNL Veeva] CRM-Instanz erstellt wurden, können auch Teil von Marketo Engage sein. Gehen Sie wie folgt vor, um sie einzurichten.

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

Wählen Sie das zu synchronisierende Objekt aus und klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

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

Ausgezeichnet! Sie können jetzt die Daten dieses benutzerdefinierten Objekts in „Smart[!UICONTROL Kampagnen“ &#x200B;] „Smart[!UICONTROL Listen“ &#x200B;].

>[!MORELIKETHIS]
>
>[Benutzerdefiniertes Objektfeld als Smart-Listen-/Trigger-Einschränkungen hinzufügen/entfernen](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
