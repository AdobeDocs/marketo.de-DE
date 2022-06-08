---
unique-page-id: 2953471
description: SFDC Sync - Custom Object Sync - Marketo Docs - Produktdokumentation
title: SFDC Sync - benutzerdefinierte Objektsynchronisierung
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# SFDC Sync: Benutzerdefinierte Objektsynchronisierung {#sfdc-sync-custom-object-sync}

Benutzerdefinierte Objekte, die in Ihrer Salesforce-Instanz erstellt wurden, können ebenfalls Teil von Marketo sein.  So richten Sie es ein.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!PREREQUISITES]
>
>Um ein benutzerdefiniertes Objekt zu verwenden, muss es mit einem [Lead](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md), [Kontakt](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)oder [account](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md) -Objekt in Salesforce.

## Benutzerdefiniertes Objekt aktivieren  {#enable-custom-object}

1. Klicken **Admin** und **Salesforce-Objektsynchronisierung** Link.

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Wenn dies Ihr erstes benutzerdefiniertes Objekt ist, klicken Sie auf **Schema synchronisieren**.

   ![](assets/rtaimage-2.png)

1. Klicken **Globale Synchronisierung deaktivieren**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Die anfängliche Synchronisierung des benutzerdefinierten Salesforce-Objektschemas kann einige Minuten dauern.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Ziehen Sie das benutzerdefinierte Objekt, das Sie synchronisieren möchten, in die Arbeitsfläche.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Benutzerdefinierte Objekte müssen eindeutige Namen haben. Marketo unterstützt zwei verschiedene benutzerdefinierte Objekte mit demselben Namen nicht.

1. Klicken **Synchronisierung aktivieren**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Klicken **Synchronisierung aktivieren** erneut.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >Vergessen Sie nicht, Ihre globale Synchronisation erneut zu aktivieren!

1. Gehen Sie zurück zu **Salesforce** Registerkarte.

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Klicken **Synchronisierung aktivieren**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Um alle benutzerdefinierten Salesforce-Objekte anzuzeigen, klicken Sie auf **Admin** und **Salesforce-Objektsynchronisierung** -Link (identisch mit Schritt 1 oben).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo unterstützt nur benutzerdefinierte Entitäten, die mit Standardentitäten verknüpft sind, die eine oder zwei Ebenen tief sind.

### Nächste Schritte: {#whats-next}

[Benutzerdefiniertes Objektfeld als Smart-List-/Trigger-Einschränkungen hinzufügen/entfernen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

Ausgezeichnet! Sie können jetzt Daten aus diesem benutzerdefinierten Objekt in Smart-Kampagnen und Smart-Listen verwenden.
