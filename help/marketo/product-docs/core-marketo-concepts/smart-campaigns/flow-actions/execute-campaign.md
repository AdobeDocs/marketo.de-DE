---
description: Ausführen von Campaign - Marketo Docs - Produktdokumentation
title: Kampagne ausführen
exl-id: d550cf08-b295-4289-9bb0-79d81cabc245
feature: Smart Campaigns
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# Kampagne ausführen {#execute-campaign}

Eine ausführbare Kampagne enthält wie andere Kampagnen eine Smart-Liste, einen Fluss und einen Zeitplan. Im Gegensatz zu anderen Kampagnen planen oder aktivieren Sie sie nicht. Sie kann nur von einer anderen Kampagne über den Schritt Kampagnenfluss ausführen aufgerufen werden. Die Workflow-Schritte in der ausführbaren Kampagne werden nacheinander mit der übergeordneten Kampagne ausgeführt (im Gegensatz zur Anforderungskampagne, die parallel in einer separaten Trigger-Kampagne ausgeführt wird).

>[!NOTE]
>
>Ausführbare Kampagnen sind immer untergeordnete Elemente der (übergeordneten) Kampagne, die sie aufruft.

## Verwendung von Execute Campaign {#when-to-use-execute-campaign}

Es gibt viele Dinge, die Sie mit einer ausführbaren Kampagne tun können. Sie sollen allgemeine operative Aufgaben wie Lead-Routing, Lebenszyklusverwaltung und Scoring (u. a.) erleichtern und können zur Ausführung desselben Workflows innerhalb von Batch oder ausgelösten Kampagnen verwendet werden.

Sie können sie auch verwenden, wenn Sie einen separaten Fluss ausführen müssen. Sie müssen jedoch von den Ergebnissen dieses Flusses in nachfolgenden Flussschritt-Optionen abhängig sein (d. h., wenn dies der Fall ist).

&quot;Kampagne ausführen&quot;ist eine Verbesserung gegenüber [Kampagne anfordern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/request-campaign.md), da sie in einer Reihe ausgeführt werden kann, während Letztere nur parallel ausgeführt wird.

>[!NOTE]
>
>Warteschritte und Webhooks sind nie mit ausführbaren Kampagnen kompatibel. Verwenden Sie dazu stattdessen Anforderungskampagne .

## Erstellen einer ausführbaren Kampagne {#how-to-create-an-executable-campaign}

1. Klicken Sie mit der rechten Maustaste auf das gewünschte Programm und wählen Sie **[!UICONTROL Neue Smart-Kampagne]** aus.

   ![](assets/execute-campaign-1.png)

1. Geben Sie ihm einen Namen, aktivieren Sie das Kontrollkästchen **[!UICONTROL Ausführbare Datei]** und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/execute-campaign-2.png)

1. Definieren Sie die Smart-Liste und den Fluss wie jede andere Smart-Kampagne.

Sie können auch eine bestehende Smart-Kampagne klonen. Wenn Sie eine vorhandene ausführbare Kampagne klonen, müssen Sie nach der Benennung weiterhin das Kontrollkästchen **[!UICONTROL Ausführbare Datei]** aktivieren.

>[!NOTE]
>
>Sie können eine Kampagne mit Triggern nicht klonen.

## Token-Kontext der übergeordneten Kampagne verwenden {#use-parent-campaign-token-context}

Wenn der Wert auf &quot;true&quot;gesetzt ist, werden die folgenden Token-Kontexte an die untergeordnete Kampagne gesendet (die ausgeführte Kampagne):

* Meine Token
* Kampagnen-Token
* Programm-Token
* Mitglieds-Token
* [Trigger-Token](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) (wenn von einer ausgelösten Kampagne aufgerufen)

**API-Interaktion**

