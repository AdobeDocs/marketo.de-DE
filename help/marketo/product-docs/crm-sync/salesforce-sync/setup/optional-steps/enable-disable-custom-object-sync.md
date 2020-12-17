---
unique-page-id: 4719297
description: Benutzerdefinierte Objektsynchronisierung aktivieren/deaktivieren - MarketingToDocs - Produktdokumentation
title: Benutzerdefinierte Objektsynchronisierung aktivieren/deaktivieren
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# Benutzerdefinierte Objektsynchronisierung aktivieren/deaktivieren {#enable-disable-custom-object-sync}

Benutzerdefinierte Objekte, die in Ihrer Salesforce-Instanz erstellt wurden, können auch Teil von Marketo sein. So richten Sie es ein:

## Benutzerdefinierte Objektsynchronisierung aktivieren/deaktivieren {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>Administratorrechte erforderlich.

1. Klicken Sie auf **Admin**.

   ** ![](assets/one.png)

   **

1. Klicken Sie im Menü Datenbankverwaltung auf **Salesforce** **Objekte synchronisieren**.

   ![](assets/two-2.png)

1. Wenn dies Ihr erstes benutzerdefiniertes Objekt ist, klicken Sie auf **Schema synchronisieren.** Klicken Sie andernfalls auf  **Schema** aktualisieren, um sicherzustellen, dass Sie die neuesten Informationen haben.

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. Wenn Ihre globale Synchronisierung ausgeführt wird, müssen Sie sie deaktivieren, indem Sie auf **Globale Synchronisierung deaktivieren.**

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >Die Synchronisierung des benutzerdefinierten Salesforce-Schemas kann einige Minuten dauern.

1. Klicken Sie auf **Schema aktualisieren**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Wählen Sie das zu synchronisierende Objekt aus und klicken Sie auf **Synchronisierung aktivieren**.

   >[!TIP]
   >
   >Marketo kann ein benutzerdefiniertes Objekt nur synchronisieren, wenn es eine direkte Beziehung zum Lead-, Kontakt- oder Kontoobjekt in Salesforce hat.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Klicken Sie erneut auf **Synchronisierung aktivieren**.

   ** ![](assets/image2014-12-10-10-3a15-3a40.png)

   **

1. Gehen Sie zurück zum Register **Salesforce** und klicken Sie auf **Synchronisierung aktivieren**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Verwenden Ihrer benutzerdefinierten Objekte {#using-your-custom-objects}

>[!NOTE]
>
>Sie können benutzerdefinierte Objekte nicht mit Auslösern in intelligenten Kampagnen verwenden.

1. Ziehen Sie in der intelligenten Liste über den Filter **Hat Gelegenheit** und setzen Sie ihn auf **true**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. Verwenden Sie dann Filtereinschränkungen, um den Fokus einzuschränken.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Ausgezeichnet! Sie können jetzt die Daten dieses benutzerdefinierten Objekts in intelligenten Kampagnen und intelligenten Listen verwenden.

>[!MORELIKETHIS]
>
>* [Benutzerdefiniertes Objektfeld als Einschränkungen für intelligente Liste/Auslöser Hinzufügen/entfernen](add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

>



