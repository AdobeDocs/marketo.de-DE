---
unique-page-id: 7512524
description: Best Practices für intelligente Listen - Marketo-Dokumente - Produktdokumentation
title: Best Practices für Smart-Listen
exl-id: 466de198-1012-4ac3-906c-d41943fe5bc0
feature: Smart Lists
source-git-commit: b6628cee17799801815f5b84c424399538eaf5ee
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# Best Practices für Smart-Listen {#best-practices-for-smart-lists}

Smart-Listen sind das leistungsfähigste Abfragetool in der Marketing-Rubrik. Sie finden die Menschen, die Sie suchen, mit magischer Geschwindigkeit und Leichtigkeit.

Um die Arbeit mit ihnen zu erleichtern und die Leistung zu optimieren, haben wir eine Liste bewährter Verfahren erstellt. Viel Spaß!

>[!NOTE]
>
>**Jeder Kunde ist anders.** Je größer die Datenbank, desto mehr Verarbeitung erfolgt. Je mehr Aktivitäten Sie gespeichert haben, desto länger dauert die Suche.
>
>Wenn Sie eine Langsamkeit feststellen, versuchen Sie die folgenden Tipps. Wenn das Problem weiterhin besteht, wenden Sie sich an [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. **Begrenzungsverlauf -** Verlaufsfilter (auch Aktivitätsfilter genannt) gehören zu den ressourcenintensivsten und zeitaufwendigsten Vorgängen. Wenn Sie sie verwenden müssen, versuchen Sie, den Datumsbereich so kurz wie möglich zu beschränken, wodurch der durchsuchbare Datensatz reduziert wird. Darüber hinaus werden die Aufbewahrungsfristen nicht durch Datumsbereiche ersetzt. Beispiel: Wenn die Aktivität, die Sie abfragen, eine 90-tägige Aufbewahrungsfrist hat und Sie &quot;Letzte 100 Tage&quot;auswählen, werden nur Ergebnisse der letzten 90 Tage zurückgegeben. Aufbewahrungsfristen [finden Sie hier .](https://nation.marketo.com/t5/knowledgebase/marketo-activities-data-retention-policy/ta-p/251480){target="_blank"}.
1. **Einschränken verschachtelter Smart-Listen -** Begrenzen Sie beim Erstellen einer neuen Smart-Liste die Anzahl der verwendeten Filter für die intelligente Liste. Dies wird als Verschachteln von Smart-Listen bezeichnet und jede referenzierte intelligente Liste verlängert die Verarbeitungszeit. Verweisen Sie stattdessen entweder auf statische Listen oder verwenden Sie [Segmentierung](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md){target="_blank"}.
1. **Verwenden Sie positive gegenüber negative Operatoren -** &quot;Nicht&quot;-Filter sind zwar verfügbar, müssen aber den gesamten Datensatz in Ihrer Instanz durchsuchen, was sehr zeitaufwendig sein kann. Positive &quot;is&quot;-Filter können effektivere Suchalgorithmen nutzen.
1. **Vermeiden Sie &quot;enthält&quot;-** Wenn Sie nur partielle Daten haben, liefern &quot;beginnt mit&quot;-Qualifikatoren deutlich schnellere Ergebnisse als &quot;enthält&quot;. &quot;Ist&quot;wird noch schneller ausgeführt. Vermeiden Sie die Verwendung von &quot;enthält&quot;mit mehreren Werten. Beide zusammen können eine Kampagne noch weiter verlangsamen.
1. **Zufallsbeispiel allein verwenden -** &quot;Zufallsbeispiel&quot;ist ein spezieller Filter. Benutzen Sie es allein, um Ihre Leute in vordefinierte Listen zu setzen. Verwenden Sie dann einfach &quot;Mitglied der Liste&quot;, um Ihre intelligente Liste schnell zu erstellen. Zufällige Beispiele **NOT** mit verschachtelten Smart-Listen arbeiten. Der Filter &quot;Zufällige Beispiele&quot;funktioniert nicht, wenn es sich um die Smart-Liste handelt, auf die für den Filter &quot;Mitglied der Smart-Liste&quot;verwiesen wird.
1. **Sparen Sie sich bei Inaktivitätsfiltern -** Filter wie &quot;Nicht ausgefülltes Formular&quot;können zwar sehr nützlich sein, erfordern aber viel mehr Verarbeitungsleistung.
1. **Sparen Sie sich beim Einfügen in mehrere Werte -** Mehrfachauswahl ist für das Einfügen in Dutzende oder möglicherweise Hunderte von Werten konzipiert. Man muss jedoch zu viele einbringen, und es wird sich verlangsamen.
1. **Sparen Sie sich beim Hinzufügen von Begrenzungen -** Dies sind die winzigen Details einer Regel und verwandte Werte. Je mehr Einschränkungen Sie hinzufügen, desto langsamer dauert die Verarbeitung.
1. **Vereinfachen Sie Ihre Kampagnen -** Mehr als 100 unabhängige Regeln (wir haben es gesehen!) werden natürlich einige Zeit in Anspruch nehmen. Halten Sie es einfach und Sie werden die Geschwindigkeitssteigerungen bemerken - und es wird Ihnen leichter sein, es zu verstehen.
1. **Bei Verwendung des Filters &quot;E-Mail-Adresse&quot;das @-Symbol vor dem Domänennamen einschließen** **-** Dadurch wird eine schnellere Abfrage verwendet. Beispiel: anstelle von _email enthält &#39;somedomain.com&#39;_, verwenden _email contains &#39;@somedomain.com_.&#39; Wenn Sie mehrere E-Mail-Adressen mit &quot;enthält&quot;verwenden, müssen ALLE von ihnen mit &quot;@&quot;beginnen.

>[!TIP]
>
>Marketo Engage kann auf vielerlei Weise eingesetzt werden und bestimmte Techniken sind besser für Sie und Ihr Unternehmen. Wenden Sie sich an Ihren Adobe Professional Services Sales Rep , wenn Sie Hilfe beim bestmöglichen Nutzen Ihrer Investition benötigen.