Bei Verwendung von Plan oder Anforderungskampagne [ in der API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/assets/smart-campaigns#batch) können Sie beide Werte für &quot;Meine Token&quot;übergeben, wodurch die für diese Token in der von Ihnen aufgerufenen Kampagne festgelegten Werte außer Kraft gesetzt werden. Wenn diese Kampagne dann eine andere Kampagne ausführt und &quot;Übergeordneten Kontext verwenden&quot;auf &quot;True&quot;setzt, verwendet sie die über die API übergebenen Werte und nicht die in der Anwendung festgelegten Werte.

## Zu beachten {#things-to-note}

* Die Smart-Liste filtert alle Personen heraus, die sich nicht qualifizieren. Wenn sich eine Person qualifiziert, werden sie im Aktivitätsdatensatz &quot;Ausgeführte Kampagne&quot;als &quot;Qualifiziert: TRUE&quot;aufgeführt (und FALSE, wenn dies nicht der Fall ist).
* Anwendung der Kampagnenqualifizierungsregeln planen (Einstellungen für intelligente Kampagnen auf der Registerkarte Plan )
* Ausführbare Kampagnen können nicht über Arbeitsbereiche hinweg aufgerufen werden
* Wenn Sie die Flussaktion [Aus Fluss entfernen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) verwenden, die auf eine ausführbare Kampagne ausgerichtet ist, wird sowohl das untergeordnete als auch das übergeordnete Element ausgewählt
* Nutzen der Token-Vererbung - Wenn Sie beispielsweise einen einzigen gemeinsamen Scoring-Fluss haben, der durch mehrere verschiedene Assets ausgelöst wird, können Sie in der untergeordneten Kampagne und in der übergeordneten Kampagne einen standardmäßigen My Token-Wert definieren, sodass Sie den untergeordneten Score-Kampagnenwert für Ihre übergeordneten Kampagnen überschreiben können (siehe unten für visuelles Beispiel).
* Ausführbare Kampagnen können bis zu drei Ebenen tief aufgerufen werden (z. B. übergeordnete Kampagne > Untergeordnet > Untergeordnet > Untergeordnet).

>[!CAUTION]
>
>Lassen Sie Ihre Smart-Listen für ausführbare Kampagnen nie ungültig, da sonst _niemand_ dafür qualifiziert ist. Es empfiehlt sich, separate Smart-List-Assets zu erstellen, sie vollständig zu definieren und sicherzustellen, dass sie gültig sind. Verwenden Sie dann den Filter &quot;Mitglied der Smart-Liste&quot;in der ausführbaren Kampagne, um die Definition der Smart-Liste zu tauschen.

## Beispiel einer Token-Vererbung {#token-inheritance-example}

Nachstehend finden Sie ein visuelles Beispiel für die Token-Vererbung in einer ausführbaren Kampagne und in zwei übergeordneten Kampagnen: eine mit Token-Kontext, der auf **[!UICONTROL True]** und die andere auf **[!UICONTROL False]** festgelegt ist.

Untergeordnete Kampagne mit einer Tokenisierten Änderungsbewertung.

![](assets/execute-campaign-3.png)

Die Token der Kinderkampagne.

![](assets/execute-campaign-4.png)

### Beispiel 1: true {#example-one-true}

Im Schritt Kampagnenfluss ausführen der ersten übergeordneten Kampagne ist &quot;Übergeordneten Kampagnen-Token-Kontext verwenden&quot;auf **True** eingestellt.

![](assets/execute-campaign-5.png)

Die My Tokens der übergeordneten Kampagne.

![](assets/execute-campaign-6.png)

Die Ergebnisse: Die Punktzahl wurde um +10 geändert.

![](assets/execute-campaign-7.png)

### Beispiel 2: False {#example-two-false}

Im Schritt Kampagnenfluss ausführen der zweiten übergeordneten Kampagne ist &quot;Übergeordneten Kampagnen-Token-Kontext verwenden&quot;auf **False** eingestellt.

![](assets/execute-campaign-8.png)

Die My Tokens der übergeordneten Kampagne.

![](assets/execute-campaign-9.png)

Die Ergebnisse: Die Punktzahl bleibt unverändert, da der Punktwert der untergeordneten Kampagne, +0, verwendet wurde.

![](assets/execute-campaign-10.png)
