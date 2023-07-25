---
unique-page-id: 4719308
description: Hinzufügen eines vorhandenen Salesforce-Felds zur Marketo-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen eines vorhandenen Salesforce-Felds zur Marketo-Synchronisierung
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Hinzufügen eines vorhandenen Salesforce-Felds zur Marketo-Synchronisierung {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

Normalerweise werden neue benutzerdefinierte Felder in Salesforce automatisch mit Marketo synchronisiert. Andernfalls sind die Felder für den Marketo-Synchronisierungsbenutzer möglicherweise nicht sichtbar. So kannst du das beheben.

1. Klicken Sie auf Ihren Namen und wählen Sie **Einrichtung**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Eingabe **profile** in der linken Suchleiste und klicken Sie auf **Profile** under **Benutzer verwalten**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Klicken Sie auf das Profil des Synchronisierungsbenutzers.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. Unter dem **Sicherheit auf Feldebene** Abschnitt, klicken Sie auf **Ansicht** neben dem Objekt, das das Feld enthält.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Klicken **Bearbeiten**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Überprüfen Sie die **Sichtbar** Kontrollkästchen für das Feld, das Sie zur Synchronisierung hinzufügen möchten, und klicken Sie auf **Speichern**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   Süß! Beim nächsten Synchronisierungszyklus wird Marketo das Feld sehen und die Magie starten.

   >[!NOTE]
   >
   > Wenn das Feld bereits über Werte in Salesforce verfügt, werden diese Werte erst beim nächsten Datensatz-Update mit Marketo synchronisiert.
