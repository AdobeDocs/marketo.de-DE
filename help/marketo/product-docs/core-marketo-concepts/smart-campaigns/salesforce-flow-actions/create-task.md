---
unique-page-id: 1147017
description: Erfahren Sie, wie Sie in einem Flussschritt eine Salesforce-Aufgabe erstellen. Erstellen Sie eine Aufgabe für den Lead-Eigentümer, wenn jemand in den Fluss eintritt.
title: Erstellen von Aufgaben
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/RJ5nZrVvURtgXEWWZwL2xXzlYOhWjKGSbX-MFTWCwzg
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 130
ht-degree: 3%

---

# Erstellen von Aufgaben {#create-task}

Als Marketing-Experte verfügen Sie über Informationen, die den Vertrieb beim Abschluss von Abschlüssen unterstützen können. Sie können Aufgaben erstellen, um ihnen mitzuteilen, was und wann sie tun sollten.

![](assets/create-task-1.png)

>[!NOTE]
>
>Wenn der Marketo-Synchronisierungsbenutzer Aufgaben erstellt **[!UICONTROL ist &quot;]**&quot; ein Pflichtfeld, damit die Aufgabe in Salesforce erstellt wird. Marketo gibt standardmäßig fünf Tage ein, wenn kein Wert vorhanden ist.

Standardmäßig sieht der Flussschritt wie folgt aus:

![](assets/create-task-2.png)

Passen Sie alle Felder an, um die Aufgabe wie gewünscht zu erstellen.

![](assets/create-task-3.png)

>[!TIP]
>
>Sie können `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` und `{{system.tokens}}` in den **[!UICONTROL Betreff]** und **[!UICONTROL Beschreibung]**. Weitere [ finden Sie unter ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} für Flussschritte .
