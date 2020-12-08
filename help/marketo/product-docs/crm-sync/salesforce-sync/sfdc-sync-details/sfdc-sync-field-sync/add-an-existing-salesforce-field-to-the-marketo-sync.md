---
unique-page-id: 4719308
description: hinzufügen eines vorhandenen Salesforce-Felds zur Marketing-Synchronisierung - Marketing-Dokumente - Produktdokumentation
title: hinzufügen eines vorhandenen Salesforce-Felds zur Synchronisierung des Markets
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# hinzufügen eines vorhandenen Salesforce-Felds zur Synchronisierung des Markets {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

Normalerweise werden neue benutzerdefinierte Felder in Salesforce automatisch mit Marketo synchronisiert. Ist dies nicht der Fall, sind die Felder für den Benutzer von &quot;Markieren zum Synchronisieren&quot;möglicherweise nicht sichtbar. Hier ist, wie man das reparieren kann.

1. Klicken Sie auf Ihren Namen und wählen Sie **Einstellungen**.

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. Geben Sie in der linken Suchleiste **Profil** ein und klicken Sie unter &quot;Benutzer **verwalten&quot;auf** Profil ****.

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. Klicken Sie auf das Profil des Synchronisierungsbenutzers.

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. Klicken Sie im Abschnitt Sicherheit **auf** Feldebene neben dem Objekt, das das Feld enthält, auf **Ansicht** .

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. Klicken Sie auf **Bearbeiten**.

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. Markieren Sie das Kontrollkästchen **Sichtbar** für das Feld, das Sie der Synchronisierung hinzufügen möchten, und klicken Sie auf **Speichern**.

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   Süß! Beim nächsten Synchronisierungszyklus sieht Marketo das Feld und Beginn die Magie.

   >[!NOTE]
   >
   > Wenn das Feld bereits Werte in Salesforce enthält, werden diese Werte erst nach der nächsten Datensatzaktualisierung mit Marketo synchronisiert.

