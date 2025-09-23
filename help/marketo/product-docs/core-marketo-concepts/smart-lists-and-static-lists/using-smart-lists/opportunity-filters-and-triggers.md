---
unique-page-id: 8159286
description: Opportunity-Filter und -Trigger - Marketo-Dokumente - Produktdokumentation
title: Opportunity-Filter und -Auslöser
exl-id: 5b372c00-1553-4ac3-a495-53e208371d8d
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 6%

---

# Opportunity-Filter und -Auslöser {#opportunity-filters-and-triggers}

Mit Opportunity-Filtern und Triggern können Sie Opportunity-Ereignisse aus [!DNL Salesforce] verfolgen. Sie unterscheiden sich ein wenig von anderen Filtern und Triggern.

## Opportunity Filter {#opportunity-filters}

Mit Opportunity-Filtern können Sie Ihren Salesforce Leads, die Opportunities haben, einen Überblick verschaffen. Sie finden sie im Ordner Opportunities der Palette, wenn Sie eine Smart-Liste bearbeiten. Es gibt sie in verschiedenen Geschmacksrichtungen.

* Anzahl Möglichkeiten
* Opty-Gesamtbetrag
* Erwarteter Opty-Gesamtumsatz
* Hat Opportunity
* Gelegenheit wurde hinzugefügt
* Opportunity wurde entfernt
* Opportunity wurde aktualisiert

Wenn Sie nach Ihren Opportunity-Feldern (benutzerdefiniert oder standardmäßig) suchen, verwenden Sie den Filter **Hat Opportunity** oder **Opportunity war`[Added/Removed/Updated]`** Filter oder Trigger.

**Anzahl der Optys, Gesamtbetrag der Optys, Gesamtbetrag der erwarteten Optys-Einnahmen**

Mit diesen Filtern können Sie Leads basierend auf der Gesamtzahl, dem Betrag oder dem erwarteten Umsatz aller Opportunitys finden.

![](assets/opportunity-filters-and-triggers-1.png)

**Hat Opportunity, wurde zu Opportunity hinzugefügt, wurde von Opportunity entfernt**

Wenn Sie nach Leads suchen, die Chancen auf der Grundlage einer Kombination von Kriterien haben, verwenden Sie den Filter **Hat Opportunity**, **Wurde zur Opportunity hinzugefügt** oder **Wurde aus Opportunity entfernt**. Sie sagen Ihnen:

* **Hat Opportunity**: Wenn dieser Lead derzeit eine passende Opportunity hat
* **Wurde zur Opportunity hinzugefügt**: Wenn dieser Lead je zu einer entsprechenden Opportunity hinzugefügt wurde
* **Wurde aus Opportunity entfernt**: Wenn dieser Lead jemals aus einer entsprechenden Opportunity entfernt wurde

Fügen Sie die Suchkriterien als &quot;**&quot;** Filter hinzu. Zu den Einschränkungen gehören Ihre standardmäßigen Opportunity- und benutzerdefinierten Felder:

![](assets/opportunity-filters-and-triggers-2.png)

![](assets/opportunity-filters-and-triggers-3.png)

Angenommen, Sie möchten Leads finden, die offene Opportunitys von mindestens 5.000 USD haben. Ziehen Sie den Filter **Hat Opportunity** und verwenden Sie die Begrenzungen **Ist geschlossen** und **Betrag**:

![](assets/opportunity-filters-and-triggers-4.png)

>[!NOTE]
>
>Wenn Sie mehrere Opportunity-Filter verwenden, erhalten Sie möglicherweise falsche Antworten. Wenn Sie das obige Beispiel mit zwei Opportunity-Filtern erstellen, erhalten Sie eine Liste der Leads, die eine Opportunity haben, die mindestens 5.000 US-Dollar beträgt, sowie jede Opportunity, die geschlossen wird, selbst wenn es sich um separate Opportunities handelt.

**Opportunity wurde aktualisiert**

Der **Opportunity wurde aktualisiert** Filter sucht nach jeder Opportunity, wenn ein bestimmtes Opportunity-Feld aktualisiert wurde. Trigger Wählen Sie das Feld aus, das mit dem Pulldown-Menü Feldattribut überprüft werden soll, und grenzen Sie dann den Änderungssatz mithilfe der Einschränkungen ein.

Beispielsweise zeigt dieser Filter alle Leads an, deren Abschlussdatum sich in den letzten 30 Tagen geändert hat:

![](assets/opportunity-filters-and-triggers-5.png)

## Opportunity-Trigger {#opportunity-triggers}

Die folgenden Opportunity-Trigger sind verfügbar. Sie funktionieren genau wie die entsprechenden (zuvor beschriebenen) Filter, mit dem Unterschied, dass sie Kampagnen direkt bei Eintritt des Ereignisses in den Trigger aufnehmen können:

* Opportunity wird aktualisiert
* Zu Opportunity hinzugefügt
* Aus Opportunity entfernt

Beispielsweise können Sie diese Smart-Liste zum Trigger verwenden, wenn einer Opportunity ein Lead hinzugefügt wird. Im Fluss können Sie sie zur Liste ausgesetztes Marketing hinzufügen oder ihnen eine zielgerichtete E-Mail senden.

![](assets/opportunity-filters-and-triggers-6.png)

Verwenden Sie zum Trigger Ihrer benutzerdefinierten Opportunity-Felder den Trigger **Opportunity wird aktualisiert** und wählen Sie das Feld in der Pulldown-Liste aus:

![](assets/opportunity-filters-and-triggers-7.png)
