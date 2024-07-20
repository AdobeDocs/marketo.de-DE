---
unique-page-id: 2949413
description: Eine Beschränkung zu einem Smart-List-Filter hinzufügen - Marketo Docs - Produktdokumentation
title: Eine Beschränkung zu einem Smart-Listenfilter hinzufügen
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
source-git-commit: ac7d6b222ca561c88e0bf10aba7736c1b2eee3f7
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---

# Eine Beschränkung zu einem Smart-Listenfilter hinzufügen {#add-a-constraint-to-a-smart-list-filter}

Beim Erstellen einer Smart-Liste verfügen einige Filter über erweiterte Optionen, die als &quot;Begrenzungen&quot;bezeichnet werden. Dies sind zusätzliche Bedingungen, die Sie zu Filtern und Triggern hinzufügen können, um Ihre Suche noch weiter einzugrenzen.

In diesem Beispiel fügen wir Einschränkungen zu einem Filter **[Datenwert geändert](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}** hinzu, um Personen zu finden, die einen Status-Wechsel von MQL zu SQL hatten.

>[!PREREQUISITES]
>
>* [Erstellen einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Verwenden des Filters &quot;Datenwert geändert&quot;in einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md){target="_blank"}

1. Wechseln Sie zu **[!UICONTROL Marketingaktivitäten]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-1.png)

1. Wählen Sie die Smart-Liste mit einem Filter aus, dem Sie eine Einschränkung hinzufügen, und klicken Sie auf die Registerkarte **[!UICONTROL Smart-Liste]** .

   ![](assets/add-a-constraint-to-a-smart-list-filter-2.png)

1. Wählen Sie unter **[!UICONTROL Beschränkung hinzufügen]** die Option **[!UICONTROL Vorheriger Wert]**.

   ![](assets/add-a-constraint-to-a-smart-list-filter-3.png)

1. Geben Sie den **[!UICONTROL vorherigen Wert]** ein. In diesem Beispiel verwenden wir MQL.

   ![](assets/add-a-constraint-to-a-smart-list-filter-4.png)

1. Wählen Sie unter **[!UICONTROL Beschränkung hinzufügen]** die Option **[!UICONTROL Neuer Wert]** aus.

   ![](assets/add-a-constraint-to-a-smart-list-filter-5.png)

1. Geben Sie den neuen Wert ein. In diesem Beispiel verwenden wir SQL.

   ![](assets/add-a-constraint-to-a-smart-list-filter-6.png)

1. Schön gemacht! Klicken Sie auf die Registerkarte **[!UICONTROL Personen]** , um alle Personen anzuzeigen, die in den letzten 30 Tagen eine Statusänderung von &quot;MQL&quot;zu &quot;SQL&quot;hatten.
