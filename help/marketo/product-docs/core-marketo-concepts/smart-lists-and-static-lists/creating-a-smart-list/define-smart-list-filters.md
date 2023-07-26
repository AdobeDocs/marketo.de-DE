---
unique-page-id: 557316
description: Definieren von Smart-List-Filtern - Marketo-Dokumente - Produktdokumentation
title: Definieren von Smart-List-Filtern
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Definieren von Smart-List-Filtern {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Erstellen einer Smart-Liste](create-a-smart-list.md)
>* [Suchen und Hinzufügen von Filtern zu Smart-Listen](find-and-add-filters-to-a-smart-list.md)

Jetzt, da du [eine Smart-Liste erstellt hat](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) und [hinzugefügte Filter](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md) definieren wir die Filter. So geht es.

Lassen Sie uns in unserem Beispiel diese Filter definieren, um alle Menschen in Kalifornien mit einer Punktzahl über 50 zu finden.

1. Navigieren Sie zu **Marketingaktivitäten**.

   ![](assets/login-marketing-activities-1.png)

1. Wählen Sie die Smart-Liste aus und klicken Sie auf die **Smart List** Registerkarte.

   ![](assets/smarlist-choosefilters.png)

1. Suchen und Auswählen **CA** für die **Bundesland** Filter.

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >Möglicherweise speichern Sie beide **Kalifornien** und **CA**. Um sowohl nach Werten als auch nach _all_ Menschen aus Kalifornien, lernen, wie  [Hinzufügen mehrerer Werte zu einem Smart-Listenfilter](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md).

1. Wählen Sie die **größer als** Operator und Eingabe **50**.

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>Wenn Sie glauben, dass Ihre Datenbank Datensätze enthält, die unvollständige E-Mail-Adressen enthalten (z. B. &quot;@adobe.com&quot;), verwenden Sie **two** Filter für E-Mail-Adressen, wenn Sie den Operator &quot;enthält&quot;verwenden. Ein Filter mit &quot;enthält @adobe.com&quot;und ein separater Filter mit &quot;enthält adobe.com&quot;(ohne das @-Symbol).

Jetzt wissen Sie, wie Sie eine Smart-Liste erstellen und Filter hinzufügen/definieren.
