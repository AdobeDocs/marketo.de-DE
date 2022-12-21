---
unique-page-id: 1147001
description: Verwenden der standardmäßigen Smart-List-Regellogik - Marketo-Dokumente - Produktdokumentation
title: Verwenden der standardmäßigen Smart-List-Regellogik
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Verwenden der standardmäßigen Smart-List-Regellogik {#using-standard-smart-list-rule-logic}

Möglicherweise haben Sie beim Erstellen von Kampagnen-Smart-Listen die Option &quot;Filter verwenden&quot;bemerkt. Mit dieser Einstellung können Sie entscheiden, ob die Filter mit einem AND- oder OR-Operator bewertet werden müssen.

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>Das Ändern der Logik von Smart-List-Regeln gilt nur für Filter. **not** Trigger.

Trigger werden immer als ODER ausgewertet, selbst wenn die obige Einstellung auf ALLE gesetzt ist.  Im Folgenden finden Sie ein Beispiel:

![](assets/image2014-9-22-14-3a12-3a57.png)

Die obige intelligente Liste in Worten:

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

Wenn also eine Person das Formular ausfüllt **oder** besucht die Seite und die Kampagne bewertet diese Person anhand **all** oder **any** der nachfolgenden Filter, je nach verwendeter Einstellung.

>[!MORELIKETHIS]
>
>[Verwenden der erweiterten Smart-List-Regellogik](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)
