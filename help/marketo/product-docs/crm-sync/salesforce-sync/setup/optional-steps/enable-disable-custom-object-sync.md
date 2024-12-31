---
unique-page-id: 4719297
description: Aktivieren/Deaktivieren der Synchronisierung benutzerdefinierter Objekte - Marketo-Dokumente - Produktdokumentation
title: Benutzerdefinierte Objektsynchronisierung aktivieren/deaktivieren
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Benutzerdefinierte Objektsynchronisierung aktivieren/deaktivieren {#enable-disable-custom-object-sync}

Benutzerdefinierte Objekte, die in Ihrer Salesforce-Instanz erstellt wurden, können auch Teil von Marketo Engage sein. So richten Sie es ein.

## Benutzerdefinierte Objektsynchronisierung aktivieren/deaktivieren {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Klicken Sie auf **[!UICONTROL Admin]**.

   ![](assets/one.png)

1. Klicken Sie im Menü „Datenbankverwaltung“ auf **[!UICONTROL Salesforce-Objekte synchronisieren]**.

   ![](assets/two-2.png)

1. Wenn dies das erste benutzerdefinierte Objekt ist, klicken Sie auf **[!UICONTROL Schema synchronisieren]**. Klicken Sie andernfalls auf **[!UICONTROL Schema aktualisieren]**, um sicherzustellen, dass Sie über die neueste verfügen.

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. Wenn die globale Synchronisierung ausgeführt wird, müssen Sie sie deaktivieren, indem Sie auf **[!UICONTROL Globale Synchronisierung deaktivieren]** klicken.

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >Eine Synchronisierung des benutzerdefinierten Salesforce-Objektschemas kann einige Minuten dauern.

1. Klicken Sie **[!UICONTROL Schema aktualisieren]**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Wählen Sie das zu synchronisierende Objekt aus und klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   >[!TIP]
   >
   >Marketo kann ein benutzerdefiniertes Objekt nur synchronisieren, wenn es eine direkte Beziehung mit dem Lead-, Kontakt- oder Kontoobjekt in Salesforce hat.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Klicken Sie erneut **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. Gehen Sie zurück zur Registerkarte **[!DNL Salesforce]** und klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Verwenden benutzerdefinierter Objekte {#using-your-custom-objects}

>[!NOTE]
>
>Benutzerdefinierte Objekte können nicht in Smart-Kampagnen mit Triggern verwendet werden.

1. Ziehen Sie in Ihrer Smart List den Filter **[!UICONTROL Hat Opportunity]** und setzen Sie ihn auf **[!UICONTROL true]**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. Verwenden Sie dann Filtereinschränkungen, um den Fokus einzugrenzen.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Ausgezeichnet! Sie können jetzt die Daten dieses benutzerdefinierten Objekts in Smart-Kampagnen und Smart-Listen verwenden.

>[!MORELIKETHIS]
>
>[Benutzerdefiniertes Objektfeld als Smart-Listen-/Trigger-Einschränkungen hinzufügen/entfernen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
