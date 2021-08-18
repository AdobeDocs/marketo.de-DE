---
description: Ausführen von Campaign - Marketo Docs - Produktdokumentation
title: Kampagne ausführen
source-git-commit: 9f8d6895e88250afc2799b2fb7fc73442018362f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Kampagne ausführen {#execute-campaign}

Eine ausführbare Kampagne enthält wie andere Kampagnen eine Smart-Liste, einen Fluss und einen Zeitplan. Im Gegensatz zu anderen Kampagnen planen oder aktivieren Sie sie nicht. Sie kann nur von einer anderen Kampagne über den Schritt Kampagnenfluss ausführen aufgerufen werden. Die Workflow-Schritte in der ausführbaren Kampagne werden nacheinander mit der übergeordneten Kampagne ausgeführt (im Gegensatz zur Anforderungskampagne, die parallel in einer separaten Trigger-Kampagne ausgeführt wird).

>[!NOTE]
>
>Ausführbare Kampagnen sind immer untergeordnete Elemente der (übergeordneten) Kampagne, die sie aufruft.

## Verwendung von Execute Campaign {#when-to-use-execute-campaign}

Es gibt viele Dinge, die Sie mit einer ausführbaren Kampagne tun können. Sie sollen allgemeine operative Aufgaben wie Lead-Routing, Lebenszyklusverwaltung und Scoring (u. a.) erleichtern und können zur Ausführung desselben Workflows innerhalb von Batch oder ausgelösten Kampagnen verwendet werden.

Sie können sie auch verwenden, wenn Sie einen separaten Fluss ausführen müssen. Sie müssen jedoch von den Ergebnissen dieses Flusses in nachfolgenden Flussschritt-Optionen abhängig sein (d. h., wenn dies der Fall ist).

&quot;Kampagne ausführen&quot;ist eine Verbesserung gegenüber [Anforderungskampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/request-campaign.md), da sie in Serie oder parallel ausgeführt werden kann, während Letztere nur parallel ausgeführt wird.

>[!NOTE]
>
>Warteschritte und Webhooks sind nie mit ausführbaren Kampagnen kompatibel. Verwenden Sie dazu stattdessen Anforderungskampagne .

## Erstellen einer ausführbaren Kampagne {#how-to-create-an-executable-campaign}

1. Klicken Sie mit der rechten Maustaste auf das gewünschte Programm und wählen Sie **Neue Smart-Kampagne** aus.

   ![](assets/execute-campaign-1.png)

1. Geben Sie einen Namen ein, aktivieren Sie das Kontrollkästchen **Ausführbare Datei** und klicken Sie auf **Erstellen**.

   ![](assets/execute-campaign-2.png)

1. Definieren Sie die Smart-Liste und den Fluss wie jede andere Smart-Kampagne.

Sie können auch eine bestehende Smart-Kampagne klonen. Wenn Sie eine vorhandene ausführbare Kampagne klonen, müssen Sie nach der Benennung weiterhin das Kontrollkästchen **Ausführbare Datei** aktivieren.

>[!NOTE]
>
>Sie können eine Kampagne mit Triggern nicht klonen.

## Übergeordneten Kampagnen-Token-Kontext verwenden {#use-parent-campaign-token-context}

Wenn der Wert auf &quot;true&quot;gesetzt ist, werden die folgenden Token-Kontexte an die untergeordnete Kampagne gesendet (die ausgeführte Kampagne):

* Meine Token
* Kampagnen-Token
* Programm-Token
* Mitglieds-Token
* [Trigger-Token](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md)  (bei Aufruf über eine ausgelöste Kampagne)

**API-Interaktion**

Bei Verwendung von Plan oder Anforderungskampagne [in der API](https://developers.marketo.com/rest-api/assets/smart-campaigns/#batch) können Sie beide Werte für &quot;Meine Token&quot;übergeben, wodurch die für diese Token in der von Ihnen aufgerufenen Kampagne festgelegten Werte außer Kraft gesetzt werden. Wenn diese Kampagne dann eine andere Kampagne ausführt und &quot;Übergeordneten Kontext verwenden&quot;auf &quot;True&quot;setzt, verwendet sie die über die API übergebenen Werte und nicht die in der Anwendung festgelegten Werte.

## Zu beachten {#things-to-note}

* Die Smart-Liste filtert alle Personen heraus, die sich nicht qualifizieren. Wenn sich eine Person qualifiziert, werden sie im Aktivitätsdatensatz der resultierenden ausgeführten Kampagne als &quot;qualifiziert&quot;aufgeführt: TRUE&quot;(und FALSE, wenn nicht)
* Anwendung der Kampagnenqualifizierungsregeln planen (Einstellungen für intelligente Kampagnen auf der Registerkarte Plan )
* Ausführbare Kampagnen können nicht über Arbeitsbereiche hinweg aufgerufen werden
* Wenn Sie die Flussaktion [Aus Fluss entfernen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) verwenden, die auf eine ausführbare Kampagne abzielt, wird sowohl das untergeordnete als auch das übergeordnete Element angesprochen
* Nutzen der Token-Vererbung - Wenn Sie beispielsweise einen einzigen gemeinsamen Scoring-Fluss haben, der durch mehrere verschiedene Assets ausgelöst wird, können Sie in der untergeordneten Kampagne und in der übergeordneten Kampagne einen standardmäßigen My Token-Wert definieren, sodass Sie den untergeordneten Score-Kampagnenwert für Ihre übergeordneten Kampagnen überschreiben können (visuelles Beispiel siehe unten).
* Ausführbare Kampagnen können bis zu drei Ebenen tief aufgerufen werden (z. B. übergeordnete Kampagne > Untergeordnet > Untergeordnet > Untergeordnet).

>[!CAUTION]
>
>Lassen Sie Ihre Smart-Listen für ausführbare Kampagnen nie ungültig, sonst qualifiziert sich **niemand** dafür. Es empfiehlt sich, separate Smart-List-Assets zu erstellen, sie vollständig zu definieren und sicherzustellen, dass sie gültig sind. Verwenden Sie dann den Filter &quot;Mitglied der Smart-Liste&quot;in der ausführbaren Kampagne, um die Definition der Smart-Liste zu tauschen.

## Beispiel einer Token-Vererbung {#token-inheritance-example}

Nachstehend finden Sie ein visuelles Beispiel für die Token-Vererbung in einer ausführbaren Kampagne und in zwei übergeordneten Kampagnen: einer mit Token-Kontext auf **True**, der andere auf **False**.

Untergeordnete Kampagne mit einer Tokenisierten Änderungsbewertung.

![](assets/execute-campaign-3.png)

Die Token der Kinderkampagne.

![](assets/execute-campaign-4.png)

**Beispiel 1: true**

Im Schritt Kampagnenfluss ausführen der ersten übergeordneten Kampagne wird &quot;Übergeordneten Kampagnen-Token-Kontext verwenden&quot;auf **True** gesetzt.

![](assets/execute-campaign-5.png)

Die My Tokens der übergeordneten Kampagne.

![](assets/execute-campaign-6.png)

Die Ergebnisse: Wert um +10 geändert.

![](assets/execute-campaign-7.png)

**Beispiel 2: False**

Im Filter Kampagne ausführen der zweiten übergeordneten Kampagne ist der &quot;Kontext des übergeordneten Kampagnen-Tokens verwenden&quot;auf **False** gesetzt.

![](assets/execute-campaign-8.png)

Die My Tokens der übergeordneten Kampagne.

![](assets/execute-campaign-9.png)

Die Ergebnisse: Wert unverändert bleibt, da der Punktwert der untergeordneten Kampagne, +0, verwendet wurde.

![](assets/execute-campaign-10.png)
