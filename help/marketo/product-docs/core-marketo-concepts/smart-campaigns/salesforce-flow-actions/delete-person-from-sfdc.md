---
unique-page-id: 1147031
description: Erfahren Sie, wie Sie mit einem Flussschritt eine Person aus Salesforce löschen. Entfernen Sie den Lead oder Kontakt aus SFDC, wenn er in den Fluss eintritt.
title: Löschen von Personen aus SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/f-Zvc4glfCtAagE314vrZjiWIcD3vaGIKmKGeZO18v0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 149
ht-degree: 5%

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
