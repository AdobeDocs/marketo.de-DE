---
unique-page-id: 1147082
description: Erfahren Sie, wie Sie mit einem Flussschritt eine Person aus der Datenbank löschen. Personen, die die Kriterien erfüllen, aus Marketo entfernen.
title: Löschen von Person
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/89EPt9SVBCuluSojdqLE4BawaPGGbzHLSmYHV9w6Uko
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: c5f60233-d5ea-4453-a799-0ad258b4d399
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 127
ht-degree: 3%

---

# Löschen von Person {#delete-person}

Fehlerhafte Personen gelangen manchmal in Ihre Datenbank. Mit dem Schritt „Personenfluss löschen“ können Sie diese entfernen.

![](assets/delete-person-1.png)

>[!CAUTION]
>
>Wenn Sie eine Person löschen, werden auch alle ihre historischen RCE-Daten gelöscht. Das kann nicht rückgängig gemacht werden.

1. Wenn Sie im Flussschritt ziehen, wird er automatisch auch auf Aus Ihrem CRM löschen eingestellt.

   ![](assets/delete-person-2.png)

1. Sie können wie folgt aus Marketo Engage und nicht aus Ihrem CRM löschen:

   ![](assets/delete-person-3.png)

>[!NOTE]
>
>Das Entfernen der Person aus Ihrem CRM _funktioniert nur mit[!DNL Salesforce]_. Wenn Sie eine Person aus Marketo löschen und in [!DNL Salesforce] lassen, wird sie in Marketo neu erstellt, sobald ihr [!DNL Salesforce]-Eintrag aktualisiert wird.
