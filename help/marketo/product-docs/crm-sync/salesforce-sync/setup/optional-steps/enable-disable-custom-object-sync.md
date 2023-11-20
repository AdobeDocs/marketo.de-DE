---
unique-page-id: 4719297
description: Benutzerdefinierte Objektsynchronisierung aktivieren/deaktivieren - Marketo Docs - Produktdokumentation
title: Benutzerdefinierte Objektsynchronisierung aktivieren/deaktivieren
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Benutzerdefinierte Objektsynchronisierung aktivieren/deaktivieren {#enable-disable-custom-object-sync}

Benutzerdefinierte Objekte, die in Ihrer Salesforce-Instanz erstellt wurden, können ebenfalls Teil von Marketo Engage sein. So richten Sie es ein.

## Benutzerdefinierte Objektsynchronisierung aktivieren/deaktivieren {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Klicks **[!UICONTROL Admin]**.

   ![](assets/one.png)

1. Klicken Sie im Menü Datenbankverwaltung auf **[!UICONTROL Salesforce-Objektsynchronisierung]**.

   ![](assets/two-2.png)

1. Wenn dies Ihr erstes benutzerdefiniertes Objekt ist, klicken Sie auf **[!UICONTROL Schema synchronisieren]**. Klicken Sie andernfalls auf **[!UICONTROL Schema aktualisieren]** , um sicherzustellen, dass Sie über die neueste Version verfügen.

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. Wenn Ihre globale Synchronisierung ausgeführt wird, müssen Sie sie deaktivieren, indem Sie auf **[!UICONTROL Globale Synchronisierung deaktivieren]**.

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >Die Synchronisierung des benutzerdefinierten Salesforce-Objektschemas kann einige Minuten dauern.

1. Klicks **[!UICONTROL Schema aktualisieren]**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Wählen Sie das zu synchronisierende Objekt aus und klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   >[!TIP]
   >
   >Marketo kann ein benutzerdefiniertes Objekt nur synchronisieren, wenn es eine direkte Beziehung zum Lead-, Kontakt- oder Kontoobjekt in Salesforce aufweist.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Klicks **[!UICONTROL Synchronisierung aktivieren]** erneut.

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. Gehen Sie zurück zu **[!DNL Salesforce]** Registerkarte und klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Verwenden Ihrer benutzerdefinierten Objekte {#using-your-custom-objects}

>[!NOTE]
>
>Sie können keine benutzerdefinierten Objekte in Smart-Kampagnen mit Triggern verwenden.

1. Ziehen Sie in Ihrer Smart-Liste über die **[!UICONTROL Hat Chancen]** filtern und auf **[!UICONTROL true]**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. Verwenden Sie dann Filterbegrenzungen, um den Fokus einzuschränken.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Ausgezeichnet! Sie können jetzt die Daten dieses benutzerdefinierten Objekts in Smart-Kampagnen und Smart-Listen verwenden.

>[!MORELIKETHIS]
>
>[Benutzerdefiniertes Objektfeld als Smart-List-/Trigger-Einschränkungen hinzufügen/entfernen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
