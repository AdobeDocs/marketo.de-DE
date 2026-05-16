---
unique-page-id: 1147001
description: Erfahren Sie, wie Sie die standardmäßige Regellogik der Smart List in einer Smart-Kampagne verwenden. Filter mit UND-Logik zur Qualifizierung kombinieren.
title: Verwenden der standardmäßigen Regellogik für intelligente Listen
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/hRPdzjEUOeC2PZK2YlO1IPZOPoPOfo7CHJu2yUtU0qc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 138
ht-degree: 10%

---

# Verwenden der standardmäßigen Regellogik für intelligente Listen {#using-standard-smart-list-rule-logic}

Ihnen ist möglicherweise die Option „Filter verwenden“ beim Erstellen von Smart Lists für Kampagnen aufgefallen. Mit dieser Einstellung können Sie entscheiden, ob die Filter mit einem AND- oder einem OR-Operator ausgewertet werden müssen.

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>Das Ändern der Regellogik der Smart List gilt nur für Filter, _nicht für_.

Trigger werden immer als ODER ausgewertet, selbst wenn die obige Einstellung auf ALL festgelegt ist. Beispiel:

![](assets/using-standard-smart-list-rule-logic-2.png)

Die obige Smart-Liste in Worten:

```box
IF person fills out Great Form
OR
IF person visits Keith's Landing Page
AND
Industry is Energy
AND
Country is US
THEN follow the campaign's flow step(s)
```

Wenn also eine Person das Formular ausfüllt _oder_ die Seite besucht, bewertet die Kampagne diese Person basierend auf _allen_ oder __ nachfolgenden Filtern, je nach der verwendeten Einstellung.

>[!MORELIKETHIS]
>
>[Verwenden der erweiterten Regellogik für Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"}
