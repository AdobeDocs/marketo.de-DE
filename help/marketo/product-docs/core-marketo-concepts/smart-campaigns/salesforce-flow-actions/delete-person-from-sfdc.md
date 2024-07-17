---
unique-page-id: 1147031
description: Person aus SFDC löschen - Marketo Docs - Produktdokumentation
title: Person aus SFDC löschen
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 5%

---

# Person aus SFDC löschen {#delete-person-from-sfdc}

Wenn Sie einen bestimmten Satz von Leads aus Salesforce entfernen müssen, diese jedoch als Personen im Marketo Engage belassen möchten, können Sie die Flusshandlung Person aus SFDC löschen verwenden.

>[!NOTE]
>
>Nur verfügbar bei Integration mit Salesforce.

1. Klicken Sie in der Datenbank auf die Person, die Sie aus Salesforce entfernen möchten. Klicken Sie dann auf **[!UICONTROL Personen-Aktionen]** und wählen Sie **[!DNL Salesforce]** aus.

   ![](assets/delete-person-from-sfdc-1.png)

1. Wählen Sie **[!UICONTROL Person aus SFDC löschen]** aus.

   ![](assets/delete-person-from-sfdc-2.png)

1. Stellen Sie sicher, dass die Einstellung **[!UICONTROL Löschen in Marketo]** den Wert **[!UICONTROL false]** aufweist, und klicken Sie dann auf **[!UICONTROL Jetzt ausführen]**.

   ![](assets/delete-person-from-sfdc-3.png)

   Nachdem der Flussschritt ausgeführt wurde, wird Ihre Person nicht mehr in Salesforce als Lead fungieren, sondern in Marketo bleiben.

   >[!CAUTION]
   >
   >Wenn Sie **[!UICONTROL Löschen in Marketo]** auf **[!UICONTROL true]** festlegen und die Personen aus Marketo und die Leads aus Salesforce löschen, sind sie für immer weg. Das kann nicht rückgängig gemacht werden.
