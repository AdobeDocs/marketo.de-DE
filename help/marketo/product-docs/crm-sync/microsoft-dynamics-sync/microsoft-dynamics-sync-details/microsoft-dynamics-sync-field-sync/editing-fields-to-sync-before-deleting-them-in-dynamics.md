---
description: Bearbeiten von zu synchronisierenden Feldern vor dem Löschen in Dynamics - Marketo Docs - Produktdokumentation
title: Zu synchronisierende Felder vor dem Löschen in Dynamics bearbeiten
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Zu synchronisierende Felder vor dem Löschen in Dynamics bearbeiten {#editing-fields-to-sync-before-deleting-them-in-dynamics}

Manchmal können Sie Felder in Dynamics löschen. Marketo behält die Feldliste als Referenz bei, auf der die Synchronisierung basieren soll. Wenn ein Feld in Dynamics gelöscht wird, während die Synchronisierung aktiviert ist, kann es bei der Synchronisierung zu Fehlern kommen. Gehen Sie wie folgt vor, bevor Sie Felder löschen.

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. Klicken Sie unter &quot;Integration&quot;auf **Microsoft Dynamics**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Klicken **Synchronisierung deaktivieren**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. Melden Sie sich in einer neuen Registerkarte in Ihrem Browser bei Dynamics an und löschen Sie die gewünschten Felder.

1. Klicken Sie in Marketo unter &quot;Microsoft Dynamics&quot;auf **Bearbeiten** neben &quot;Schritt 2: Wählen Sie Zu synchronisierende Felder aus.&quot;

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Überprüfen Sie die Felder und klicken Sie auf **Speichern**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>Klicken **Speichern** ist erforderlich, um das aktualisierte Schema für die Synchronisierung zu speichern, selbst wenn keine Änderungen vorgenommen wurden.

>[!NOTE]
>
>Wenn die Synchronisierung vor dem Löschen eines Felds in Dynamics nicht angehalten wird, kann es zu Fehlern bei der Synchronisierung kommen. Ist dies der Fall, wird die Synchronisierung beendet. Vor der Wiederaufnahme muss der Marketo-Administrator die Option &quot;Zu synchronisierende Felder auswählen&quot;(siehe oben) durchsuchen und auf **Speichern** , damit die Synchronisierung die Schemaänderungen akzeptiert.

Denken Sie daran, die Synchronisierung zu aktivieren, nachdem die Änderungen gespeichert wurden!
