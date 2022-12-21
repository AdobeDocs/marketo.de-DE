---
unique-page-id: 37356429
description: Aufgabe in Microsoft erstellen - Marketo Docs - Produktdokumentation
title: Aufgabe in Microsoft erstellen
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Aufgabe in Microsoft erstellen {#create-task-in-microsoft}

Als Marketing-Experte verfügen Sie über Informationen, die dem Vertrieb beim Abschluss von Angeboten helfen können. Sie können Aufgaben erstellen, um ihnen mitzuteilen, was sie tun und wann sie es tun sollten.

Aufgabe erstellen in Microsoft erstellt eine Aufgabe unter Aktivitäten, die sich auf die Person (Lead oder Kontakt) in Microsoft beziehen.

>[!NOTE]
>
>Dieser Flussschritt **funktioniert nur bei Verwendung mit Triggern**, nicht Filter, in Ihrer Smart-Kampagne verwenden.

Standardmäßig sieht der Flussschritt wie folgt aus:

![](assets/msd1.png)

>[!NOTE]
>
>Wenn der Marketo Sync User Aufgaben erstellt, **aufgrund von** ist ein erforderliches Feld für die Aufgabe, die in Microsoft erstellt werden soll. Marketo gibt standardmäßig fünf Tage ein, wenn kein Wert eingegeben wird.

Passen Sie alle Felder an, um die Aufgabe wie gewünscht zu erstellen.

![](assets/msd2.png)

>[!NOTE]
>
>Das Feld &quot;Status&quot;, das für die Aufgabe in der Flussaktion angegeben ist, aktualisiert das Feld: &quot;Statusgrund&quot;in Microsoft.

>[!TIP]
>
>Sie können `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` und `{{system.tokens}}` im **Betreff** und **Beschreibung**. Siehe [Token für Flussschritte](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md) für weitere Details.
