---
unique-page-id: 4719308
description: Erfahren Sie, wie Sie ein vorhandenes Salesforce-Feld zur Marketo-Synchronisierung hinzufügen. Feld für den Synchronisierungsbenutzer in Salesforce sichtbar machen, damit es beim nächsten Zyklus synchronisiert wird.
title: Hinzufügen eines vorhandenen Salesforce-Felds zur Marketo-Synchronisierung
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 8%

---

# Hinzufügen eines vorhandenen [!DNL Salesforce] zur Marketo-Synchronisierung {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Admin-Berechtigungen erforderlich**

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
   > Wenn das Feld bereits Werte in [!DNL Salesforce] enthält, werden diese Werte erst bei der nächsten Datensatzaktualisierung mit Marketo synchronisiert.
