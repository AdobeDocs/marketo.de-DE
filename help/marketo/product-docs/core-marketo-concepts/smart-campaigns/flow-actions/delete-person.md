---
unique-page-id: 1147082
description: Person löschen - Marketo Docs - Produktdokumentation
title: Person löschen
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 3%

---

# Person löschen {#delete-person}

Fehlerhafte Personen gelangen manchmal in Ihre Datenbank. Der Schritt zum Löschen von Personen kann sie entfernen.

![](assets/delete-person-1.png)

>[!CAUTION]
>
>Wenn Sie eine Person löschen, werden auch alle historischen RCE-Daten gelöscht. Sie kann nicht rückgängig gemacht werden.

1. Wenn Sie in den Flussschritt ziehen, wird automatisch auch der Löschvorgang aus Ihrem CRM-System eingestellt.

   ![](assets/delete-person-2.png)

1. Sie können aus der Marketo Engage löschen und nicht aus Ihrem CRM-System wie folgt:

   ![](assets/delete-person-3.png)

>[!NOTE]
>
>Wenn Sie die Person aus Ihrem CRM entfernen, funktioniert _nur mit[!DNL Salesforce]_. Wenn Sie eine Person aus Marketo löschen und diese in [!DNL Salesforce] belassen, wird sie in Marketo neu erstellt, wenn ihr [!DNL Salesforce] -Datensatz jemals aktualisiert wird.
