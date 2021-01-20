---
unique-page-id: 1146901
description: Verwenden der erweiterten Regellogik für intelligente Listen - Marketing Docs - Produktdokumentation
title: Erweiterte Logik der Smart-Liste
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# Verwenden der erweiterten Regellogik für intelligente Listen {#using-advanced-smart-list-rule-logic}

Sie können genau die Personen finden, die Sie benötigen, indem Sie innerhalb einer intelligenten Liste eine intelligente Liste-Regellogik auf mehrere Filter anwenden. So geht es.

>[!PREREQUISITES]
>
>* [Filter für eine intelligente Liste suchen und Hinzufügen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [Definieren von Filtern für intelligente Listen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)


>[!NOTE]
>
>Erweiterte Filterlogik ist nur verfügbar, wenn Ihre intelligente Liste drei oder mehr Filter enthält.

## hinzufügen der Logik zu einer intelligenten Liste {#add-logic-to-a-smart-list}

Standardmäßig finden Sie in Ihrer intelligenten Liste die Personen, die mit den Filtern **ALL** übereinstimmen (Filter 1 _und_ 2 _und_ 3). Sie können die Regellogik ändern, um nach Personen zu suchen, die **ANY** der definierten Filter (Filter 1 _oder_ 2 _oder_ 3) übereinstimmen, oder erweiterte Filter (Filter 1 _und_ 2 _oder_ 3) verwenden.

In diesem Beispiel möchten Sie Personen in Kalifornien _und_ mit einem Ergebnis von mindestens 50 Punkten _oder_ mit dem Status &quot;Sales Qualified&quot;finden.

1. Wählen Sie **Erweiterte Filter** aus der Dropdownliste.

   ![](assets/one.png)

   >[!NOTE]
   >
   >Durch die Verwendung von **Advanced**-Filtern müssen keine intelligenten Listen mit dem Filter Member of Smart Liste erstellt werden. Dies hilft, die Leistung zu optimieren.

1. Im Textfeld **Erweiterte Filter** wird &quot;und&quot;als Standardwert für alle Filter angezeigt.

   ![](assets/two-2.png)

1. Geben Sie ein Paar Klammern um &quot;2 und 3&quot;ein.

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >Bei der Eingabe der Regellogik müssen Sie &quot;und&quot;vor &quot;oder&quot;verwenden.

1. Ändern Sie das &quot;und&quot;zwischen &quot;2 und 3&quot;in &quot;oder&quot;.

   ![](assets/four-1.png)

## Klammern beim Mischen von &quot;And&quot;und &quot;or {#use-parentheses-when-mixing-and-and-or}

Das Mischen von &quot;Und&quot;- und &quot;Oder&quot;-Logik erfordert Klammern, um Ihre Absicht klar zu machen.

![](assets/advancedfilters-parent.png)

## Verschachtelte Klammern für vier oder mehr Filter verwenden, wenn erforderlich {#use-nested-parentheses-for-four-or-more-filters-if-needed}

Abhängig von Ihrer Absicht müssen Sie ggf. verschachtelte Klammern hinzufügen, wenn Sie vier oder mehr Filter verwenden.

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>Wenn Sie eine ungültige Regel eingeben, wird eine rote Linie unter der Regel angezeigt. Blättern Sie über den Text, um die entsprechende Fehlermeldung anzuzeigen.
