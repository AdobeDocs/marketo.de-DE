---
unique-page-id: 1147082
description: Person löschen - Marketo Dokumente - Produktdokumentation
title: Person löschen
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 4%

---

# Person löschen {#delete-person}

Fehlerhafte Personen werden manchmal in Ihre Datenbank aufgenommen. Der Schritt zum Löschen von Personen kann diese löschen.

## Übersicht {#overview}

Verwenden Sie den Flussschritt in einer intelligenten Kampagne.

![](assets/one-4.png)

>[!CAUTION]
>
>Wenn Sie eine Person löschen, werden auch alle ihre historischen RCE-Daten gelöscht. Sie kann nicht rückgängig gemacht werden.

## Nutzung {#usage}

Wenn Sie in den Flow-Schritt ziehen, wird es automatisch so eingestellt, dass es auch aus Ihrem CRM gelöscht wird.

![](assets/two-4.png)

So können Sie aus Marketo und nicht aus Ihrem CRM löschen:

![](assets/three-3.png)

>[!NOTE]
>
>Das Entfernen der Person aus Ihrem CRM **funktioniert nur mit Salesforce**. Wenn Sie eine Person aus Marketo löschen und sie in Salesforce behalten, werden sie in Marketo neu erstellt, wenn ihr Salesforce-Datensatz jemals aktualisiert wird.
