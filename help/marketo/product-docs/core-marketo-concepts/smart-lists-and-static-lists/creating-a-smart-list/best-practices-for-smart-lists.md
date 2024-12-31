---
unique-page-id: 7512524
description: Best Practices für Smart Lists - Marketo-Dokumente - Produktdokumentation
title: Best Practices für Smart Lists
exl-id: 466de198-1012-4ac3-906c-d41943fe5bc0
feature: Smart Lists
source-git-commit: 198d7d7fd4c1c312aeb30fa922fd89863ac87f81
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Best Practices für Smart Lists {#best-practices-for-smart-lists}

Smart Lists sind das leistungsfähigste Abfrage-Tool im Marketing-Universum. Sie finden die Menschen, die Sie suchen, mit magischer Geschwindigkeit und Leichtigkeit.

Um die Arbeit mit ihnen zu vereinfachen und die Leistung zu optimieren, haben wir eine Liste von Best Practices erstellt. Viel Spaß!

>[!NOTE]
>
>**Jeder Marketo Engage-Anwender ist anders.** Je größer die Datenbank, desto mehr Verarbeitung erfolgt. Je mehr Aktivitäten Sie gespeichert haben, desto länger dauert es, sie zu durchsuchen.
>
>Wenn Sie Langsamkeit verspüren, versuchen Sie die folgenden Tipps. Wenn das Problem weiterhin besteht, wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. **Limitverlauf -** Verlaufsfilter (auch Aktivitätsfilter genannt) gehören zu den ressourcenintensivsten und zeitaufwendigsten Vorgängen. Wenn Sie sie verwenden müssen, versuchen Sie, den Datumsbereich auf so kurz wie möglich zu beschränken, wodurch der durchsuchbare Datensatz reduziert würde. Darüber hinaus ersetzen Datumsbereiche keine Aufbewahrungsfristen. Beispiel: Wenn die Aktivität, die Sie abfragen, eine Aufbewahrungsfrist von 90 Tagen hat und Sie „Letzte 100 Tage“ auswählen, werden nur Ergebnisse aus den letzten 90 Tagen zurückgegeben. Aufbewahrungsfristen für Aktivitäten [finden Sie hier](https://nation.marketo.com/t5/knowledgebase/marketo-activities-data-retention-policy/ta-p/251480){target="_blank"}.
1. **Einschränken von verschachtelten Smart-Listen -** Beschränken Sie beim Erstellen einer neuen Smart-Liste die Anzahl der verwendeten Filter „Mitglieder der Smart-Liste“. Dies wird als Verschachteln von Smart Lists bezeichnet. Jede Smart List, auf die verwiesen wird, verlängert die Verarbeitungszeit. Verweisen Sie stattdessen entweder auf statische Listen oder verwenden Sie [Segmentierung](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md){target="_blank"}.
1. **Positive über negative Operatoren verwenden -** Obwohl „Nicht“-Filter verfügbar sind, müssen sie den gesamten Datensatz in Ihrer Instanz durchsuchen, was extrem zeitaufwendig sein kann. Positive „is“-Filter können effektivere Suchalgorithmen nutzen.
1. **Vermeiden Sie „contains“ -** Wenn Sie nur partielle Daten haben, liefert „starts with“-Kriterien viel schnellere Ergebnisse als „contains“. „Is“ wird sogar noch schneller ausgeführt. Vermeiden Sie die Verwendung von „contains“ mit mehreren Werten; die beiden zusammen können eine Kampagne noch weiter verlangsamen.
1. **Zufallsprobe allein verwenden -** Zufallsprobe ist ein spezieller Filter. Nutzen Sie es für sich, um Ihre Leute in vorgefertigte Listen zu setzen. Verwenden Sie dann einfach „Member of List“, um Ihre Smart List superschnell zu machen. Die zufällige Stichprobe **NICHT** mit verschachtelten Smart Lists. Der Filter Zufällige Stichprobe funktioniert nicht, wenn es sich um die Smart-Liste handelt, auf die für den Filter „Mitglied der Smart-Liste“ verwiesen wird.
1. **Seien Sie sparsam mit Inaktivitätsfiltern -** Filter wie „Nicht ausgefülltes Formular“ können wirklich nützlich sein, erfordern aber viel mehr Rechenleistung.
1. **Seien Sie sparsam mit dem Einfügen in mehrere Werte -** Multi-select ist zum Einfügen in Dutzende oder möglicherweise Hunderte von Werten konzipiert. Wenn man jedoch zu viele davon einbringt, wird man langsamer werden.
1. **sparsam sein beim Hinzufügen von Einschränkungen -** Dies sind die winzigen Details einer Regel und zugehörigen Werte. Je mehr Einschränkungen Sie hinzufügen, desto langsamer wird die Verarbeitungszeit.
1. **Vereinfachen Sie Ihre Kampagnen -** 100+ unabhängige Regeln (wir haben es gesehen!) brauchen natürlich einige Zeit, um sie zu verarbeiten. Halten Sie es einfach und Sie werden die Geschwindigkeitsgewinne bemerken - und es wird für Sie leichter zu verstehen sein.
1. **Bei Verwendung des E-Mail-Adressfilters muss vor dem Domain-Namen das @-Symbol** werden **-** Dadurch wird eine schnellere Abfrage verwendet. Beispiel: Verwenden Sie anstelle von _E-Mail enthält &#39;somedomain.com_ &quot;_enthält &#39;@somedomain.com_&quot;. Wenn Sie mehrere E-Mail-Adressen mit „contains“ verwenden, müssen ALLE mit &quot;@&quot; beginnen.

>[!TIP]
>
>Marketo Engage kann auf viele Arten verwendet werden und bestimmte Techniken sind besser für Sie und Ihr Unternehmen. Wenden Sie sich an Ihren Adobe Professional Services-Vertriebsmitarbeiter, wenn Sie Unterstützung benötigen, um Ihre Investition optimal zu nutzen.
