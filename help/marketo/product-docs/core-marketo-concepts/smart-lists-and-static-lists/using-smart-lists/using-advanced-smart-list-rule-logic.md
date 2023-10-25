---
unique-page-id: 1146901
description: Verwenden der erweiterten Smart-List-Regellogik - Marketo-Dokumente - Produktdokumentation
title: Verwenden der erweiterten Smart-List-Regellogik
exl-id: fc41b6fd-c65e-4c44-b0ee-7bb5c77c51fb
feature: Smart Lists
source-git-commit: 8a5903fa5313e34f448f833f20ab8e3624cf23e6
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Verwenden der erweiterten Smart-List-Regellogik {#using-advanced-smart-list-rule-logic}

Sie können genau die Personen finden, die Sie benötigen, indem Sie die Regellogik für intelligente Listen auf mehrere Filter in einer Smart-Liste anwenden. So geht es.

>[!PREREQUISITES]
>
>* [Suchen und Hinzufügen von Filtern zu einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}
>* [Definieren von Smart-List-Filtern](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md){target="_blank"}

>[!NOTE]
>
>Erweiterte Filterlogik ist nur verfügbar, wenn Ihre Smart-Liste mindestens drei Filter enthält.

## Hinzufügen einer Logik zu einer Smart-Liste {#add-logic-to-a-smart-list}

Standardmäßig findet Ihre Smart-Liste die Personen, die **[!UICONTROL ALL]** Filter (Filter 1 _und_ 2 _und_ 3). Sie können die Regellogik ändern, um passende Personen zu finden **[!UICONTROL ANDERE]** der Filter 1 _oder_ 2 _oder_ 3) oder erweiterte Filter verwenden (Filter 1) _und_ 2 _oder_ 3).

Nehmen wir an, Sie möchten Menschen in Kalifornien finden _und_ mit einer Punktzahl von mindestens 50 Punkten _oder_ mit dem Status &quot;Sales Qualified&quot;.

1. Auswählen **[!UICONTROL Erweiterte Filter verwenden]** aus der Dropdown-Liste aus.

   ![](assets/one.png)

   >[!NOTE]
   >
   >Verwenden **[!UICONTROL Erweitert]** -Filter verringern die Notwendigkeit, Smart-Listen mit dem Filter Mitglied der Smart-Liste zu erstellen. Dies trägt zur Leistungsoptimierung bei.

1. Die **[!UICONTROL Erweiterte Filter]** im Textfeld wird &quot;und&quot;als Standardwert zwischen allen Filtern angezeigt.

   ![](assets/two-2.png)

1. Geben Sie ein Paar Klammern um &quot;2 und 3&quot;ein.

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >Sie müssen beim Eingeben der Regellogik &quot;und&quot;vor &quot;oder&quot;verwenden.

1. Ändern Sie das &quot;und&quot;zwischen &quot;2 und 3&quot;in &quot;oder&quot;.

   ![](assets/four-1.png)

## Verwenden Sie beim Mischen von &quot;Und&quot;und &quot;Oder&quot;Klammern {#use-parentheses-when-mixing-and-and-or}

Das Mischen der Logik &quot;und&quot;und &quot;Oder&quot;erfordert Klammern, um Ihre Absicht klar zu machen.

![](assets/advancedfilters-parent.png)

## Verwenden Sie verschachtelte Klammern für vier oder mehr Filter, falls erforderlich {#use-nested-parentheses-for-four-or-more-filters-if-needed}

Abhängig von Ihrer Absicht müssen Sie möglicherweise verschachtelte Klammern hinzufügen, wenn Sie vier oder mehr Filter verwenden.

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>Wenn Sie eine ungültige Regel eingeben, wird unter der Regel eine rote Linie angezeigt. Scrollen Sie über den Text, um die zugehörige Fehlermeldung anzuzeigen.
