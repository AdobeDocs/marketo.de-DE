---
unique-page-id: 2949413
description: Eine Beschränkung zu einem Smart-List-Filter hinzufügen - Marketo Docs - Produktdokumentation
title: Eine Beschränkung zu einem Smart-Listenfilter hinzufügen
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Eine Beschränkung zu einem Smart-Listenfilter hinzufügen {#add-a-constraint-to-a-smart-list-filter}

Beim Erstellen von Smart-Listen verfügen einige Filter über erweiterte Optionen, die als &quot;Begrenzungen&quot;bezeichnet werden. Dies sind zusätzliche Bedingungen, die Sie zu Filtern und Triggern hinzufügen können, um Ihre Suche noch weiter einzugrenzen.

Fügen wir in diesem Beispiel Einschränkungen zu einem **[Datenwert geändert](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)** nach Personen suchen, die einen Status-Wechsel von MQL zu SQL hatten.

>[!PREREQUISITES]
>
>* [Erstellen einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [Verwenden des Filters &quot;Datenwert geändert&quot;in einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md)
>

1. Navigieren Sie zu **Marketingaktivitäten**.

   ![](assets/ma-1.png)

1. Wählen Sie die Smart-Liste mit einem Filter aus, dem Sie eine Einschränkung hinzufügen möchten, und klicken Sie auf die **Smart List** Registerkarte.

   ![](assets/two-3.png)

1. under **Beschränkung hinzufügen** auswählen **Vorheriger Wert**.

   ![](assets/three-3.png)

1. Geben Sie die **Vorheriger Wert**. In diesem Beispiel verwenden wir MQL.

   ![](assets/four-2.png)

1. under **Beschränkung hinzufügen** auswählen **Neuer Wert**.

   ![](assets/five.png)

1. Geben Sie die **Neuer Wert**. In diesem Beispiel verwenden wir SQL.

   ![](assets/six.png)

1. Schön gemacht! Klicken Sie auf **Personen** Registerkarte, um alle Personen anzuzeigen, die eine **Status** ändern von **MQL** nach **SQL** in den letzten 30 Tagen.
