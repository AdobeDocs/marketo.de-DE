---
unique-page-id: 1146901
description: Verwenden der erweiterten Regellogik für intelligente Listen - Marketing Docs - Produktdokumentation
title: Erweiterte Logik der Smart-Liste
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# Verwenden der erweiterten Regellogik für intelligente Listen {#using-advanced-smart-list-rule-logic}

Sie können genau die Personen finden, die Sie benötigen, indem Sie innerhalb einer intelligenten Liste eine intelligente Liste-Regellogik auf mehrere Filter anwenden. So geht es.

>[!PREREQUISITES]
>
>* [Filter für eine intelligente Liste suchen und Hinzufügen](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [Definieren von Filtern für intelligente Listen](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)

>



>[!NOTE]
>
>Erweiterte Filterlogik ist nur verfügbar, wenn Ihre intelligente Liste drei oder mehr Filter enthält.

## hinzufügen der Logik zu einer intelligenten Liste {#add-logic-to-a-smart-list}

Standardmäßig finden Sie in Ihrer intelligenten Liste die Personen, die mit den Filtern **ALL** übereinstimmen (Filter 1 *und* 2 *und* 3). Sie können die Regellogik ändern, um nach Personen zu suchen, die **ANY** der definierten Filter (Filter 1 *oder* 2 *oder* 3) übereinstimmen, oder erweiterte Filter (Filter 1 *und* 2 *oder *3) verwenden.

In diesem Beispiel möchten Sie Personen in Kalifornien *und* mit einem Ergebnis von mindestens 50 Punkten *oder* mit dem Status &quot;Sales Qualified&quot;finden.

1. Wählen Sie **Verwenden Sie** **Erweitert** **Filter** aus der Dropdownliste.

   ![](assets/one.png)

   >[!NOTE]
   >
   >Durch die Verwendung von **Advanced**-Filtern müssen keine intelligenten Listen mit dem Filter Member of Smart Liste erstellt werden. Dies hilft, die Leistung zu optimieren.

1. Das Textfeld **Erweitert** **Filter** zeigt &quot;und&quot;als Standardwert zwischen allen Ihren Filtern an.

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

