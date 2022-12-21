---
unique-page-id: 1147082
description: Person löschen - Marketo Docs - Produktdokumentation
title: Person löschen
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 4%

---

# Person löschen {#delete-person}

Fehlerhafte Personen werden manchmal in Ihre Datenbank aufgenommen. Der Schritt zum Löschen von Personen kann sie entfernen.

## Überblick {#overview}

Verwenden Sie den Flussschritt in einer intelligenten Kampagne.

![](assets/one-4.png)

>[!CAUTION]
>
>Wenn Sie eine Person löschen, werden auch alle historischen RCE-Daten gelöscht. Sie kann nicht rückgängig gemacht werden.

## Nutzung {#usage}

Wenn Sie in den Flussschritt ziehen, wird automatisch auch der Löschvorgang aus Ihrem CRM-System eingestellt.

![](assets/two-4.png)

Sie können aus Marketo und nicht aus Ihrem CRM-System löschen, z. B.:

![](assets/three-3.png)

>[!NOTE]
>
>Person aus Ihrem CRM entfernen **funktioniert nur mit Salesforce**. Wenn Sie eine Person aus Marketo löschen und sie in Salesforce behalten möchten, werden sie in Marketo neu erstellt, wenn ihr Salesforce-Datensatz jemals aktualisiert wird.
