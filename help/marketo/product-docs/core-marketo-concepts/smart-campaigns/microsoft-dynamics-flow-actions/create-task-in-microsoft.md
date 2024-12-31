---
unique-page-id: 37356429
description: Aufgabe in Microsoft erstellen - Marketo-Dokumente - Produktdokumentation
title: Aufgabe in Microsoft erstellen
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# Aufgabe in Microsoft erstellen {#create-task-in-microsoft}

Als Marketing-Experte verfügen Sie über Informationen, die den Vertrieb beim Abschluss von Abschlüssen unterstützen können. Sie können Aufgaben erstellen, um ihnen mitzuteilen, was und wann sie tun sollten.

Aufgabe erstellen in Microsoft erstellt eine Aufgabe unter Aktivitäten, die sich auf die Person (Lead oder Kontakt) in [!DNL Microsoft] beziehen.

>[!NOTE]
>
>Dieser Flussschritt funktioniert _nur bei Verwendung mit Triggern_ nicht mit Filtern in Ihrer Smart-Kampagne.

Standardmäßig sieht der Flussschritt wie folgt aus:

![](assets/create-task-in-microsoft-1.png)

>[!NOTE]
>
>Wenn der Marketo-Synchronisierungsbenutzer Aufgaben erstellt **[!UICONTROL ist &quot;]**&quot; ein erforderliches Feld, damit die Aufgabe in [!DNL Microsoft] erstellt wird. Marketo gibt standardmäßig fünf Tage ein, wenn kein Wert eingegeben wird.

Passen Sie alle Felder an, um die Aufgabe wie gewünscht zu erstellen.

![](assets/create-task-in-microsoft-2.png)

>[!NOTE]
>
>Das Feld „Status“, das für die Aufgabe in der Flussaktion angegeben ist, aktualisiert das Feld „Statusgrund“ in [!DNL Microsoft].

>[!TIP]
>
>Sie können `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` und `{{system.tokens}}` in den **[!UICONTROL Betreff]** und **[!UICONTROL Beschreibung]**. Weitere [ finden Sie unter ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} für Flussschritte .
