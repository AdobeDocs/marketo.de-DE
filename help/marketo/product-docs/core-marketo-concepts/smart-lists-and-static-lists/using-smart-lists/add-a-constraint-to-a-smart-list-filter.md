---
unique-page-id: 2949413
description: hinzufügen einer Beschränkung auf einen Filter für intelligente Listen - Marketing Docs - Produktdokumentation
title: hinzufügen einer Beschränkung auf einen Filter für intelligente Listen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---


# hinzufügen einer Beschränkung auf einen Filter für intelligente Listen {#add-a-constraint-to-a-smart-list-filter}

Beim Erstellen intelligenter Listen verfügen einige Filter über erweiterte Optionen, die als *einschränkungen bezeichnet werden. *Dies sind zusätzliche Bedingungen, die Sie zu Filtern und Auslösern hinzufügen können, um Ihre Suche noch weiter einzuschränken.

In diesem Beispiel sollten wir einem ** [Datenwert geändert](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)**-Filter einige Einschränkungen hinzufügen, um nach Personen zu suchen, die eine Statusänderung von MQL in SQL hatten.

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!PREREQUISITES]
>
>* [Erstellen einer intelligenten Liste](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [Verwenden Sie den Filter &quot;Datenwert geändert&quot;in einer intelligenten Liste](use-the-data-value-changed-filter-in-a-smart-list.md)

>



1. Gehen Sie zu **Marketing-Aktivitäten**.

   ![](assets/ma-1.png)

1. Wählen Sie die intelligente Liste mit einem Filter aus, dem Sie eine Beschränkung hinzufügen möchten, und klicken Sie auf die Registerkarte &quot; **Intelligente Liste** &quot;.

   ![](assets/two-3.png)

1. Wählen Sie unter **Hinzufügen Einschränkung** die Option **Vorheriger Wert**.

   ![](assets/three-3.png)

1. Geben Sie den **vorherigen Wert** ein. In diesem Beispiel verwenden wir MQL.

   ![](assets/four-2.png)

1. Wählen Sie unter **Hinzufügen Einschränkung** die Option **Neuer Wert**.

   ![](assets/five.png)

1. Geben Sie den **neuen Wert** ein. In diesem Beispiel verwenden wir SQL.

   ![](assets/six.png)

1. Gut gemacht! Klicken Sie auf die Registerkarte **Personen** , um alle Personen anzuzeigen, die in den letzten 30 Tagen eine **Statusänderung** von **MQL** zu **SQL** vorgenommen haben.

