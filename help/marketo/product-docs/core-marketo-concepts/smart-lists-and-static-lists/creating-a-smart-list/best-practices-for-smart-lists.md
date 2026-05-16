---
unique-page-id: 7512524
description: Hier erhalten Sie Hilfe zu Best Practices für Smart Lists. Mit diesen Tipps können Sie schnellere und genauere Listen erstellen.
title: Best Practices für intelligente Listen
exl-id: 466de198-1012-4ac3-906c-d41943fe5bc0
feature: Smart Lists
TQID: https://experienceleague.adobe.com/Z1k--jj24QHIEThtPbj29i9FBhcEp0Hf9hBeZEgSP3w
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 592
ht-degree: 2%

---

# Best Practices für intelligente Listen {#best-practices-for-smart-lists}

Smart Lists sind das leistungsfähigste Abfrage-Tool im Marketing-Universum. Sie finden die Menschen, die Sie suchen, mit magischer Geschwindigkeit und Leichtigkeit.

Um die Arbeit mit ihnen zu vereinfachen und die Leistung zu optimieren, werden folgende Best Practices bereitgestellt.

>[!NOTE]
>
>**Jeder Marketo Engage-Benutzer ist anders.** Je größer die Datenbank, desto mehr Verarbeitung erfolgt. Je mehr Aktivitäten Sie gespeichert haben, desto länger dauert es, sie zu durchsuchen.
>
>Wenn Sie Langsamkeit verspüren, versuchen Sie die folgenden Tipps. Wenn das Problem weiterhin besteht, wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support?profile.language=de){target="_blank"}.

1. **Limitverlauf -** Verlaufsfilter (auch Aktivitätsfilter genannt) gehören zu den ressourcenintensivsten und zeitaufwendigsten Vorgängen. Wenn Sie sie verwenden müssen, versuchen Sie, den Datumsbereich auf so kurz wie möglich zu beschränken, wodurch der durchsuchbare Datensatz reduziert würde. Darüber hinaus ersetzen Datumsbereiche keine Aufbewahrungsfristen. Beispiel: Wenn die Aktivität, die Sie abfragen, eine Aufbewahrungsfrist von 90 Tagen hat und Sie „Letzte 100 Tage“ auswählen, werden nur Ergebnisse aus den letzten 90 Tagen zurückgegeben. Aufbewahrungsfristen für Aktivitäten [finden Sie hier](https://nation.marketo.com/t5/knowledgebase/marketo-activities-data-retention-policy/ta-p/251480){target="_blank"}.
1. **Einschränken von verschachtelten Smart-Listen -** Beschränken Sie beim Erstellen einer neuen Smart-Liste die Anzahl der verwendeten Filter „Mitglieder der Smart-Liste“. Dies wird als Verschachteln von Smart Lists bezeichnet. Jede Smart List, auf die verwiesen wird, verlängert die Verarbeitungszeit. Verweisen Sie stattdessen entweder auf statische Listen oder verwenden Sie [Segmentierung](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md){target="_blank"}.
1. **Positive über negative Operatoren verwenden -** Obwohl „Nicht“-Filter verfügbar sind, müssen sie den gesamten Datensatz in Ihrer Instanz durchsuchen, was extrem zeitaufwendig sein kann. Positive „is“-Filter können effektivere Suchalgorithmen nutzen.
1. **Vermeiden Sie „contains“ -** Wenn Sie nur partielle Daten haben, liefert „starts with“-Kriterien viel schnellere Ergebnisse als „contains“. „Is“ wird sogar noch schneller ausgeführt. Vermeiden Sie die Verwendung von „contains“ mit mehreren Werten; die beiden zusammen können eine Kampagne noch weiter verlangsamen.
1. **Zufallsprobe allein verwenden -** Zufallsprobe ist ein spezieller Filter. Nutzen Sie es für sich, um Ihre Leute in vorgefertigte Listen zu setzen. Verwenden Sie dann „Member of List“, um Ihre Smart List superschnell zu machen. Die zufällige Stichprobe **NICHT** mit verschachtelten Smart Lists. Der Filter Zufällige Stichprobe funktioniert nicht, wenn es sich um die Smart-Liste handelt, auf die für den Filter „Mitglied der Smart-Liste“ verwiesen wird.
1. **Seien Sie sparsam mit Inaktivitätsfiltern -** Filter wie „Nicht ausgefülltes Formular“ können wirklich nützlich sein, erfordern aber viel mehr Rechenleistung.
1. **Seien Sie sparsam mit dem Einfügen in mehrere Werte -** Multi-select ist zum Einfügen in Dutzende oder möglicherweise Hunderte von Werten konzipiert. Wenn man jedoch zu viele davon einbringt, wird man langsamer werden.
1. **sparsam sein beim Hinzufügen von Einschränkungen -** Dies sind die winzigen Details einer Regel und zugehörigen Werte. Je mehr Einschränkungen Sie hinzufügen, desto langsamer wird die Verarbeitungszeit.
1. **Vereinfachen Sie Ihre Kampagnen -** mehr als 100 unabhängige Regeln benötigen natürlich einige Zeit für die Verarbeitung. Halten Sie es einfach und Sie werden die Geschwindigkeitsgewinne bemerken - und es wird für Sie leichter zu verstehen sein.
1. **Bei Verwendung des E-Mail-Adressfilters muss vor dem Domain-Namen das @-Symbol** werden **-** Dadurch wird eine schnellere Abfrage verwendet. Beispiel: Verwenden Sie anstelle von _E-Mail enthält &#39;somedomain.com_ &quot;_enthält &#39;@somedomain.com_&quot;. Wenn Sie mehrere E-Mail-Adressen mit „contains“ verwenden, müssen ALLE mit &quot;@&quot; beginnen.

>[!TIP]
>
>Marketo Engage kann auf viele Arten verwendet werden und bestimmte Verfahren sind besser für Sie und Ihr Unternehmen. Wenden Sie sich an Ihren Adobe Professional Services-Vertriebsmitarbeiter, wenn Sie Unterstützung benötigen, um Ihre Investition optimal zu nutzen.
