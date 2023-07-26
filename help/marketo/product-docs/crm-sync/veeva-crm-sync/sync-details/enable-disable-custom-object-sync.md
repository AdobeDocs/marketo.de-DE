---
description: Benutzerdefinierte Objektsynchronisierung aktivieren/deaktivieren - Marketo Docs - Produktdokumentation
title: Benutzerdefinierte Objektsynchronisierung aktivieren/deaktivieren
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Benutzerdefinierte Objektsynchronisierung aktivieren/deaktivieren {#enable-disable-custom-object-sync}

Benutzerdefinierte Objekte, die in Ihrer VEE CRM-Instanz erstellt wurden, können ebenfalls Teil von Marketo Engage sein. So richten Sie es ein.

## Benutzerdefinierte Objektsynchronisierung aktivieren oder deaktivieren {#enable-or-disable-the-custom-object-sync}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Klicken Sie in Marketo auf **Admin**, dann **VEC-Objektsynchronisierung**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. Wenn es Ihr erstes benutzerdefiniertes Objekt ist, klicken Sie auf Schema synchronisieren . Wenn nicht, klicken Sie auf **Schema aktualisieren** , um sicherzustellen, dass Sie über die neueste Version verfügen.

   ![](assets/enable-disable-custom-object-sync-2.png)

1. Wenn Ihre globale Synchronisierung ausgeführt wird, deaktivieren Sie sie, indem Sie auf **Globale Synchronisierung deaktivieren**.

   ![](assets/enable-disable-custom-object-sync-3.png)

   >[!NOTE]
   >
   >Die Synchronisierung des benutzerdefinierten Objektschemas von Veeva kann einige Minuten dauern.

1. Klicks **Schema aktualisieren**.

   ![](assets/enable-disable-custom-object-sync-4.png)

Wählen Sie das zu synchronisierende Objekt aus und klicken Sie auf Synchronisierung aktivieren .

![](assets/enable-disable-custom-object-sync-5.png)

>[!TIP]
>
>Marketo kann ein benutzerdefiniertes Objekt nur dann synchronisieren, wenn es eine direkte Beziehung zum Kontakt- oder Kontoobjekt in Veeva CRM hat.

1. Klicks **Synchronisierung aktivieren** erneut.

   ![](assets/enable-disable-custom-object-sync-6.png)

1. Gehen Sie zurück zur Registerkarte Veeva und klicken Sie auf **Synchronisierung aktivieren**.

   ![](assets/enable-disable-custom-object-sync-7.png)

## Verwenden Ihrer benutzerdefinierten Objekte {#using-your-custom-objects}

>[!NOTE]
>
>Sie können keine benutzerdefinierten Objekte in Smart-Kampagnen mit Triggern verwenden.

1. Ziehen Sie in Ihre Smart-Liste den Filter &quot;Hat Chancen&quot;und legen Sie **True**.

   ![](assets/enable-disable-custom-object-sync-8.png)

1. Verwenden Sie optional Filterbegrenzungen, um den Fokus einzuschränken.

   ![](assets/enable-disable-custom-object-sync-9.png)

Ausgezeichnet! Sie können jetzt die Daten dieses benutzerdefinierten Objekts in Smart-Kampagnen und Smart-Listen verwenden.

>[!MORELIKETHIS]
>
>[Benutzerdefiniertes Objektfeld als Smart-List-/Trigger-Einschränkungen hinzufügen/entfernen](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
