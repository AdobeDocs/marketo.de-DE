---
unique-page-id: 1147031
description: Person aus SFDC löschen - Marketo-Dokumente - Produktdokumentation
title: Person aus SFDC löschen
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 5%

---

# Person aus SFDC löschen {#delete-person-from-sfdc}

Wenn Sie einen bestimmten Satz von Leads aus Salesforce entfernen müssen, sie jedoch als Personen auf dem Marketo Engage belassen müssen, können Sie die Flussaktion Person aus SFDC löschen verwenden.

>[!NOTE]
>
>Nur verfügbar, wenn mit Salesforce integriert.

1. Klicken Sie in der Datenbank auf die Person, die Sie aus Salesforce entfernen möchten. Klicken Sie dann auf **[!UICONTROL Personenaktionen]** und wählen Sie **[!DNL Salesforce]** aus.

   ![](assets/delete-person-from-sfdc-1.png)

1. Wählen Sie **[!UICONTROL Person aus SFDC löschen]**.

   ![](assets/delete-person-from-sfdc-2.png)

1. Stellen Sie sicher, dass die Einstellung **[!UICONTROL Löschen in Marketo]** auf **[!UICONTROL false]** eingestellt ist, und klicken Sie dann auf **[!UICONTROL Jetzt ausführen]**.

   ![](assets/delete-person-from-sfdc-3.png)

   Nach Ausführung des Flussschritts ist Ihre Person kein Lead mehr in Salesforce, sondern verbleibt in Marketo.

   >[!CAUTION]
   >
   >Wenn Sie **[!UICONTROL Löschen in Marketo]** auf **[!UICONTROL true]** setzen und die Personen aus Marketo und die Leads aus Salesforce löschen, sind diese unwiederbringlich verloren. Das kann nicht rückgängig gemacht werden.
