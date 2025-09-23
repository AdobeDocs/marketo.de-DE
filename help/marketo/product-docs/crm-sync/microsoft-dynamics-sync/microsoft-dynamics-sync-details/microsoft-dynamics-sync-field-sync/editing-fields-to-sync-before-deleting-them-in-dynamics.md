---
description: Bearbeiten von Feldern, die vor dem Löschen synchronisiert werden sollen, in Dynamics - Marketo-Dokumente - Produktdokumentation
title: Bearbeiten von Feldern, die vor dem Löschen in Dynamics synchronisiert werden sollen
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 4%

---

# Bearbeiten von Feldern, die vor dem Löschen in [!DNL Dynamics] synchronisiert werden sollen {#editing-fields-to-sync-before-deleting-them-in-dynamics}

Manchmal empfiehlt es sich, Felder in [!DNL Dynamics] zu löschen. Marketo speichert die Feldliste als Referenz, auf der die Synchronisierung basieren soll. Wenn ein Feld in [!DNL Dynamics] gelöscht wird, während die Synchronisierung aktiviert ist, kann es zu Fehlern bei der Synchronisierung kommen. Bevor Sie Felder löschen, gehen Sie wie folgt vor.

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. Klicken [!UICONTROL &#x200B; unter „Integration] auf **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Klicken Sie auf **[!UICONTROL Synchronisierung deaktivieren]**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. Melden Sie sich auf einer neuen Registerkarte in Ihrem Browser bei [!DNL Dynamics] an und löschen Sie Ihre gewünschten Felder.

1. Zurück in Marketo klicken Sie unter [!DNL Microsoft Dynamics] auf **[!UICONTROL Bearbeiten]** neben &quot;[!UICONTROL Schritt 2: Zu synchronisierende Felder auswählen].

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Überprüfen Sie die Felder und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>Wenn Sie auf **[!UICONTROL Speichern]** klicken, wird das aktualisierte Schema für die Synchronisierung gespeichert, auch wenn keine Änderungen vorgenommen wurden.

>[!NOTE]
>
>Wenn die Synchronisierung nicht gestoppt wird, bevor ein Feld in [!DNL Dynamics] gelöscht wurde, kann es zu Fehlern bei der Synchronisierung kommen. Wenn dies der Fall ist, wird die Synchronisierung beendet. Vor der Wiederaufnahme muss der Marketo-Administrator &quot;[!UICONTROL Zu synchronisierende Felder auswählen]&quot; (siehe oben) überprüfen und auf **[!UICONTROL Speichern]** klicken, damit die Synchronisierung die Schemaänderungen akzeptiert.

Denken Sie daran, die Synchronisierung zu aktivieren, nachdem die Änderungen gespeichert wurden!
