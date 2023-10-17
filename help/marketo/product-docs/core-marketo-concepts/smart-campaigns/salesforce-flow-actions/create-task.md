---
unique-page-id: 1147017
description: Aufgabe erstellen - Marketo-Dokumente - Produktdokumentation
title: Aufgabe erstellen
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 3%

---

# Aufgabe erstellen {#create-task}

Als Marketing-Experte verfügen Sie über Informationen, die dem Vertrieb beim Abschluss von Geschäften helfen können. Sie können Aufgaben erstellen, um ihnen mitzuteilen, was sie tun und wann sie es tun sollten.

![](assets/image2014-9-22-14-3a54-3a46.png)

>[!NOTE]
>
>Wenn der Marketo Sync User Aufgaben erstellt, **[!UICONTROL aufgrund von]** ist ein erforderliches Feld für die Aufgabe, die in Salesforce erstellt werden soll. Marketo gibt standardmäßig fünf Tage ein, wenn kein Wert vorhanden ist.

Standardmäßig sieht der Flussschritt wie folgt aus:

![](assets/image2014-9-22-14-3a54-3a49.png)

Passen Sie alle Felder an, um die Aufgabe wie gewünscht zu erstellen.

![](assets/image2014-9-22-14-3a54-3a52.png)

>[!TIP]
>
>Sie können `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` und `{{system.tokens}}` im **[!UICONTROL Betreff]** und **[!UICONTROL Beschreibung]**. Siehe [Token für Flussschritte](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} für weitere Details.
