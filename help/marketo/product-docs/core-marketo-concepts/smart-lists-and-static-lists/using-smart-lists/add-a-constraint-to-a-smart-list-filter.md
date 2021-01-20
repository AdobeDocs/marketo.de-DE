---
unique-page-id: 2949413
description: hinzufügen einer Beschränkung auf einen Filter für intelligente Listen - Marketing Docs - Produktdokumentation
title: hinzufügen einer Beschränkung auf einen Filter für intelligente Listen
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---


# hinzufügen einer Beschränkung auf einen Filter für intelligente Listen {#add-a-constraint-to-a-smart-list-filter}

Beim Erstellen intelligenter Listen verfügen einige Filter über erweiterte Optionen, die als &quot;Beschränkungen&quot;bezeichnet werden. Dies sind zusätzliche Bedingungen, die Sie Filtern und Triggern hinzufügen können, um Ihre Suche noch weiter einzuschränken.

In diesem Beispiel fügen wir dem Filter **[Datenwert geändert](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)** einige Einschränkungen hinzu, um nach Personen zu suchen, deren Status von MQL in SQL geändert wurde.

>[!PREREQUISITES]
>
>* [Erstellen einer intelligenten Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [Verwenden Sie den Filter &quot;Datenwert geändert&quot;in einer intelligenten Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md)

>



1. Gehen Sie zu **Marketing-Aktivitäten**.

   ![](assets/ma-1.png)

1. Wählen Sie die intelligente Liste mit einem Filter aus, dem Sie eine Beschränkung hinzufügen möchten, und klicken Sie auf die Registerkarte **Intelligente Liste**.

   ![](assets/two-3.png)

1. Wählen Sie unter **Hinzufügen Constraint** **Vorheriger Wert**.

   ![](assets/three-3.png)

1. Geben Sie den Wert **Vorheriger Wert** ein. In diesem Beispiel verwenden wir MQL.

   ![](assets/four-2.png)

1. Wählen Sie unter **Hinzufügen Constraint** **Neuer Wert**.

   ![](assets/five.png)

1. Geben Sie den Wert **Neuer Wert** ein. In diesem Beispiel verwenden wir SQL.

   ![](assets/six.png)

1. Gut gemacht! Klicken Sie auf die Registerkarte **Personen**, um alle Personen anzuzeigen, die in den letzten 30 Tagen einen Wechsel von **MQL** zu **SQL** hatten.****
