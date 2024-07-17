---
unique-page-id: 1146950
description: Warten - Marketo-Dokumente - Produktdokumentation
title: Warten
exl-id: 58f43c4b-6f20-4740-9a25-e09c7ea31dcf
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Warteübersicht {#wait-overview}

Halten Sie eine Person in einem Fluss mit intelligenter Kampagne an, indem Sie den praktischen **Warteschritt** verwenden.

![](assets/wait-overview-1.png)

Beachten Sie, wie Sie in natürliche Sprache eingeben können, z. B. &quot;4 Stunden&quot;. Nehmen Sie jedoch **nicht** vor, kürzen Sie die Wörter (d. h. 4 Stunden). Die intelligente Kampagne würde weiterhin laufen, aber der Warteschritt würde ignoriert.

>[!CAUTION]
>
>Eine Änderung der Dauer eines Warteschritts wirkt sich nicht auf Personen aus, die bereits in diesen Schritt eingetreten sind. Beispiel: Sie haben einen Warteschritt für 5 Tage, eine Person tritt ihn ein, dann ändern Sie den Warteschritt auf 7 Tage - diese Person wartet immer noch die ursprünglichen 5 Tage, bevor sie zum nächsten Flussschritt übergeht.

>[!TIP]
>
>Wenn sich bereits jemand in einem Warteschritt befindet und Sie nicht möchten, dass er nach Ende der Wartezeit fortfährt, fügen Sie &quot;[remove from flow](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md)&quot;direkt nach dem Warteschritt ein. Geben Sie mit der Option [Auswahl hinzufügen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md) an, wer entfernt werden soll.

Es gibt drei Möglichkeiten, einen Schritt zum Warten zu verwenden:

1. [Verwenden einer Dauer in einem Warteflussschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [Verwenden eines bestimmten Datums in einem Warteflussschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [Verwenden eines Datums-Tokens in einem Warteflussschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
