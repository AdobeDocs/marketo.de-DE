---
unique-page-id: 1147001
description: Verwenden der standardmäßigen Smart-List-Regellogik - Marketo-Dokumente - Produktdokumentation
title: Verwenden der standardmäßigen Smart-List-Regellogik
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Verwenden der standardmäßigen Smart-List-Regellogik {#using-standard-smart-list-rule-logic}

Möglicherweise haben Sie beim Erstellen von Smart-Listen für Kampagnen die Option &quot;Filter verwenden&quot;bemerkt. Mit dieser Einstellung können Sie entscheiden, ob die Filter mit einem AND- oder OR-Operator bewertet werden müssen.

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>Das Ändern der Logik von Smart-List-Regeln gilt nur für Filter, nicht für __ Trigger.

Trigger werden immer als ODER ausgewertet, selbst wenn die obige Einstellung auf ALLE gesetzt ist. Im Folgenden finden Sie ein Beispiel:

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

Wenn also eine Person das Formular _oder_ ausfüllt, die Seite besucht, wird diese Person von der Kampagne anhand der verwendeten Einstellung anhand von _all_ oder _any_ der nachfolgenden Filter ausgewertet.

>[!MORELIKETHIS]
>
>[Verwenden der erweiterten Smart-List-Regellogik](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"}
