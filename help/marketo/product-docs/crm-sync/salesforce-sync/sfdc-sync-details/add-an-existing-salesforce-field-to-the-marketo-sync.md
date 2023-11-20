---
unique-page-id: 4719308
description: Hinzufügen eines vorhandenen Salesforce-Felds zur Marketo-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen eines vorhandenen Salesforce-Felds zur Marketo-Synchronisierung
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Hinzufügen eines vorhandenen Salesforce-Felds zur Marketo-Synchronisierung {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

Normalerweise werden neue benutzerdefinierte Felder in Salesforce automatisch mit Marketo Engage synchronisiert. Andernfalls sind die Felder für den Marketo-Synchronisierungsbenutzer möglicherweise nicht sichtbar. So kannst du das beheben.

1. Klicken Sie auf Ihren Namen und wählen Sie **[!UICONTROL Einrichtung]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Geben Sie &quot;profile&quot;in die linke Suchleiste ein und klicken Sie auf **[!UICONTROL Profile]** under **[!UICONTROL Benutzer verwalten]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Klicken Sie auf das Profil des Synchronisierungsbenutzers.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. Unter dem **[!UICONTROL Sicherheit auf Feldebene]** Abschnitt, klicken Sie auf **[!UICONTROL Ansicht]** neben dem Objekt, das das Feld enthält.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Klicks **[!UICONTROL Bearbeiten]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Überprüfen Sie die **[!UICONTROL Sichtbar]** Kontrollkästchen für das Feld, das Sie zur Synchronisierung hinzufügen möchten, und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   Beim nächsten Synchronisierungszyklus wird Marketo das Feld sehen und die Magie starten.

   >[!NOTE]
   >
   > Wenn das Feld bereits über Werte in Salesforce verfügt, werden diese Werte erst beim nächsten Datensatz-Update mit Marketo synchronisiert.
