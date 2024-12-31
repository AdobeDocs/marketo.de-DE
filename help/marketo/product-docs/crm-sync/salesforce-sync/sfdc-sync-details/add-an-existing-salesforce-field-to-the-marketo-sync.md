---
unique-page-id: 4719308
description: Hinzufügen eines bestehenden Salesforce-Felds zur Marketo-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen eines vorhandenen Salesforce-Felds zur Marketo-Synchronisierung
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 1%

---

# Hinzufügen eines vorhandenen Salesforce-Felds zur Marketo-Synchronisierung {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

Normalerweise werden neue benutzerdefinierte Felder in Salesforce automatisch mit Marketo Engage synchronisiert. Andernfalls sind die Felder für den Marketo Sync-Benutzer möglicherweise nicht sichtbar. So können Sie das beheben.

1. Klicken Sie auf Ihren Namen und wählen Sie **[!UICONTROL Setup]** aus.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Geben Sie in der linken Suchleiste „Profil“ ein und klicken Sie unter **[!UICONTROL Benutzer verwalten]** auf **[!UICONTROL Profile]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Klicken Sie auf das Profil des Benutzers synchronisieren.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. Klicken Sie **[!UICONTROL Abschnitt „Sicherheit auf]**&quot; auf **[!UICONTROL Anzeigen]** neben dem Objekt, das das Feld enthält.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Klicken Sie auf **[!UICONTROL Bearbeiten]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Markieren Sie das **[!UICONTROL Sichtbar]** für das Feld, das Sie der Synchronisierung hinzufügen möchten, und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   Beim nächsten Synchronisationszyklus sieht Marketo das Feld und startet die Magie.

   >[!NOTE]
   >
   > Wenn das Feld bereits Werte in Salesforce enthält, werden diese Werte erst bei der nächsten Datensatzaktualisierung mit Marketo synchronisiert.
