---
unique-page-id: 1147001
description: Verwenden von Standard-Regellogik für intelligente Liste - Marketo Docs - Produktdokumentation
title: Verwenden der Standard-Logik für intelligente Listen
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Verwenden der standardmäßigen Regel-Logik für intelligente Listen {#using-standard-smart-list-rule-logic}

Möglicherweise haben Sie die Option &quot;Filter verwenden&quot;beim Erstellen von intelligenten Listen für Kampagnen bemerkt. Mit dieser Einstellung können Sie entscheiden, ob die Filter mit einem UND- oder ODER-Operator ausgewertet werden müssen.

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>Das Ändern der Regellogik für intelligente Listen gilt nur für Filter, **nicht**-Trigger.

Trigger werden immer als ODER ausgewertet, selbst wenn die oben angegebene Einstellung auf ALL eingestellt ist.  Hier ein Beispiel:

![](assets/image2014-9-22-14-3a12-3a57.png)

Die oben genannte intelligente Liste in Worten:

```box
IF person fills out My Form
OR
IF person visits My Page 
AND 
Industry is Marketing 
AND 
Country is USA 
THEN follow the campaign's flow step(s)
```

Wenn eine Person also das Formular **oder** ausfüllt, wird diese Kampagne anhand der **alle** oder **alle** der nachfolgenden Filter auswerten, je nach verwendeter Einstellung.

>[!MORELIKETHIS]
>
>[Erweiterte Logik der Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
