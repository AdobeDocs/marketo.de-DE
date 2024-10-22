---
unique-page-id: 2953471
description: SFDC Sync - Custom Object Sync - Marketo Docs - Produktdokumentation
title: SFDC Sync - benutzerdefinierte Objektsynchronisierung
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
feature: Salesforce Integration
source-git-commit: 79ae0d56dd4bb8bf563c6546cba54b89b5841425
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# SFDC Sync: Benutzerdefinierte Objektsynchronisierung {#sfdc-sync-custom-object-sync}

Benutzerdefinierte Objekte, die in Ihrer Salesforce-Instanz erstellt wurden, können ebenfalls Teil von Marketo Engage sein. So richten Sie es ein.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!PREREQUISITES]
>
>Um ein benutzerdefiniertes Objekt zu verwenden, muss es mit einem [Lead](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md){target="_blank"}-, [Kontakt](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"}- oder [Konto](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"}-Objekt in Salesforce verknüpft sein.

>[!IMPORTANT]
>
>Der Marketo Sync User benötigt Lesezugriff auf das benutzerdefinierte Objekt, um es aufzulisten und eine Synchronisierung durchzuführen.

## Benutzerdefiniertes Objekt aktivieren  {#enable-custom-object}

1. Klicken Sie auf den Link **[!UICONTROL Admin]** und auf den Link **[!UICONTROL Salesforce Objects Sync]** .

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Wenn dies Ihr erstes benutzerdefiniertes Objekt ist, klicken Sie auf **[!UICONTROL Schema synchronisieren]**.

   ![](assets/rtaimage-2.png)

1. Klicken Sie auf **[!UICONTROL Globale Synchronisierung deaktivieren]**.

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

1. Klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Klicken Sie erneut auf **[!UICONTROL Synchronisierung aktivieren]** .

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >Vergessen Sie nicht, Ihre globale Synchronisation erneut zu aktivieren!

1. Gehen Sie zurück zur Registerkarte **Salesforce** .

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Um alle benutzerdefinierten Salesforce-Objekte anzuzeigen, klicken Sie auf **[!UICONTROL Admin]** und den Link **[!UICONTROL Salesforce Objects Sync]** (wie in Schritt 1 oben).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >* Marketo unterstützt nur benutzerdefinierte Entitäten, die mit Standardentitäten verknüpft sind, die eine oder zwei Ebenen tief sind.
   >
   >* Die benutzerdefinierte Objektstruktur kann dasselbe Objekt mehrmals anzeigen, da sie direkt mit einem der Hauptobjekte verbunden ist (z. B. Leads, Kontakte oder Konten oder indirekte Verbindungen über ein Intermediarobjekt). Wählen Sie in diesem Fall das Objekt aus, das dem Hauptobjekt am nächsten liegt, und wählen Sie nur eines aus. Die mehrfache Auswahl desselben Objekts kann die Synchronisierung dieses benutzerdefinierten Objekts behindern.

### Nächste Schritte: {#whats-next}

[Benutzerdefiniertes Objektfeld als Smart List/Trigger Constraints hinzufügen/entfernen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}

Ausgezeichnet! Sie können jetzt Daten aus diesem benutzerdefinierten Objekt in Smart-Kampagnen und Smart-Listen verwenden.
