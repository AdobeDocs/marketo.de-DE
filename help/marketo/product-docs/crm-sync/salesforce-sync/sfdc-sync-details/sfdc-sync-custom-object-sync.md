---
unique-page-id: 2953471
description: SFDC-Synchronisierung - Benutzerdefinierte Objektsynchronisierung - Marketing-Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Benutzerdefinierte Objektsynchronisierung
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%

---


# SFDC-Synchronisierung: Eigene Objektsynchronisierung {#sfdc-sync-custom-object-sync}

Benutzerdefinierte Objekte, die in Ihrer Salesforce-Instanz erstellt wurden, können auch Teil von Marketo sein.  So richten Sie es ein:

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!PREREQUISITES]
>
>Um ein benutzerdefiniertes Objekt zu verwenden, muss es mit einem [Interessenten](sfdc-sync-lead-sync.md)-, [](sfdc-sync-contact-sync.md)Schützen- [](sfdc-sync-account-sync.md)Konto in Salesforce verknüpft sein.

## Benutzerdefiniertes Objekt aktivieren  {#enable-custom-object}

1. Klicken Sie auf **Admin** und den **Link** zur Synchronisierung von Salesforce-Objekten.****

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Wenn dies Ihr erstes benutzerdefiniertes Objekt ist, klicken Sie auf Schema **synchronisieren.**

   ![](assets/rtaimage-2.png)

1. Klicken Sie auf Globale Synchronisierung **deaktivieren.**

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

1. Klicken Sie auf Synchronisierung **aktivieren.**

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Klicken Sie erneut auf Synchronisierung **aktivieren** .

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >**Erinnerung**
   >
   >
   >Vergessen Sie nicht, Ihre globale Synchronisierung erneut zu aktivieren!

1. Gehen Sie zurück zur Registerkarte **Salesforce **s.

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Klicken Sie auf Synchronisierung **aktivieren.**

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Um alle Ihre Salesforce-Objekte Ansicht, klicken Sie auf den Link **Admin** und auf den Link** Salesforce-Objekte synchronisieren **(siehe oben Schritt 1).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo unterstützt nur benutzerdefinierte Entitäten, die mit standardmäßigen Entitäten in einer oder zwei Ebenen verknüpft sind.

### Nächste Schritte: {#whats-next}

[Benutzerdefiniertes Objektfeld als Einschränkungen für intelligente Liste/Auslöser Hinzufügen/entfernen](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

Ausgezeichnet! Sie können jetzt Daten aus diesem benutzerdefinierten Objekt in intelligenten Kampagnen und intelligenten Listen verwenden.

