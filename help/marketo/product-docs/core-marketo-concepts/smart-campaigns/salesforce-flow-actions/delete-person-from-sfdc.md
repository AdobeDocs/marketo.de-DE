---
unique-page-id: 1147031
description: Person aus SFDC löschen - Marketo-Dokumente - Produktdokumentation
title: Löschen von Personen aus SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 6%

---

# Löschen von Personen aus SFDC {#delete-person-from-sfdc}

Wenn Sie einen bestimmten Satz von Leads aus Salesforce entfernen müssen, sie jedoch als Personen in Marketo Engage belassen, können Sie die Flussaktion Person aus SFDC löschen verwenden.

>[!NOTE]
>
>Nur verfügbar, wenn mit [!DNL Salesforce] integriert.

1. Klicken Sie in der Datenbank auf die Person, die Sie aus Salesforce entfernen möchten. Klicken Sie dann auf **[!UICONTROL Personenaktionen]** und wählen Sie **[!DNL Salesforce]** aus.

   ![](assets/delete-person-from-sfdc-1.png)

1. Wählen Sie **[!UICONTROL Person aus SFDC löschen]**.

   ![](assets/delete-person-from-sfdc-2.png)

1. Stellen Sie sicher, dass die Einstellung **[!UICONTROL Löschen in Marketo]** auf **[!UICONTROL false]** eingestellt ist, und klicken Sie dann auf **[!UICONTROL Jetzt ausführen]**.

   ![](assets/delete-person-from-sfdc-3.png)

   Nach Ausführung des Flussschritts ist Ihre Person kein Lead mehr in [!DNL Salesforce], sondern verbleibt in Marketo.

   >[!CAUTION]
   >
   >Wenn Sie **[!UICONTROL Löschen in Marketo]** auf **[!UICONTROL true]** setzen und die Personen aus Marketo und die Leads aus Salesforce löschen, sind diese unwiederbringlich verloren. Das kann nicht rückgängig gemacht werden.
