---
description: Kampagne ausführen - Marketo Docs - Produktdokumentation
title: Kampagne ausführen
translation-type: tm+mt
source-git-commit: 20a3bee9973340d7b772532d1be31fe745e5ffd7
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 1%

---

# Kampagne ausführen {#execute-campaign}

Eine ausführbare Kampagne enthält wie andere Kampagnen eine intelligente Liste, einen Fluss und einen Zeitplan. Im Gegensatz zu anderen Kampagnen planen oder aktivieren Sie sie nicht. Sie kann nur von einer anderen Kampagne über den Flussschritt Kampagne ausführen aufgerufen werden. Die Flussschritte in der ausführbaren Kampagne werden nacheinander mit der übergeordneten Kampagne ausgeführt (im Gegensatz zur Request-Kampagne, die parallel in einer separaten Trigger-Kampagne ausgeführt wird).

>[!NOTE]
>
>Ausführbare Kampagnen sind immer untergeordnete Elemente der (übergeordneten) Kampagne, die sie aufruft.

## Verwenden der Execute-Kampagne {#when-to-use-execute-campaign}

Es gibt viele Dinge, die Sie mit einer ausführbaren Kampagne tun können. Sie sollen allgemeine betriebliche Aufgaben wie Interessentenanwerbung, Lebenszyklusmanagement und Scoring (u. a.) erleichtern und können dazu verwendet werden, den gleichen Arbeitsablauf aus Batch- oder Trigger-Kampagnen auszuführen.

Sie können sie auch dann verwenden, wenn Sie einen separaten Fluss ausführen müssen, aber Sie müssen bei den folgenden Flussstufenoptionen von den Ergebnissen dieses Flusses abhängig sein (d. h., wenn dies der Fall ist).

Die Execute-Kampagne ist eine Verbesserung bei [Request-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/request-campaign.md), da sie in Serie oder parallel ausgeführt werden kann, während Letztere nur parallel ausgeführt wird.

>[!NOTE]
>
>Warteschritte und Webhooks sind nie mit ausführbaren Kampagnen kompatibel. Dafür müssen Sie stattdessen die Kampagne Anfordern verwenden.

## Erstellen einer ausführbaren Kampagne {#how-to-create-an-executable-campaign}

1. Klicken Sie mit der rechten Maustaste auf das gewünschte Programm und wählen Sie **Neue Smart-Kampagne**.

   ![](assets/execute-campaign-1.png)

1. Geben Sie einen Namen ein, aktivieren Sie das Kontrollkästchen **Ausführbare Datei** und klicken Sie auf **Erstellen**.

   ![](assets/execute-campaign-2.png)

1. Definieren Sie die intelligente Liste und den intelligenten Fluss wie jede andere intelligente Kampagne.

Sie können auch eine vorhandene intelligente Kampagne klonen. Wenn Sie eine vorhandene ausführbare Kampagne klonen, müssen Sie nach der Benennung weiterhin das Kontrollkästchen **Ausführbare Datei** aktivieren.

>[!NOTE]
>
>Eine Kampagne mit Triggern kann nicht geklont werden.

## Übergeordneter Token-Kontext für Kampagnen verwenden {#use-parent-campaign-token-context}

Bei der Einstellung &quot;true&quot;werden die folgenden Token-Kontexte an die untergeordnete Kampagne gesendet (die ausgeführte):

* Meine Token
* Kampagnen-Tokens
* Programm-Token
* Tokens für Mitglieder
* [Trigger-Token](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md)  (falls aus einer ausgelösten Kampagne aufgerufen)

**API-Interaktion**

Bei Verwendung von Plan- oder Anforderungs-Kampagne [in der API](https://developers.marketo.com/rest-api/assets/smart-campaigns/#batch) können Sie beide Werte für &quot;Meine Token&quot;übergeben, wodurch die für diese Token in der aufzurufenden Kampagne festgelegten Werte außer Kraft gesetzt werden. Wenn diese Kampagne dann eine andere Kampagne ausführt und &quot;Übergeordneten Kontext verwenden&quot;auf &quot;True&quot;setzt, verwendet sie statt der in der Anwendung festgelegten Werte die über die API weitergeleiteten Werte.

## Dinge zu beachten {#things-to-note}

* Die intelligente Liste filtert alle, die sich nicht qualifizieren. Qualifiziert sich eine Person, werden sie im Ergebnisdatensatz zur Aktivität der ausgeführten Kampagne als &quot;Qualifiziert&quot; Liste: TRUE&quot;(und FALSE, wenn nicht)
* Es gelten Regeln zur Kampagne planen (Einstellungen für intelligente Kampagne unter der Registerkarte Plan)
* Ausführbare Kampagnen können nicht über mehrere Arbeitsbereiche hinweg aufgerufen werden
* Wenn Sie die Fließaktion [Aus Fluss entfernen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) für eine ausführbare Kampagne verwenden, wird sowohl das untergeordnete als auch das übergeordnete Element Zielgruppe
* Nutzen der Token-Vererbung - Wenn Sie z. B. einen einzigen gemeinsamen Bewertungsfluss haben, der durch mehrere verschiedene Assets ausgelöst wird, können Sie in der untergeordneten Kampagne und in der übergeordneten Kampagne ein standardmäßiges My Token-Ergebnis definieren, sodass Sie den Wert der Kampagne der untergeordneten Punktzahl für Ihre übergeordneten Kampagnen außer Kraft setzen können (siehe das folgende Beispiel)
* Die Verschachtelung ausführbarer Kampagnen ist derzeit nicht verfügbar, wird jedoch in einer kommenden Version verfügbar sein

>[!CAUTION]
>
>Lassen Sie Ihre intelligenten Listen für ausführbare Kampagnen nie ungültig, sonst ist **niemand** berechtigt. Es empfiehlt sich, separate Assets mit intelligenter Liste zu erstellen, diese vollständig zu definieren und sicherzustellen, dass sie gültig sind. Verwenden Sie dann den Filter &quot;Member of Smart Liste&quot;in der ausführbaren Kampagne, damit Sie die Definition der Smart-Liste austauschen können.

## Beispiel für Token-Vererbung {#token-inheritance-example}

Nachstehend finden Sie ein visuelles Beispiel für die Token-Vererbung in einer ausführbaren Kampagne und zwei übergeordneten Kampagnen: einer mit Token-Kontext, der auf **True** gesetzt ist, der andere auf **False**.

Untergeordnete Kampagne mit einer Token-Bewertung für Änderungen.

![](assets/execute-campaign-3.png)

Die Kindertoken der Kampagne.

![](assets/execute-campaign-4.png)

**Beispiel 1: true**

Im Flussschritt zur Ausführung der Kampagne der ersten übergeordneten Kampagne ist &quot;Übergeordneter Token-Kontext verwenden&quot;auf **True** eingestellt.

![](assets/execute-campaign-5.png)

Die My Tokens der übergeordneten Kampagne.

![](assets/execute-campaign-6.png)

Die Ergebnisse: Das Ergebnis wurde um +10 geändert.

![](assets/execute-campaign-7.png)

**Beispiel 2: False**

Im Filter Kampagne ausführen der zweiten übergeordneten Kampagne ist &quot;Kontext für übergeordnete Kampagne verwenden&quot;auf **False** eingestellt.

![](assets/execute-campaign-8.png)

Die My Tokens der übergeordneten Kampagne.

![](assets/execute-campaign-9.png)

Die Ergebnisse: Wert unverändert, da der Wert +0 der untergeordneten Kampagne verwendet wurde.

![](assets/execute-campaign-10.png)
