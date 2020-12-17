---
unique-page-id: 1147001
description: Verwenden der Standard-Regellogik für intelligente Listen - Marketing-Dokumente - Produktdokumentation
title: Verwenden der Standard-Logik für intelligente Listen
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---


# Verwenden der standardmäßigen Regel-Logik für intelligente Listen {#using-standard-smart-list-rule-logic}

Möglicherweise haben Sie die Option &quot;Filter verwenden&quot;beim Erstellen von intelligenten Listen für Kampagnen bemerkt. Mit dieser Einstellung können Sie entscheiden, ob die Filter mit einem UND- oder ODER-Operator ausgewertet werden müssen.

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>Das Ändern der Regellogik für intelligente Listen gilt nur für Filter, die nicht **auslösen.**

Auslöser werden immer als ODER ausgewertet, selbst wenn die oben angegebene Einstellung auf ALL eingestellt ist.  Hier ein Beispiel:

![](assets/image2014-9-22-14-3a12-3a57.png)

Die oben genannte intelligente Liste in Worten:
`<pre data-theme="Confluence">IF person fills out My Form OR IF person visits My Page AND Industry is Marketing AND Country is USA THEN follow the campaign's flow step(s)</pre>` Wenn also eine Person das Formular **oder** ausfüllt, wird diese Kampagne anhand von **alle **oder **beliebige **der nachfolgenden Filter ausgewertet, je nach verwendeter Einstellung.

>[!MORELIKETHIS]
>
>* [Erweiterte Logik der Smart-Liste](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)

>



