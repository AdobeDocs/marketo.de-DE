---
unique-page-id: 1147031
description: Person aus dem SFDC löschen - Marketing Docs - Produktdokumentation
title: Person aus dem SFDC löschen
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---


# Person aus dem SFDC löschen {#delete-person-from-sfdc}

Wenn Sie einen bestimmten Satz von Interessenten aus Salesforce entfernen, diese jedoch als Personen in Marketo belassen müssen, können Sie die Flusshandlung &quot;Person aus SFDC löschen&quot;verwenden.

>[!NOTE]
>
>Nur verfügbar, wenn in Salesforce integriert.

1. Klicken Sie in der Datenbank auf die Person, die Sie aus Salesforce entfernen möchten. Klicken Sie dann auf **Benutzeraktionen** und wählen Sie **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. Wählen Sie **Person aus dem SFDC** löschen.

   ![](assets/delete-person-from-sfdc.png)

1. Vergewissern Sie sich, dass die Einstellung **In Marker löschen** **false** lautet, und klicken Sie dann auf **Jetzt ausführen**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   Nachdem der Flussschritt ausgeführt wurde, wird Ihre Person nicht mehr ein Lead in Salesforce sein, sondern in Marketo bleiben.

   >[!CAUTION]
   >
   >Wenn Sie **Löschen in Marketo** auf **true** setzen und die Personen aus Marketo und die Interessenten aus Salesforce löschen, sind sie für immer weg. Das kann nicht rückgängig gemacht werden.

