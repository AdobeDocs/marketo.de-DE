---
unique-page-id: 1146901
description: Verwenden der erweiterten Smart-List-Regellogik - Marketo-Dokumente - Produktdokumentation
title: Verwenden der erweiterten Regellogik für Smart List
exl-id: fc41b6fd-c65e-4c44-b0ee-7bb5c77c51fb
feature: Smart Lists
source-git-commit: d087b22e84c23fea5e38fe7bf20349dc7eec09f7
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Verwenden der erweiterten Regellogik für Smart List {#using-advanced-smart-list-rule-logic}

Sie können genau die Personen finden, die Sie benötigen, indem Sie die Regellogik der Smart-Liste auf mehrere Filter in einer Smart-Liste anwenden. So geht&#39;s.

>[!PREREQUISITES]
>
>* [Filter suchen und zu einer Smart-Liste hinzufügen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}
>* [Definieren von Smart-Listen-Filtern](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md){target="_blank"}

>[!NOTE]
>
>Die erweiterte Filterlogik ist nur verfügbar, wenn in Ihrer Smart-Liste mindestens drei Filter vorhanden sind.

## Logik zu einer Smart-Liste hinzufügen {#add-logic-to-a-smart-list}

Standardmäßig findet Ihre Smart-Liste die Personen, die mit **[!UICONTROL ALL]**-Filtern übereinstimmen (Filter 1 _und_ 2 _und_ 3). Sie können die Regellogik ändern, um Personen zu finden, **[!UICONTROL „BELIEBIG]** der definierten Filter (Filter 1 _oder_ 2 _oder_ 3) entsprechen, oder erweiterte Filter verwenden (Filter 1 _und_ 2 _oder_ 3).

In diesem Beispiel möchten Sie beispielsweise Personen in Kalifornien _und_ mit einer Punktzahl von mindestens 50 Punkten _oder_ mit dem Status „Verkauf qualifiziert“ finden.

1. Wählen **[!UICONTROL Erweiterte Filter verwenden]** aus der Dropdownliste aus.

   ![](assets/using-advanced-smart-list-rule-logic-1.png)

   >[!NOTE]
   >
   >Die Verwendung **[!UICONTROL Erweiterter]** Filter reduziert die Notwendigkeit, Smart-Listen mit dem Mitglied des Smart-Listen-Filters zu erstellen. Dies trägt zur Leistungsoptimierung bei.

1. Das **[!UICONTROL Erweiterte Filter]**-Textfeld zeigt „und“ als Standardwert für alle Ihre Filter an.

   ![](assets/using-advanced-smart-list-rule-logic-2.png)

1. Geben Sie ein Paar Klammern um „2 und 3“ ein.

   ![](assets/using-advanced-smart-list-rule-logic-3.png)

   >[!CAUTION]
   >
   >Sie müssen bei der Eingabe von Regellogik „and“ vor „or“ verwenden.

1. Ändern Sie „and“ zwischen „2 und 3“ in „or“.

   ![](assets/using-advanced-smart-list-rule-logic-4.png)

## Verwenden Sie Klammern beim Mischen von „Und“ und „Oder“ {#use-parentheses-when-mixing-and-and-or}

Das Mischen der Logik „Und“ und „Oder“ erfordert Klammern, um Ihre Absicht klar zu machen.

![](assets/using-advanced-smart-list-rule-logic-5.png)

## Verwenden Sie bei Bedarf verschachtelte Klammern für vier oder mehr Filter {#use-nested-parentheses-for-four-or-more-filters-if-needed}

Abhängig von Ihrer Absicht müssen Sie möglicherweise verschachtelte Klammern hinzufügen, wenn Sie vier oder mehr Filter verwenden.

![](assets/using-advanced-smart-list-rule-logic-6.png)

>[!TIP]
>
>Wenn Sie eine ungültige Regel eingeben, wird unter der Regel eine rote Linie angezeigt. Scrollen Sie über den Text, um die entsprechende Fehlermeldung anzuzeigen.
