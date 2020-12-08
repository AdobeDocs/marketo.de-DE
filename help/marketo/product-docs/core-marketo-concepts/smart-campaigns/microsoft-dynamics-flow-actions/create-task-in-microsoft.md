---
unique-page-id: 37356429
description: Aufgabe in Microsoft - Marketing Docs - Produktdokumentation erstellen
title: Aufgabe in Microsoft erstellen
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Aufgabe in Microsoft erstellen {#create-task-in-microsoft}

Als Marketingspezialist verfügen Sie über Informationen, die dem Vertrieb beim Abschluss von Geschäften helfen können. Sie können Aufgaben erstellen, um ihnen mitzuteilen, was sie tun und wann sie es tun sollten.

Erstellen Sie Aufgabe in Microsoft erstellt eine Aufgabe unter Aktivitäten, die mit der Person (Lead oder Kontakt) in Microsoft zu tun haben.

>[!NOTE]
>
>Dieser Flussschritt funktioniert **nur, wenn er mit Auslösern** und nicht mit Filtern in Ihrer intelligenten Kampagne verwendet wird.

Standardmäßig sieht der Flussschritt wie folgt aus:   ![](assets/msd1.png)

>[!NOTE]
>
>Wenn der Benutzer &quot;Markieren synchronisieren&quot;Aufgaben erstellt, ist **Aufgrund in **ein erforderliches Feld, damit die Aufgabe in Microsoft erstellt werden kann. Marketo gibt standardmäßig fünf Tage ein, wenn kein Wert eingegeben wurde.

Passen Sie alle Felder an, um die Aufgabe wie gewünscht zu erstellen.   ![](assets/msd2.png)

>[!NOTE]
>
>Das für die Aufgabe in der Flussaktion angegebene Feld &quot;Status&quot;aktualisiert das Feld: &quot;Statusgrund&quot;in Microsoft.

>[!TIP]
>
>Sie können `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` und `{{system.tokens}}` im **Betreff** und in der **Beschreibung** verwenden. Weitere Informationen finden Sie unter [Tokens für Flussschritte](http://docs.marketo.com/x/c4AR) .

