---
unique-page-id: 37356429
description: Erfahren Sie, wie Sie in Microsoft Dynamics eine Aufgabe aus einem Flussschritt erstellen. Erstellen Sie eine Aufgabe für den Eigentümer, wenn jemand in den Fluss eintritt.
title: Erstellen einer Aufgabe in Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
TQID: https://experienceleague.adobe.com/qQL3O4Vi8ncdlXtk2gvraWzquz3oZx5B-1YWTkwdVac
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 184
ht-degree: 4%

---

# Erstellen einer Aufgabe in Microsoft {#create-task-in-microsoft}

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
>Sie können `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` und `{{system.tokens}}` in den **[!UICONTROL Betreff]** und **[!UICONTROL Beschreibung]**. Weitere [&#x200B; finden Sie unter &#x200B;](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} für Flussschritte .
