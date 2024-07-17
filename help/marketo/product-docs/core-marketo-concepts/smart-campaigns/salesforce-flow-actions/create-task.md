---
unique-page-id: 1147017
description: Aufgabe erstellen - Marketo-Dokumente - Produktdokumentation
title: Aufgabe erstellen
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 3%

---

# Aufgabe erstellen {#create-task}

Als Marketing-Experte verfügen Sie über Informationen, die dem Vertrieb beim Abschluss von Geschäften helfen können. Sie können Aufgaben erstellen, um ihnen mitzuteilen, was sie tun und wann sie es tun sollten.

![](assets/create-task-1.png)

>[!NOTE]
>
>Wenn der Marketo-Synchronisierungsbenutzer Aufgaben erstellt, ist **[!UICONTROL Fälliger in]** ein erforderliches Feld, damit die Aufgabe in Salesforce erstellt werden kann. Marketo gibt standardmäßig fünf Tage ein, wenn kein Wert vorhanden ist.

Standardmäßig sieht der Flussschritt wie folgt aus:

![](assets/create-task-2.png)

Passen Sie alle Felder an, um die Aufgabe wie gewünscht zu erstellen.

![](assets/create-task-3.png)

>[!TIP]
>
>Sie können `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` und `{{system.tokens}}` im **[!UICONTROL Betreff]** und in **[!UICONTROL Beschreibung]** verwenden. Weitere Informationen finden Sie unter [Token für Flussschritte](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} .
