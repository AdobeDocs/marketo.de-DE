---
unique-page-id: 557316
description: Erfahren Sie, wie Sie Smart-List-Filter definieren. Legen Sie Filterbegrenzungen und -werte fest, um zu bestimmen, wer in der Liste angezeigt wird.
title: Definieren von Filtern für eine Smart List
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
TQID: 'https://experienceleague.adobe.com/gCJT14FtnJaPAMhDUWI7XpoST1lc9yvzZbVKq-oTx-w'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
    internal-label: Smart lists
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 6%
---
# Definieren von Filtern für eine Smart List {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Erstellen einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Suchen und Hinzufügen von Filtern zu Smart-Listen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

Nachdem Sie nun [Smart-Liste erstellt](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} und [Filter hinzugefügt](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"} definiert haben, definieren Sie die Filter wie folgt.

Wenn Sie dieses Beispiel fortsetzen, definieren Sie diese Filter, um alle Personen in Kalifornien mit einem Ergebnis über 50 zu finden.

1. Navigieren Sie zu **[!UICONTROL Marketing-Aktivitäten]**.

   ![](assets/define-smart-list-filters-1.png)

1. Wählen Sie die gewünschte Smart-Liste aus und klicken Sie auf **[!UICONTROL Registerkarte]** Smart-Liste“.

   ![](assets/define-smart-list-filters-2.png)

1. Suchen Sie nach „CA“ für den Filter **[!UICONTROL State]** und wählen Sie es aus.

   ![](assets/define-smart-list-filters-3.png)

   >[!NOTE]
   >
   >Möglicherweise lagern Sie sowohl „Kalifornien“ als auch „CA“. Um nach beiden Werten zu filtern und _alle)_ aus Kalifornien einzuschließen, erfahren Sie, wie Sie [mehrere Werte zu einem Smart-Listen-Filter hinzufügen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"}.

1. Wählen Sie den **[!UICONTROL größer als]** und geben Sie „50“ ein.

   ![](assets/define-smart-list-filters-4.png)

>[!TIP]
>
>Wenn Sie der Meinung sind, dass Ihre Datenbank Datensätze enthalten könnte, die unvollständige E-Mail-Adressen enthalten (z. B. nur &quot;@adobe.com„), verwenden Sie zwei E-Mail-Adressfilter, wenn Sie den Operator „enthält“ verwenden. Ein Filter mit „enthält @adobe.com&quot; und ein separater Filter mit „enthält adobe.com“ (ohne das @-Symbol).

Jetzt wissen Sie, wie Sie eine Smart List erstellen und Filter hinzufügen/definieren.
