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

1. Klicken Sie auf Ihren Namen und wählen Sie dann **[!UICONTROL Einrichten]** aus.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Geben Sie in der linken Suchleiste &quot;profile&quot;ein und klicken Sie unter **[!UICONTROL Benutzer verwalten]** auf **[!UICONTROL Profile]** .

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Klicken Sie auf das Profil des Synchronisierungsbenutzers.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. Klicken Sie unter dem Abschnitt **[!UICONTROL Sicherheit auf Feldebene]** neben dem Objekt, das das Feld enthält, auf **[!UICONTROL Anzeigen]** .

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Klicken Sie auf **[!UICONTROL Bearbeiten]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Aktivieren Sie das Kontrollkästchen **[!UICONTROL Sichtbar]** für das Feld, das Sie zur Synchronisierung hinzufügen möchten, und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   Beim nächsten Synchronisierungszyklus wird Marketo das Feld sehen und die Magie starten.

   >[!NOTE]
   >
   > Wenn das Feld bereits über Werte in Salesforce verfügt, werden diese Werte erst beim nächsten Datensatz-Update mit Marketo synchronisiert.
