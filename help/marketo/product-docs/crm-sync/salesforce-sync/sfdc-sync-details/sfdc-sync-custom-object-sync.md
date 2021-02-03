---
unique-page-id: 2953471
description: SFDC-Synchronisierung - Benutzerdefinierte Objektsynchronisierung - Marketing-Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Benutzerdefinierte Objektsynchronisierung
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# SFDC-Synchronisierung: Benutzerdefinierte Objektsynchronisierung {#sfdc-sync-custom-object-sync}

Benutzerdefinierte Objekte, die in Ihrer Salesforce-Instanz erstellt wurden, können auch Teil von Marketo sein.  So richten Sie es ein:

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!PREREQUISITES]
>
>Um ein benutzerdefiniertes Objekt zu verwenden, muss es mit einem [lead](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md)-, [contact](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)- oder [account](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)-Objekt in Salesforce verknüpft sein.

## Benutzerdefiniertes Objekt {#enable-custom-object} aktivieren

1. Klicken Sie auf **Admin** und auf den Link **Salesforce-Objekte synchronisieren**.

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Wenn dies Ihr erstes benutzerdefiniertes Objekt ist, klicken Sie auf **Schema synchronisieren**.

   ![](assets/rtaimage-2.png)

1. Klicken Sie auf **Globale Synchronisierung deaktivieren**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Eine anfängliche Synchronisierung des benutzerdefinierten Salesforce-Schemas kann einige Minuten dauern.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Ziehen Sie das benutzerdefinierte Objekt, das Sie synchronisieren möchten, in die Arbeitsfläche.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Benutzerdefinierte Objekte müssen eindeutige Namen haben. Marketo unterstützt nicht zwei verschiedene benutzerdefinierte Objekte mit demselben Namen.

1. Klicken Sie auf **Synchronisierung aktivieren**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Klicken Sie erneut auf **Synchronisierung aktivieren**.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >Vergessen Sie nicht, Ihre globale Synchronisierung erneut zu aktivieren!

1. Gehen Sie zurück zum Register **Salesforce**.

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Klicken Sie auf **Synchronisierung aktivieren**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Um alle Ihre benutzerdefinierten Salesforce-Objekte Ansicht, klicken Sie auf **Admin** und auf den Link **Salesforce-Objekte synchronisieren** (siehe oben Schritt 1).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo unterstützt nur benutzerdefinierte Entitäten, die mit standardmäßigen Entitäten in einer oder zwei Ebenen verknüpft sind.

### Nächste Schritte: {#whats-next}

[Benutzerdefiniertes Objektfeld als Einschränkungen für intelligente Liste/Trigger Hinzufügen/entfernen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

Ausgezeichnet! Sie können jetzt Daten aus diesem benutzerdefinierten Objekt in intelligenten Kampagnen und intelligenten Listen verwenden.
