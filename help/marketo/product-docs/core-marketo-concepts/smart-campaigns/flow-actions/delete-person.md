---
unique-page-id: 1147082
description: Person löschen - Marketo Docs - Produktdokumentation
title: Person löschen
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 4%

---

# Person löschen {#delete-person}

Fehlerhafte Personen gelangen manchmal in Ihre Datenbank. Der Schritt zum Löschen von Personen kann sie entfernen.

## Überblick {#overview}

Verwenden Sie den Flussschritt in einer Smart-Kampagne.

![](assets/one-4.png)

>[!CAUTION]
>
>Wenn Sie eine Person löschen, werden auch alle historischen RCE-Daten gelöscht. Sie kann nicht rückgängig gemacht werden.

## Nutzung {#usage}

Wenn Sie in den Flussschritt ziehen, wird automatisch auch der Löschvorgang aus Ihrem CRM-System eingestellt.

![](assets/two-4.png)

Sie können aus der Marketo Engage löschen und nicht aus Ihrem CRM-System wie folgt:

![](assets/three-3.png)

>[!NOTE]
>
>Person aus Ihrem CRM entfernen _funktioniert nur mit[!DNL Salesforce]_. Wenn Sie eine Person aus Marketo löschen und sie beibehalten [!DNL Salesforce], werden sie in Marketo neu erstellt, wenn ihre [!DNL Salesforce] wird immer aktualisiert.
