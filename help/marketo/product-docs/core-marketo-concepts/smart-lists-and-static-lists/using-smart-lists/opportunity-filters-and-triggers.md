---
unique-page-id: 8159286
description: Opportunity Filters and Triggers - Marketing Docs - Produktdokumentation
title: Chancen, Filter und Auslöser
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---


# Opportunity-Filter und -Auslöser {#opportunity-filters-and-triggers}

Mit Filtern und Auslösern von Chancen können Sie Ereignis von Salesforce nachverfolgen. Sie unterscheiden sich etwas von anderen Filtern und Auslösern.

## Opportunity-Filter {#opportunity-filters}

Mit den Filtern von Gelegenheiten können Sie Ihre Salesforce-Leads, die Chancen haben, näher untersuchen. Sie können sie beim Bearbeiten einer intelligenten Liste im Ordner &quot;Chancen&quot;der Palette finden. Sie kommen in ein paar Geschmacksrichtungen.

* Anzahl der Optionen
* Optimalbetrag gesamt
* Erwarteter Gesamtumsatz der Option
* Hat Chancen
* Gelegenheit wurde hinzugefügt
* Chancen wurden entfernt
* Gelegenheit wurde aktualisiert

Wenn Sie nach Ihren Opportunity-Feldern suchen (benutzerdefiniert oder Standard), verwenden Sie den Filter **Hat Chancen** oder **Die Gelegenheit war`[Added/Removed/Updated]`** Filter oder Auslöser.

**Anzahl der Optionen, Gesamtanzahl der Optionen, Gesamtsumme der Optionen, Gesamtsumme des erwarteten Umsatzes**

Mit diesen Filtern können Sie Interessenten auf Basis der Gesamtanzahl, des Betrags oder des erwarteten Umsatzes all ihrer Chancen finden.

![](assets/image2015-6-11-12-3a29-3a34.png)

**Hat Chancen, wurde zu Chancen hinzugefügt, wurde aus der Gelegenheit entfernt**

Wenn Sie nach Interessenten suchen, die Möglichkeiten auf der Grundlage einer Kombination von Kriterien haben, verwenden Sie den Filter **Hat Gelegenheit**, **Wurde zu Opportunity** hinzugefügt oder **Wurde aus Opportunity** entfernt. Sie sagen Ihnen:

* **Hat Gelegenheit**: Wenn dieser Interessent derzeit eine passende Gelegenheit hat
* **Der Möglichkeit** wurde hinzugefügt: Wenn dieser Interessent jemals einer passenden Gelegenheit hinzugefügt wurde
* **Aus der Gelegenheit** entfernt: Wenn dieser Interessent jemals aus einer passenden Gelegenheit entfernt wurde

hinzufügen Sie die Suchkriterien im Filter mit **Beschränkungen**. Zu den Einschränkungen gehören Ihre Standard- und benutzerdefinierten Felder für Möglichkeiten:

![](assets/image2015-6-11-12-3a31-3a0.png)

![](assets/image2015-6-11-12-3a31-3a46.png)

Nehmen wir beispielsweise an, Sie möchten Interessenten finden, die eine offene Chance von mindestens 5.000 Dollar haben. Ziehen Sie den Filter **Hat Gelegenheit** und verwenden Sie die Einschränkungen **Ist geschlossen** und **Betrag**:

![](assets/image2015-6-11-12-3a32-3a0.png)

>[!NOTE]
>
>Wenn Sie mehrere Opportunity-Filter verwenden, erhalten Sie möglicherweise falsche Antworten. Wenn Sie das obige Beispiel mit zwei Opportunity-Filtern erstellen, erhalten Sie eine Liste von Interessenten, die eine Chance von mindestens 5.000 $ haben und jede Gelegenheit, die geschlossen ist, auch wenn es sich um separate Möglichkeiten handelt.

**Gelegenheit wurde aktualisiert**

Der Filter **Gelegenheit wurde aktualisiert** sucht nach Möglichkeiten, wenn ein bestimmtes Feld aktualisiert wurde. Wählen Sie das Feld aus, um es mit dem Pulldown für das Auslöserattribut zu überprüfen, und verwenden Sie dann die Einschränkungen, um den Satz der Änderungen einzugrenzen.

Dieser Filter zeigt beispielsweise alle Interessenten an, deren Datumsangabe in den letzten 30 Tagen kurz war:

![](assets/image2015-6-11-12-3a33-3a7.png)

## Opportunity Triggers {#opportunity-triggers}

Die folgenden Gelegenheitsauslöser stehen zur Verfügung. Sie funktionieren genau wie die entsprechenden Filter (siehe Beschreibung weiter oben), allerdings können sie Kampagnen direkt auslösen, wenn das Ereignis eintritt:

* Chancen werden aktualisiert
* Zu Chancen hinzugefügt
* Aus Gelegenheit entfernt

Beispielsweise können Sie diese intelligente Liste verwenden, um auszulösen, wenn ein Interessent einer Gelegenheit hinzugefügt wird. Im Fluss können Sie sie der Liste &quot;Ausgesetzt für Marketing&quot;hinzufügen oder ihnen eine zielgerichtete E-Mail senden.

![](assets/image2015-6-11-12-3a33-3a48.png)

Wenn Sie Ihre Gelegenheit für benutzerdefinierte Felder auslösen möchten, verwenden Sie den Auslöser **Gelegenheit wurde aktualisiert** und wählen Sie das Feld im Pulldown aus:

![](assets/image2015-6-11-12-3a33-3a34.png)

