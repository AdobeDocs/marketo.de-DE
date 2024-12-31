---
unique-page-id: 2949413
description: Hinzufügen einer Einschränkung zu einem Smart-Listenfilter - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen einer Einschränkung zu einem Smart-Listen-Filter
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
source-git-commit: ac7d6b222ca561c88e0bf10aba7736c1b2eee3f7
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---

# Hinzufügen einer Einschränkung zu einem Smart-Listen-Filter {#add-a-constraint-to-a-smart-list-filter}

Beim Erstellen einer Smart-Liste verfügen einige Filter über erweiterte Optionen, die als „Einschränkungen“ bezeichnet werden. Dies sind zusätzliche Bedingungen, die Sie zu Filtern und Triggern hinzufügen können, um Ihre Suche weiter einzugrenzen.

In diesem Beispiel fügen wir einige Einschränkungen zu einem Filter **[Datenwert geändert“ hinzu](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}** um Personen zu finden, deren Status von MQL in SQL geändert wurde.

>[!PREREQUISITES]
>
>* [Erstellen einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Verwenden des Filters „Datenwert geändert“ in einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md){target="_blank"}

1. Navigieren Sie **[!UICONTROL Marketing-Aktivitäten]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-1.png)

1. Wählen Sie die Smart-Liste mit einem Filter aus, dem Sie eine Einschränkung hinzufügen möchten, und klicken Sie auf die Registerkarte **[!UICONTROL Smart-Liste]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-2.png)

1. Wählen **[!UICONTROL unter &quot;]** hinzufügen“ **[!UICONTROL Vorheriger Wert]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-3.png)

1. Geben Sie den **[!UICONTROL vorherigen Wert]** ein. In diesem Beispiel verwenden wir SQL.

   ![](assets/add-a-constraint-to-a-smart-list-filter-4.png)

1. Wählen **[!UICONTROL unter &quot;]** hinzufügen“ **[!UICONTROL Neuer Wert]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-5.png)

1. Geben Sie den neuen Wert ein. In diesem Beispiel verwenden wir SQL.

   ![](assets/add-a-constraint-to-a-smart-list-filter-6.png)

1. Gut gemacht! Klicken Sie auf **[!UICONTROL Personen]**, um alle Personen anzuzeigen, deren Status in den letzten 30 Tagen von „MQL“ in „SQL“ geändert wurde.
