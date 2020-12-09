---
unique-page-id: 1147001
description: Verwenden der Standard-Regellogik für intelligente Listen - Marketing-Dokumente - Produktdokumentation
title: Verwenden der Standard-Logik für intelligente Listen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# Verwenden der Standard-Logik für intelligente Listen {#using-standard-smart-list-rule-logic}

Möglicherweise haben Sie die Option &quot;Filter verwenden&quot;beim Erstellen von intelligenten Listen für Kampagnen bemerkt. Mit dieser Einstellung können Sie entscheiden, ob die Filter mit einem UND- oder ODER-Operator ausgewertet werden müssen.

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>Das Ändern der Regellogik für intelligente Listen gilt nur für Filter, **nicht** für Auslöser.

Auslöser werden immer als ODER ausgewertet, selbst wenn die oben angegebene Einstellung auf ALL eingestellt ist.  Hier ein Beispiel:

![](assets/image2014-9-22-14-3a12-3a57.png)

Die oben genannte intelligente Liste in Worten:
`<pre data-theme="Confluence">IF person fills out My Form OR IF person visits My Page AND Industry is Marketing AND Country is USA THEN follow the campaign's flow step(s)</pre>` Wenn eine Person also das Formular ausfüllt **oder** die Seite besucht, bewertet die Kampagne diese Person anhand der **alle **oder **alle **der nachfolgenden Filter, je nach verwendeter Einstellung.

>[!MORELIKETHIS]
>
>* [Erweiterte Logik der Smart-Liste](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)

>



