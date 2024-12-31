---
unique-page-id: 2953471
description: SFDC-Synchronisierung - Benutzerdefinierte Objektsynchronisierung - Marketo-Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Synchronisierung benutzerdefinierter Objekte
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
feature: Salesforce Integration
source-git-commit: 79ae0d56dd4bb8bf563c6546cba54b89b5841425
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# SFDC-Synchronisierung: Benutzerdefinierte Objektsynchronisierung {#sfdc-sync-custom-object-sync}

Benutzerdefinierte Objekte, die in Ihrer Salesforce-Instanz erstellt wurden, können auch Teil von Marketo Engage sein. So richten Sie es ein.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!PREREQUISITES]
>
>Um ein benutzerdefiniertes Objekt zu verwenden, muss es mit einem [Lead](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md){target="_blank"}-, [Kontakt](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"}- oder [Konto](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"}-Objekt in Salesforce verknüpft sein.

>[!IMPORTANT]
>
>Der Marketo-Synchronisierungsbenutzer benötigt Lesezugriff auf das benutzerdefinierte Objekt, um es aufzulisten und eine Synchronisierung mit ihm durchzuführen.

## Benutzerdefiniertes Objekt aktivieren  {#enable-custom-object}

1. Klicken Sie auf **[!UICONTROL Admin]** und den Link **[!UICONTROL Salesforce-Objekte synchronisieren]**.

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Wenn dies das erste benutzerdefinierte Objekt ist, klicken Sie auf **[!UICONTROL Schema synchronisieren]**.

   ![](assets/rtaimage-2.png)

1. Klicken Sie **[!UICONTROL Globale Synchronisierung deaktivieren]**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Eine Erstsynchronisierung des benutzerdefinierten Salesforce-Objektschemas kann einige Minuten dauern.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Ziehen Sie das benutzerdefinierte Objekt, das Sie synchronisieren möchten, auf die Arbeitsfläche.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Benutzerdefinierte Objekte müssen eindeutige Namen haben. Marketo unterstützt nicht zwei verschiedene benutzerdefinierte Objekte mit demselben Namen.

1. Klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Klicken Sie erneut **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >Vergessen Sie nicht, die globale Synchronisierung erneut zu aktivieren!

1. Kehren Sie zur Registerkarte **Salesforce** zurück.

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Um alle Ihre benutzerdefinierten Salesforce-Objekte anzuzeigen, klicken Sie auf **[!UICONTROL Admin]** und den Link **[!UICONTROL Salesforce-Objekte synchronisieren]** (wie in Schritt 1 oben).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >* Marketo unterstützt nur benutzerdefinierte Entitäten, die mit Standardelementen eine oder zwei Ebenen tief verknüpft sind.
   >
   >* Der benutzerdefinierte Objektbaum kann dasselbe Objekt mehrmals anzeigen, da es direkt mit einem der Hauptobjekte verbunden ist (z. B. Leads, Kontakte, Konten oder indirekte Verbindungen über ein Zwischenobjekt). Wählen Sie in solchen Fällen das Objekt aus, das dem Hauptobjekt am nächsten ist, und wählen Sie nur eines. Die mehrfache Auswahl desselben Objekts kann die Synchronisierung dieses benutzerdefinierten Objekts beeinträchtigen.

### Wie geht es weiter: {#whats-next}

[Benutzerdefiniertes Objektfeld als Smart-Listen-/Trigger-Einschränkungen hinzufügen/entfernen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}

Ausgezeichnet! Sie können jetzt Daten aus diesem benutzerdefinierten Objekt in Smart-Kampagnen und Smart-Listen verwenden.
