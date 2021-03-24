---
description: Bearbeiten von zu synchronisierenden Feldern vor dem Löschen in Dynamik - Marketing-Dokumente - Produktdokumentation
title: Zu synchronisierende Felder bearbeiten, bevor sie in Dynamik gelöscht werden
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---


# Bearbeiten von zu synchronisierenden Feldern vor dem Löschen in Dynamik {#editing-fields-to-sync-before-deleting-them-in-dynamics}

Manchmal möchten Sie Felder in Dynamics löschen. Marketo behält die Liste des Felds als Referenz für die Synchronisierung bei. Wenn ein Feld in Dynamics gelöscht wird, während die Synchronisierung aktiviert ist, kann es zu Fehlern bei der Synchronisierung kommen. Gehen Sie wie folgt vor, bevor Sie Felder löschen.

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. Klicken Sie unter Integration auf **Microsoft Dynamics**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Klicken Sie auf **Synchronisierung deaktivieren**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. Melden Sie sich auf einer neuen Registerkarte in Ihrem Browser bei Dynamics an und löschen Sie die gewünschten Felder.

1. Zurück in Marketo klicken Sie unter Microsoft Dynamics auf **Bearbeiten** neben &quot;Schritt 2: Wählen Sie die zu synchronisierenden Felder aus.&quot;

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Überprüfen Sie die Felder und klicken Sie auf **Speichern**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>Klicken Sie auf **Speichern**, um das aktualisierte Schema für die Synchronisierung zu speichern, auch wenn keine Änderungen vorgenommen wurden.

>[!NOTE]
>
>Wenn die Synchronisierung vor dem Löschen eines Felds in Dynamics nicht beendet wird, kann es zu Fehlern bei der Synchronisierung kommen. Ist dies der Fall, wird die Synchronisierung beendet. Vor der Wiederaufnahme muss der Marketing-Administrator die Meldung &quot;Zu synchronisierende Felder auswählen&quot;(siehe oben) überprüfen und auf **Speichern** klicken, damit die Synchronisierung die Änderungen des Schemas akzeptiert.

Denken Sie daran, die Synchronisierung zu aktivieren, nachdem die Änderungen gespeichert wurden!
