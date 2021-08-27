---
unique-page-id: 4719308
description: Hinzufügen eines vorhandenen Salesforce-Felds zur Marketo-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen eines vorhandenen Salesforce-Felds zur Marketo-Synchronisierung
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Hinzufügen eines vorhandenen Salesforce-Felds zur Marketo-Synchronisierung {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

Normalerweise werden neue benutzerdefinierte Felder in Salesforce automatisch mit Marketo synchronisiert. Andernfalls sind die Felder für den Marketo-Synchronisierungsbenutzer möglicherweise nicht sichtbar. So kannst du das beheben.

1. Klicken Sie auf Ihren Namen und wählen Sie **Setup** aus.

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. Geben Sie **profile** in die linke Suchleiste ein und klicken Sie unter **Benutzer verwalten** auf **Profile** .

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. Klicken Sie auf das Profil des Synchronisierungsbenutzers.

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. Klicken Sie unter dem Abschnitt **Sicherheit auf Feldebene** neben dem Objekt, das das Feld enthält, auf **Anzeigen** .

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. Klicken Sie auf **Bearbeiten**.

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. Aktivieren Sie das Kontrollkästchen **Sichtbar** für das Feld, das Sie zur Synchronisierung hinzufügen möchten, und klicken Sie auf **Speichern**.

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   Süß! Beim nächsten Synchronisierungszyklus wird Marketo das Feld sehen und die Magie starten.

   >[!NOTE]
   >
   > Wenn das Feld bereits über Werte in Salesforce verfügt, werden diese Werte erst beim nächsten Datensatz-Update mit Marketo synchronisiert.
