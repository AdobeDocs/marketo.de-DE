---
description: Benutzerdefinierte Objektsynchronisierung - Marketo-Dokumente - Produktdokumentation
title: Benutzerdefinierte Objektsynchronisierung
hide: true
hidefromtoc: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
feature: Veeva CRM
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---

# Benutzerdefinierte Objektsynchronisierung {#custom-object-sync}

Benutzerdefinierte Objekte, die in Ihrer VEE CRM-Instanz erstellt wurden, können ebenfalls Teil von Marketo Engage sein. So richten Sie es ein.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!PREREQUISITES]
>
>Um ein benutzerdefiniertes Objekt zu verwenden, muss es mit einem Kontakt- oder Kontoobjekt in Veeva CRM verknüpft sein.

## Benutzerdefiniertes Objekt aktivieren {#enable-custom-object}

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]** und dann auf **[!UICONTROL Veeva Objects Sync]**.

   ![](assets/custom-object-sync-1.png)

1. Wenn dies Ihr erstes benutzerdefiniertes Objekt ist, klicken Sie auf **[!UICONTROL Schema synchronisieren]**.

   ![](assets/custom-object-sync-2.png)

1. Klicken Sie auf **[!UICONTROL Globale Synchronisierung deaktivieren]**.

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >Die anfängliche Synchronisierung des benutzerdefinierten Objektschemas von Veeva kann einige Minuten dauern.

1. Ziehen Sie das benutzerdefinierte Objekt, das Sie synchronisieren möchten, in die Arbeitsfläche.

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >Benutzerdefinierte Objekte müssen eindeutige Namen haben. Marketo unterstützt zwei verschiedene benutzerdefinierte Objekte mit demselben Namen nicht.

1. Klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/custom-object-sync-5.png)

1. Klicken Sie erneut auf **[!UICONTROL Synchronisierung aktivieren]** .

   ![](assets/custom-object-sync-6.png)

1. Gehen Sie zurück zur Registerkarte **[!UICONTROL Veeva]** .

   ![](assets/custom-object-sync-7.png)

1. Klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/custom-object-sync-8.png)

1. Um alle benutzerdefinierten Objekte von VEC anzuzeigen, klicken Sie auf **[!UICONTROL Admin]** und **[!UICONTROL Veeva-Objektsynchronisierung]**.

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo unterstützt nur benutzerdefinierte Entitäten, die mit Standardentitäten verknüpft sind, eine bis zwei Ebenen tief.

Ausgezeichnet! Sie können jetzt Daten aus diesem benutzerdefinierten Objekt in Smart-Kampagnen und Smart-Listen verwenden.

>[!MORELIKETHIS]
>
>* [Synchronisierungsaufruf und -aufruf für Schlüsselmeldungen](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
>* [Benutzerdefiniertes Objektfeld als Smart List/Trigger Constraints hinzufügen/entfernen](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
