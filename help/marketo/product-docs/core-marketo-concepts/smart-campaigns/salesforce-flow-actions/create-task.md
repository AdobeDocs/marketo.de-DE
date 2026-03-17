---
unique-page-id: 1147017
description: Erfahren Sie, wie Sie in einem Flussschritt eine Salesforce-Aufgabe erstellen. Erstellen Sie eine Aufgabe für den Lead-Eigentümer, wenn jemand in den Fluss eintritt.
title: Erstellen von Aufgaben
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 3efcb529cd3e35027f35e51dfd91f95e94af9d61
workflow-type: tm+mt
source-wordcount: '130'
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
>Sie können `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` und `{{system.tokens}}` in den **[!UICONTROL Betreff]** und **[!UICONTROL Beschreibung]**. Weitere [&#x200B; finden Sie unter &#x200B;](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} für Flussschritte .
