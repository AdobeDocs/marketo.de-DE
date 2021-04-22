---
unique-page-id: 37356429
description: Aufgabe in Microsoft - Marketo Docs - Produktdokumentation erstellen
title: Aufgabe in Microsoft erstellen
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Aufgabe in Microsoft {#create-task-in-microsoft} erstellen

Als Marketingspezialist verfügen Sie über Informationen, die dem Vertrieb beim Abschluss von Geschäften helfen können. Sie können Aufgaben erstellen, um ihnen mitzuteilen, was sie tun und wann sie es tun sollten.

Erstellen Sie Aufgabe in Microsoft erstellt eine Aufgabe unter Aktivitäten, die mit der Person (Lead oder Kontakt) in Microsoft zu tun haben.

>[!NOTE]
>
>Dieser Flussschritt funktioniert nur, wenn er mit Triggern **, nicht mit Filtern, in Ihrer intelligenten Kampagne verwendet wird.**

Standardmäßig sieht der Flussschritt wie folgt aus:

![](assets/msd1.png)

>[!NOTE]
>
>Wenn der Marketo Sync User Aufgaben erstellt, ist **Due In** ein erforderliches Feld, damit die Aufgabe in Microsoft erstellt werden kann. Marketo gibt standardmäßig fünf Tage ein, wenn kein Wert eingegeben wurde.

Passen Sie alle Felder an, um die Aufgabe wie gewünscht zu erstellen.

![](assets/msd2.png)

>[!NOTE]
>
>Das für die Aufgabe in der Flussaktion angegebene Feld &quot;Status&quot;aktualisiert das Feld: &quot;Statusgrund&quot;in Microsoft.

>[!TIP]
>
>Sie können `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` und `{{system.tokens}}` in den **Betreff** und **Beschreibung** verwenden. Weitere Informationen finden Sie unter [Token für Flussschritte](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).
