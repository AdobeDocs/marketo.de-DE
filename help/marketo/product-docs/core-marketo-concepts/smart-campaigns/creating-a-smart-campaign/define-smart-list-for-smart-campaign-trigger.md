---
unique-page-id: 1146942
description: Definieren einer Smart-Liste für eine intelligente Kampagne | Trigger - Marketo Docs - Produktdokumentation
title: Definieren einer Smart-Liste für eine intelligente Kampagne | Trigger
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
feature: Smart Campaigns
source-git-commit: c3aa1a29b084cb1c1add9d22cdbfc23bdcf7512b
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Definieren einer Smart-Liste für eine intelligente Kampagne | Trigger {#define-smart-list-for-smart-campaign-trigger}

Erstellen Sie basierend auf Live-Ereignissen eine Smart-Kampagne für eine Person, indem Sie Trigger hinzufügen.

>[!CAUTION]
>
>Die Bearbeitung von Smart-Listen- oder Flussschritt-Bearbeitungen an einer aktiven Kampagne kann möglicherweise deren Funktionalität beeinträchtigen. Gehen Sie dabei mit Vorsicht vor.

1. Klicken Sie in Ihrer Smart-Kampagne auf die **[!UICONTROL Smart List]** Registerkarte.

   ![](assets/define-smart-list-for-smart-campaign-trigger-1.png)

1. Suchen Sie nach dem gewünschten Trigger und ziehen Sie ihn per Drag-and-Drop auf die Arbeitsfläche.

   ![](assets/define-smart-list-for-smart-campaign-trigger-2.png)

   >[!NOTE]
   >
   >Eine Smart-Kampagne mit Triggern wird in _Trigger_ -Modus. Er wird basierend auf ausgelösten Ereignissen und beliebigen zusätzlichen Filtern jeweils für eine Person ausgeführt.

   >[!IMPORTANT]
   >
   >Bei Verwendung eines booleschen Felds in einer Smart-List einer Trigger-Kampagne müssen Sie es explizit auf &quot;false&quot;setzen, damit das Feld während der Ausführung der Kampagne korrekt ausgewertet wird.

1. Klicken Sie auf die Dropdown-Liste und wählen Sie einen Operator aus.

   ![](assets/define-smart-list-for-smart-campaign-trigger-3.png)

   >[!CAUTION]
   >
   >Rote eckige Linien zeigen Fehler oder fehlende Informationen an. Wenn die Kampagne nicht korrigiert wird, ist sie ungültig und wird nicht ausgeführt.

   >[!TIP]
   >
   >In einer Smart-Kampagne mit Triggern und Filtern werden die Trigger ganz oben angezeigt und bei der Auslösung durchlaufen nur Personen, die die Filterkriterien erfüllen.

1. Definieren Sie den Trigger.

   ![](assets/define-smart-list-for-smart-campaign-trigger-4.png)

   >[!NOTE]
   >
   >Bei mehreren Triggern durchläuft eine Person den Fluss, wenn _ANDERE_ einer der Trigger aktiviert wird.

Um die Kampagne für eine Reihe von Personen gleichzeitig auszuführen, erfahren Sie, wie Sie [Definieren einer Smart-Liste für eine intelligente Kampagne | Batch](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}.

>[!MORELIKETHIS]
>
>[Hinzufügen eines Flussschritts zu einer Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
