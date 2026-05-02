---
unique-page-id: 1147001
description: Erfahren Sie, wie Sie die standardmäßige Regellogik der Smart List in einer Smart-Kampagne verwenden. Filter mit UND-Logik zur Qualifizierung kombinieren.
title: Verwenden der standardmäßigen Regellogik für intelligente Listen
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 60c5603fa29bb1039b9d477633beb2c6f5c63486
workflow-type: tm+mt
source-wordcount: '138'
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
