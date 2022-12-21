---
unique-page-id: 1146950
description: Warten - Marketo-Dokumente - Produktdokumentation
title: Warten
exl-id: 58f43c4b-6f20-4740-9a25-e09c7ea31dcf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 2%

---

# Warten {#wait}

## Überblick {#overview}

Halten Sie eine Person in einem intelligenten Kampagnenfluss mit dem Handlichen an **Warteschritt**.

![](assets/wait-overview.png)

Beachten Sie, wie Sie in natürliche Sprache wie &quot;4 Stunden&quot;eingeben können. Do **not** Abkürzung: 4 Stunden. Die intelligente Kampagne würde weiterhin laufen, aber der Warteschritt würde ignoriert.

>[!CAUTION]
>
>Eine Änderung der Dauer eines Warteschritts wirkt sich nicht auf Personen aus, die bereits in diesen Schritt eingetreten sind. Beispiel: Wenn Sie einen Warteschritt für 5 Tage haben, tritt eine Person ein, dann ändern Sie den Warteschritt in 7 Tage - diese Person wird immer noch nur die ursprünglichen 5 Tage warten, bevor sie zum nächsten Flussschritt übergeht.

>[!TIP]
>
>Wenn Sie bereits in einem Warteschritt sind und nicht möchten, dass sie nach Ablauf der Wartezeit weitergehen, fügen Sie [Aus Fluss entfernen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) direkt nach dem Warteschritt. Geben Sie mithilfe der [Auswahl hinzufügen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md) -Option.

## Nutzung {#usage}

Es gibt drei Möglichkeiten, einen Schritt zum Warten zu verwenden:

1. [Verwenden einer Dauer in einem Warteflussschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [Verwenden eines bestimmten Datums in einem Warteflussschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [Verwenden eines Datums-Tokens in einem Warteflussschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
