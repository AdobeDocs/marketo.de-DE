---
description: Aktivieren/Deaktivieren der Synchronisierung benutzerdefinierter Objekte - Marketo-Dokumente - Produktdokumentation
title: Benutzerdefinierte Objektsynchronisierung aktivieren/deaktivieren
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
feature: Veeva CRM
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Benutzerdefinierte Objektsynchronisierung aktivieren/deaktivieren {#enable-disable-custom-object-sync}

Benutzerdefinierte Objekte, die in Ihrer Veeva CRM-Instanz erstellt wurden, können auch Teil von Marketo Engage sein. So richten Sie es ein.

## Aktivieren oder Deaktivieren der Synchronisierung benutzerdefinierter Objekte {#enable-or-disable-the-custom-object-sync}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]** und dann auf **[!UICONTROL Veeva Objects Sync]**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. Wenn dies Ihr erstes benutzerdefiniertes Objekt ist, klicken Sie auf Schema synchronisieren. Klicken Sie andernfalls auf **[!UICONTROL Schema aktualisieren]**, um sicherzustellen, dass Sie über die neueste Version verfügen.

   ![](assets/enable-disable-custom-object-sync-2.png)

1. Wenn die globale Synchronisierung ausgeführt wird, deaktivieren Sie sie, indem Sie auf **[!UICONTROL Globale Synchronisierung deaktivieren]** klicken.

   ![](assets/enable-disable-custom-object-sync-3.png)

   >[!NOTE]
   >
   >Eine Synchronisierung des benutzerdefinierten Veeva-Objektschemas kann einige Minuten dauern.

1. Klicken Sie **[!UICONTROL Schema aktualisieren]**.

   ![](assets/enable-disable-custom-object-sync-4.png)

Wählen Sie das zu synchronisierende Objekt aus und klicken Sie auf Synchronisierung aktivieren .

![](assets/enable-disable-custom-object-sync-5.png)

>[!TIP]
>
>Marketo kann ein benutzerdefiniertes Objekt nur synchronisieren, wenn es eine direkte Beziehung mit dem Kontakt- oder Kontoobjekt in Veeva CRM hat.

1. Klicken Sie erneut **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/enable-disable-custom-object-sync-6.png)

1. Gehen Sie zurück zur Registerkarte Veeva und klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/enable-disable-custom-object-sync-7.png)

## Verwenden benutzerdefinierter Objekte {#using-your-custom-objects}

>[!NOTE]
>
>Benutzerdefinierte Objekte können nicht in Smart-Kampagnen mit Triggern verwendet werden.

1. Ziehen Sie in Ihrer Smart List den Filter „Hat Chance“ auf den Bereich und legen Sie ihn auf **[!UICONTROL True]** fest.

   ![](assets/enable-disable-custom-object-sync-8.png)

1. Verwenden Sie optional Filtereinschränkungen, um den Fokus einzugrenzen.

   ![](assets/enable-disable-custom-object-sync-9.png)

Ausgezeichnet! Sie können jetzt die Daten dieses benutzerdefinierten Objekts in Smart-Kampagnen und Smart-Listen verwenden.

>[!MORELIKETHIS]
>
>[Benutzerdefiniertes Objektfeld als Smart-Listen-/Trigger-Einschränkungen hinzufügen/entfernen](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
