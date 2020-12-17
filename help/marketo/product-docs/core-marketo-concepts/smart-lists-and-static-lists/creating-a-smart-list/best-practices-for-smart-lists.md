---
unique-page-id: 7512524
description: Best Practices für intelligente Listen - Marketing-Dokumente - Produktdokumentation
title: Best Practices für intelligente Listen
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---


# Best Practices für intelligente Listen {#best-practices-for-smart-lists}

Intelligente Listen sind das leistungsfähigste Werkzeug zur Abfrage im Marketing-Universum. Sie finden die Leute, die Sie suchen mit magischer Geschwindigkeit und Leichtigkeit.

Um ihnen die Arbeit zu erleichtern und die Leistung zu optimieren, haben wir eine Liste bewährter Verfahren entwickelt. Viel Spaß!

>[!NOTE]
>
>**Jeder Kunde ist anders.** Je größer die Datenbank, desto mehr Verarbeitung erfolgt. Je mehr Aktivitäten Sie gespeichert haben, desto länger dauert es, sie zu durchsuchen.
>
>Wenn Sie eine Langsamkeit erleben, versuchen Sie die unten stehenden Tipps. Wenn das Problem weiterhin besteht, wenden Sie sich an Marketo [Support](http://support.marketo.com).

1. **Limit history - **History Filters (alias Aktivität-Filter) gehören zu den ressourcenintensivsten und zeitaufwendigsten Abläufen. Wenn Sie diese verwenden müssen, versuchen Sie, den Datumsbereich so kurz wie möglich zu beschränken, wodurch der durchsuchbare Datensatz reduziert wird.
1. **Verschachtelte intelligente Listen begrenzen - **Beim Erstellen einer neuen intelligenten Liste sollten Sie die Anzahl der verwendeten Filter für &quot;Mitglied der intelligenten Liste&quot;begrenzen. Dies wird als Verschachtelung intelligenter Listen bezeichnet. Jede referenzierte intelligente Liste verlängert die Verarbeitungszeit. Verweisen Sie stattdessen entweder auf statische Listen oder verwenden Sie [segmentation](../../../../product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md).
1. **Verwenden Sie positive und negative Operatoren - **Obwohl &quot;nicht&quot;-Filter verfügbar sind, müssen sie den gesamten Datensatz in Ihrer Instanz durchsuchen, was sehr zeitaufwendig sein kann. Positive &quot;is&quot;-Filter können effektivere Suchalgorithmen nutzen.
1. **Vermeiden Sie &quot;enthält&quot;-** Wenn Sie nur partielle Daten haben, führen &quot;Beginn mit&quot;zu wesentlich schnelleren Ergebnissen als &quot;enthält&quot;. &quot;Ist&quot;läuft sogar noch schneller. Vermeiden Sie die Verwendung von &quot;contains&quot;mit mehreren Werten; Die beiden zusammen können eine Kampagne noch weiter verlangsamen.
1. **Eigenes Random-Beispiel verwenden - **Random-Beispiel ist ein Sonderfilter. Benutzen Sie es selbst, um Ihre Leute in vorgefertigte Listen zu setzen. Dann verwenden Sie einfach &quot;Member of Liste&quot;, um Ihre intelligente Liste super schnell zu machen. Random Sample funktioniert **NOT** mit verschachtelten Smart-Listen. Der Filter &quot;Random-Beispiel&quot;funktioniert nicht, wenn auf die Smart-Liste für den Filter &quot;Member of Smart Liste&quot;verwiesen wird.
1. **Sparsam mit inaktiven Filtern - **Filter wie &quot;Nicht ausgefülltes Formular&quot;können sehr nützlich sein, erfordern aber viel mehr Verarbeitungsleistung.
1. **Beim Einfügen mehrerer Werte sparsam sein - **Multi-select wurde zum Einfügen in Dutzende oder möglicherweise Hunderte von Werten entwickelt. Aber lassen Sie zu viele hinein, und es wird langsamer werden.
1. **Seien Sie beim Hinzufügen von Beschränkungen sparsam - **Dies sind die winzigen Details einer Regel und verwandter Werte. Je mehr Einschränkungen Sie hinzufügen, desto langsamer wird die Verarbeitungszeit.
1. **Vereinfachung Ihrer Kampagnen - **100+ unabhängige Regeln (wir haben sie gesehen!) werden natürlich einige Zeit in Anspruch nehmen. Halten Sie es einfach und Sie werden die Geschwindigkeit zu spüren - plus es wird einfacher für Sie zu verstehen.
1. **Wenn Sie den Filter** **&quot;E-Mail-Adresse&quot;verwenden, müssen Sie das @-Symbol vor dem Domänennamen einfügen.** Dadurch wird eine schnellere Abfrage verwendet. Beispiel: Anstatt *email enthält &#39;somedomain.com*&#39;, verwenden Sie *email contains &#39;@somedomain.com*&#39;. Wenn Sie mehrere E-Mail-Adressen mit &quot;contains&quot;verwenden, müssen ALLE von ihnen mit &quot;@&quot;Beginn werden.

>[!TIP]
>
>Marketo kann auf vielfältige Weise eingesetzt werden und bestimmte Techniken sind besser für Sie und Ihr Unternehmen. Erwägen Sie [Marketo Professional Services](http://pages2.marketo.com/72-hour-survival-guide.html), um Ihre Investition zu glänzen.

