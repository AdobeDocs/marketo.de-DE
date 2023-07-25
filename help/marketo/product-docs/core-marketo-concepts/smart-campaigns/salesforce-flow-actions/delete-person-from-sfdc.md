---
unique-page-id: 1147031
description: Person aus SFDC löschen - Marketo Docs - Produktdokumentation
title: Person aus SFDC löschen
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 5%

---

# Person aus SFDC löschen {#delete-person-from-sfdc}

Wenn Sie einen bestimmten Satz von Leads aus Salesforce entfernen müssen, diese jedoch als Personen in Marketo belassen möchten, können Sie die Flusshandlung Person aus SFDC löschen verwenden.

>[!NOTE]
>
>Nur verfügbar bei Integration mit Salesforce.

1. Klicken Sie in der Datenbank auf die Person, die Sie aus Salesforce entfernen möchten. Klicken Sie anschließend auf **Personenaktionen** und wählen Sie **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. Auswählen **Person aus SFDC löschen**.

   ![](assets/delete-person-from-sfdc.png)

1. Stellen Sie sicher, dass **Löschen in Marketo** Einstellung ist **false** Klicken Sie auf **Jetzt ausführen**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   Nachdem der Flussschritt ausgeführt wurde, wird Ihre Person nicht mehr in Salesforce als Lead fungieren, sondern in Marketo bleiben.

   >[!CAUTION]
   >
   >Wenn Sie **Löschen in Marketo** nach **true** und die Personen aus Marketo und die Leads aus Salesforce löschen, sind sie für immer verschwunden. Das kann nicht rückgängig gemacht werden.
