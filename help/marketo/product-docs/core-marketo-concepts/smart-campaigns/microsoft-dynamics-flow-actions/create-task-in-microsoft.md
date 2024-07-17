---
unique-page-id: 37356429
description: Aufgabe in Microsoft erstellen - Marketo Docs - Produktdokumentation
title: Aufgabe in Microsoft erstellen
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# Aufgabe in Microsoft erstellen {#create-task-in-microsoft}

Als Marketing-Experte verfügen Sie über Informationen, die dem Vertrieb beim Abschluss von Geschäften helfen können. Sie können Aufgaben erstellen, um ihnen mitzuteilen, was sie tun und wann sie es tun sollten.

Aufgabe erstellen in Microsoft erstellt eine Aufgabe unter Aktivitäten, die mit der Person (Lead oder Kontakt) in [!DNL Microsoft] in Verbindung stehen.

>[!NOTE]
>
>Dieser Flussschritt funktioniert in Ihrer Smart-Kampagne nur bei Verwendung mit Triggern _, nicht mit Filtern._

Standardmäßig sieht der Flussschritt wie folgt aus:

![](assets/create-task-in-microsoft-1.png)

>[!NOTE]
>
>Wenn der Marketo-Synchronisierungsbenutzer Aufgaben erstellt, ist **[!UICONTROL Fällig in]** ein erforderliches Feld, damit die Aufgabe in [!DNL Microsoft] erstellt werden kann. Marketo gibt standardmäßig fünf Tage ein, wenn kein Wert eingegeben wird.

Passen Sie alle Felder an, um die Aufgabe wie gewünscht zu erstellen.

![](assets/create-task-in-microsoft-2.png)

>[!NOTE]
>
>Das Feld &quot;Status&quot;, das für die Aufgabe in der Flow-Aktion angegeben ist, aktualisiert das Feld: &quot;Status Reason&quot;in [!DNL Microsoft].

>[!TIP]
>
>Sie können `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` und `{{system.tokens}}` im **[!UICONTROL Betreff]** und in **[!UICONTROL Beschreibung]** verwenden. Weitere Informationen finden Sie unter [Token für Flussschritte](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} .
