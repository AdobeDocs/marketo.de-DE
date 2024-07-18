---
unique-page-id: 557316
description: Definieren von Smart-List-Filtern - Marketo-Dokumente - Produktdokumentation
title: Definieren von Smart-List-Filtern
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 4bf27f7eb534ec76983a898d020f0b8c336a36dc
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# Definieren von Smart-List-Filtern {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Erstellen einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Filter zu Smart-Listen suchen und hinzufügen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

Nachdem Sie [eine Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} erstellt und [Filter](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"} hinzugefügt haben, legen wir die Filter fest. So geht es.

Lassen Sie uns in unserem Beispiel diese Filter definieren, um alle Menschen in Kalifornien mit einer Punktzahl über 50 zu finden.

1. Wechseln Sie zu **[!UICONTROL Marketingaktivitäten]**.

   ![](assets/define-smart-list-filters-1.png)

1. Wählen Sie die gewünschte Smart-Liste aus und klicken Sie auf die Registerkarte **[!UICONTROL Smart-Liste]** .

   ![](assets/define-smart-list-filters-2.png)

1. Suchen und wählen Sie &quot;CA&quot;für den Filter **[!UICONTROL Status]** aus.

   ![](assets/define-smart-list-filters-3.png)

   >[!NOTE]
   >
   >Möglicherweise speichern Sie sowohl &quot;Kalifornien&quot;als auch &quot;CA&quot;. Um nach beiden Werten zu filtern und _alle_ Personen aus Kalifornien einzubeziehen, erfahren Sie, wie Sie [mehrere Werte zu einem Smart-List-Filter hinzufügen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"}.

1. Wählen Sie den Operator **[!UICONTROL größer als]** aus und geben Sie &quot;50&quot;ein.

   ![](assets/define-smart-list-filters-4.png)

>[!TIP]
>
>Wenn Sie glauben, dass Ihre Datenbank Datensätze enthält, die unvollständige E-Mail-Adressen enthalten (z. B. &quot;@adobe.com&quot;), verwenden Sie bei Verwendung des Operators &quot;enthält&quot; zwei Filter für E-Mail-Adressen. Ein Filter mit &quot;enthält @adobe.com&quot;und ein separater Filter mit &quot;enthält adobe.com&quot;(ohne das @-Symbol).

Jetzt wissen Sie, wie Sie eine Smart-Liste erstellen und Filter hinzufügen/definieren.
