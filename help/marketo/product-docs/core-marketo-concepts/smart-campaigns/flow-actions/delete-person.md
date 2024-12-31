---
unique-page-id: 1147082
description: Person löschen - Marketo-Dokumente - Produktdokumentation
title: Person löschen
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 3%

---

# Person löschen {#delete-person}

Fehlerhafte Personen gelangen manchmal in Ihre Datenbank. Mit dem Schritt „Personenfluss löschen“ können Sie diese entfernen.

![](assets/delete-person-1.png)

>[!CAUTION]
>
>Wenn Sie eine Person löschen, werden auch alle ihre historischen RCE-Daten gelöscht. Das kann nicht rückgängig gemacht werden.

1. Wenn Sie im Flussschritt ziehen, wird er automatisch auch auf Aus Ihrem CRM löschen eingestellt.

   ![](assets/delete-person-2.png)

1. Sie können wie folgt von der Marketo Engage und nicht aus Ihrem CRM löschen:

   ![](assets/delete-person-3.png)

>[!NOTE]
>
>Das Entfernen der Person aus Ihrem CRM _funktioniert nur mit[!DNL Salesforce]_. Wenn Sie eine Person aus Marketo löschen und in [!DNL Salesforce] lassen, wird sie in Marketo neu erstellt, sobald ihr [!DNL Salesforce]-Eintrag aktualisiert wird.
