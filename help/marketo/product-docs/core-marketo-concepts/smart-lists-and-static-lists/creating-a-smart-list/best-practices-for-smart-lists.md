---
unique-page-id: 7512524
description: Best Practices für intelligente Listen - Marketo-Dokumente - Produktdokumentation
title: Best Practices für Smart-Listen
exl-id: 466de198-1012-4ac3-906c-d41943fe5bc0
feature: Smart Lists
source-git-commit: 198d7d7fd4c1c312aeb30fa922fd89863ac87f81
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Best Practices für Smart-Listen {#best-practices-for-smart-lists}

Smart-Listen sind das leistungsfähigste Abfragetool in der Marketing-Rubrik. Sie finden die Menschen, die Sie suchen, mit magischer Geschwindigkeit und Leichtigkeit.

Um die Arbeit mit ihnen zu vereinfachen und die Leistung zu optimieren, haben wir eine Liste mit Best Practices erstellt. Viel Spaß!

>[!NOTE]
>
>**Jeder Marketo Engage-Benutzer ist anders.** Je größer die Datenbank, desto mehr Verarbeitung erfolgt. Je mehr Aktivitäten Sie gespeichert haben, desto länger dauert die Suche.
>
>Wenn Sie eine Langsamkeit feststellen, versuchen Sie die folgenden Tipps. Wenn das Problem weiterhin besteht, wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. **Begrenzungsverlauf -** Verlaufsfilter (auch Aktivitätsfilter genannt) gehören zu den ressourcenintensivsten und zeitaufwendigsten Vorgängen. Wenn Sie sie verwenden müssen, versuchen Sie, den Datumsbereich so kurz wie möglich zu beschränken, wodurch der durchsuchbare Datensatz reduziert wird. Darüber hinaus werden die Aufbewahrungsfristen nicht durch Datumsbereiche ersetzt. Beispiel: Wenn die Aktivität, die Sie abfragen, eine 90-tägige Aufbewahrungsfrist hat und Sie &quot;Letzte 100 Tage&quot;auswählen, werden nur Ergebnisse der letzten 90 Tage zurückgegeben. Die Aufbewahrungsfristen für Aktivitäten [ finden Sie hier ](https://nation.marketo.com/t5/knowledgebase/marketo-activities-data-retention-policy/ta-p/251480){target="_blank"}.
1. **Schränken verschachtelter Smart-Listen ein -** Begrenzen Sie beim Erstellen einer neuen Smart-Liste die Anzahl der verwendeten Filter &quot;Mitglied der Smart-Liste&quot;. Dies wird als Verschachteln von Smart-Listen bezeichnet und jede referenzierte Smart-Liste verlängert die Verarbeitungszeit. Verweisen Sie stattdessen auf statische Listen oder verwenden Sie [segmentation](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md){target="_blank"}.
1. **Positive Operatoren gegenüber negativen Operatoren verwenden -** Obwohl &quot;keine&quot;Filter verfügbar sind, müssen sie den gesamten Datensatz in Ihrer Instanz durchsuchen, was sehr zeitaufwendig sein kann. Positive &quot;is&quot;-Filter können effektivere Suchalgorithmen nutzen.
1. **Vermeiden Sie &quot;enthält&quot;-** Wenn Sie nur partielle Daten haben, liefern &quot;beginnt mit&quot;-Qualifikatoren deutlich schnellere Ergebnisse als &quot;enthält&quot;. &quot;Ist&quot;wird noch schneller ausgeführt. Vermeiden Sie die Verwendung von &quot;enthält&quot;mit mehreren Werten. Beide zusammen können eine Kampagne noch weiter verlangsamen.
1. **Zufallsbeispiel allein verwenden -** Zufallsbeispiel ist ein spezieller Filter. Benutzen Sie es allein, um Ihre Leute in vordefinierte Listen zu setzen. Verwenden Sie dann einfach &quot;Mitglied der Liste&quot;, um Ihre Smart List schnell zu machen. Das Zufallsbeispiel funktioniert mit verschachtelten Smart-Listen **NOT**. Der Filter &quot;Zufällige Beispiele&quot;funktioniert nicht, wenn es sich um die Smart-Liste handelt, auf die für den Filter &quot;Mitglied der Smart-Liste&quot;verwiesen wird.
1. **Seien Sie sparsam mit Inaktivitätsfiltern -** Filter wie &quot;Nicht ausgefülltes Formular&quot;können zwar wirklich nützlich sein, erfordern aber viel mehr Verarbeitungsleistung.
1. **Sparen Sie sich beim Einfügen in mehrere Werte -** Multi-Select wurde für das Einfügen in Dutzende oder möglicherweise Hunderte von Werten entwickelt. Man muss jedoch zu viele einbringen, und es wird sich verlangsamen.
1. **Seien Sie beim Hinzufügen von Begrenzungen sparsam -** Dies sind die winzigen Details einer Regel und verwandter Werte. Je mehr Einschränkungen Sie hinzufügen, desto langsamer dauert die Verarbeitung.
1. **Vereinfachen Sie Ihre Kampagnen -** 100+ unabhängige Regeln (wir haben sie gesehen!) werden natürlich einige Zeit in Anspruch nehmen. Halten Sie es einfach und Sie werden die Geschwindigkeitssteigerungen bemerken - und es wird Ihnen leichter sein, es zu verstehen.
1. **Fügen Sie bei Verwendung des Filters &quot;E-Mail-Adresse&quot;das Symbol &quot;@&quot;vor dem Domänennamen ein** **-** Dadurch wird eine schnellere Abfrage verwendet. Beispiel: Verwenden Sie anstelle von _E-Mail enthält &#39;somedomain.com&#39;_ _E-Mail enthält &#39;@somedomain.com_&#39;. Wenn Sie mehrere E-Mail-Adressen mit &quot;enthält&quot;verwenden, müssen ALLE von ihnen mit &quot;@&quot;beginnen.

>[!TIP]
>
>Marketo Engage kann auf vielerlei Weise eingesetzt werden und bestimmte Techniken sind besser für Sie und Ihr Unternehmen. Wenden Sie sich an Ihren Adobe Professional Services Sales Rep , wenn Sie Hilfe beim bestmöglichen Nutzen Ihrer Investition benötigen.
