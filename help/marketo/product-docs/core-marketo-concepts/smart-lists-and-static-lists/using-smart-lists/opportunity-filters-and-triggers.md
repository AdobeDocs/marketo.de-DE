---
unique-page-id: 8159286
description: Opportunity Filters and Trigger - Marketo Docs - Produktdokumentation
title: Opportunity Filters and Trigger
exl-id: 5b372c00-1553-4ac3-a495-53e208371d8d
feature: Smart Lists
source-git-commit: 8a5903fa5313e34f448f833f20ab8e3624cf23e6
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 5%

---

# Opportunity Filters and Trigger {#opportunity-filters-and-triggers}

Mit Opportunity-Filtern und -Triggern können Sie Opportunity-Ereignisse aus Salesforce verfolgen. Sie unterscheiden sich etwas von anderen Filtern und Triggern.

## Opportunity Filters {#opportunity-filters}

Mit Opportunity-Filtern können Sie in Ihre Salesforce-Leads vordringen, die Möglichkeiten haben. Sie finden sie beim Bearbeiten einer Smart-Liste im Ordner &quot;Chancen&quot;der Palette. Sie kommen in ein paar Geschmacksrichtungen.

* Anzahl Opportunities
* Opty-Gesamtbetrag
* Erwarteter Opty-Gesamtumsatz
* Hat Opportunity
* Chancen wurden hinzugefügt
* Chancen wurden entfernt
* Opportunity wurde aktualisiert

Wenn Sie nach Ihren (benutzerdefinierten oder standardmäßigen) Opportunity-Feldern suchen, verwenden Sie die **Hat Chancen** Filter oder **Chancen`[Added/Removed/Updated]`** Filter oder Trigger.

**Anzahl der Optionen, Gesamtanzahl der Optionen, Gesamtanzahl der Optionen, Gesamterwarteter Gesamtumsatz der Option**

Mit diesen Filtern können Sie Leads auf Grundlage der Gesamtzahl, des Betrags oder des erwarteten Umsatzes aller ihrer Möglichkeiten finden.

![](assets/image2015-6-11-12-3a29-3a34.png)

**Hat Gelegenheit, wurde der Gelegenheit hinzugefügt, wurde aus der Gelegenheit entfernt**

Wenn Sie nach Leads suchen, die Möglichkeiten basierend auf einer Kombination von Kriterien haben, verwenden Sie die **Hat Chancen**, **wurde der Gelegenheit hinzugefügt** oder **Aus Opportunity entfernt** Filter. Sie sagen Ihnen:

* **Hat Chancen**: Wenn dieser Lead derzeit eine übereinstimmende Chance hat
* **wurde der Gelegenheit hinzugefügt**: Wenn dieser Lead jemals zu einer übereinstimmenden Gelegenheit hinzugefügt wurde
* **Aus Opportunity entfernt**: Wenn dieser Lead jemals aus einer übereinstimmenden Gelegenheit entfernt wurde

Fügen Sie die Suchkriterien als **Einschränkungen** auf den Filter. Zu den Einschränkungen gehören Ihr Opportunity-Standard und Ihre benutzerdefinierten Felder:

![](assets/image2015-6-11-12-3a31-3a0.png)

![](assets/image2015-6-11-12-3a31-3a46.png)

Angenommen, Sie möchten Leads finden, die Öffnungsmöglichkeiten von mindestens 5.000 $ haben. Ziehen Sie in die **Hat Chancen** und verwenden Sie **Ist geschlossen** und **Betrag** Einschränkungen:

![](assets/image2015-6-11-12-3a32-3a0.png)

>[!NOTE]
>
>Wenn Sie mehrere Opportunity-Filter verwenden, erhalten Sie möglicherweise falsche Antworten. Wenn Sie das obige Beispiel mit zwei Opportunity-Filtern erstellt haben, erhalten Sie eine Liste von Leads, die eine Chance von mindestens 5.000 $ haben, und jede Gelegenheit, die geschlossen wird, auch wenn es sich um separate Möglichkeiten handelt.

**Opportunity wurde aktualisiert**

Die **Gelegenheit wurde aktualisiert** -Filter sucht nach allen Möglichkeiten, wenn ein bestimmtes Opportunitätsfeld aktualisiert wurde. Wählen Sie das Feld aus, das mit der Pulldown-Liste &quot;Trigger-Attribut&quot;überprüft werden soll, und verwenden Sie dann die Begrenzungen, um den Änderungssatz einzuschränken.

Dieser Filter zeigt beispielsweise alle Leads an, deren Datum sich in den letzten 30 Tagen geändert hat:

![](assets/image2015-6-11-12-3a33-3a7.png)

## Opportunity Trigger {#opportunity-triggers}

Die folgenden Opportunity-Trigger sind verfügbar. Sie funktionieren genau wie die entsprechenden Filter (siehe Beschreibung weiter oben). Sie können jedoch Kampagnen direkt bei Eintreten des Ereignisses Trigger haben:

* Opportunity wird aktualisiert
* Zu Opportunity hinzugefügt
* Aus Opportunity entfernt

Beispielsweise können Sie diese Smart-Liste zum Trigger verwenden, wenn ein Lead einer beliebigen Gelegenheit hinzugefügt wird. Im Fluss können Sie sie der Liste Ausgesetzte Marketing hinzufügen oder ihnen eine zielgerichtete E-Mail senden.

![](assets/image2015-6-11-12-3a33-3a48.png)

Verwenden Sie zum Trigger Ihrer Opportunity-benutzerdefinierten Felder die **Chancen werden aktualisiert** Trigger und wählen Sie das Feld in der Pulldown-Liste aus:

![](assets/image2015-6-11-12-3a33-3a34.png)
