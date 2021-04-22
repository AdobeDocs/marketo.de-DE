---
unique-page-id: 1147031
description: Personen aus dem SFDC löschen - Marketo Docs - Produktdokumentation
title: Person aus SFDC löschen
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 5%

---

# Person aus SFDC löschen {#delete-person-from-sfdc}

Wenn Sie einen bestimmten Satz von Interessenten aus Salesforce entfernen, diese jedoch als Personen in Marketo belassen müssen, können Sie die Flusshandlung &quot;Person aus SFDC löschen&quot;verwenden.

>[!NOTE]
>
>Nur verfügbar, wenn in Salesforce integriert.

1. Klicken Sie in der Datenbank auf die Person, die Sie aus Salesforce entfernen möchten. Klicken Sie dann auf **Benutzeraktionen** und wählen Sie **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. Wählen Sie **Person aus dem SFDC** löschen.

   ![](assets/delete-person-from-sfdc.png)

1. Vergewissern Sie sich, dass die Einstellung **Löschen in Marketo** **false** lautet, und klicken Sie dann auf **Jetzt ausführen**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   Nachdem der Flussschritt ausgeführt wurde, wird Ihre Person nicht mehr eine Führungsrolle in Salesforce übernehmen, sondern in Marketo bleiben.

   >[!CAUTION]
   >
   >Wenn Sie **Löschen in Marketo** auf **true** setzen und die Personen aus Marketo und die Interessenten aus Salesforce löschen, sind sie für immer weg. Das kann nicht rückgängig gemacht werden.
