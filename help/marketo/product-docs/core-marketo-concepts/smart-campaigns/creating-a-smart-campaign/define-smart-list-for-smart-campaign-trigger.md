---
unique-page-id: 1146942
description: Definieren einer Smart-Liste für eine intelligente Kampagne | Trigger - Marketo Docs - Produktdokumentation
title: Definieren einer Smart-Liste für eine intelligente Kampagne | Trigger
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
source-git-commit: a15a4b9bccb069b51186aac7b913008d15aa645e
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# Definieren einer Smart-Liste für eine intelligente Kampagne | Trigger {#define-smart-list-for-smart-campaign-trigger}

Erstellen Sie eine intelligente Kampagne auf der Basis von Live-Ereignissen, indem Sie Trigger hinzufügen.

1. Klicken Sie in Ihrer Smart-Kampagne auf die **Smart List** Registerkarte.

   ![](assets/image2014-9-19-16-3a22-3a55.png)

1. Suchen Sie nach dem Trigger und ziehen Sie den Trigger per Drag-and-Drop auf die Arbeitsfläche.

   ![](assets/image2014-9-19-16-3a23-3a24.png)

   >[!NOTE]
   >
   >Eine intelligente Kampagne mit Triggern wird in **Trigger** -Modus. Er wird basierend auf ausgelösten Ereignissen und beliebigen zusätzlichen Filtern jeweils für eine Person ausgeführt.

   >[!IMPORTANT]
   >
   >Wenn Sie ein boolesches Feld in einer Trigger-Kampagnen-Smart-Liste verwenden, müssen Sie es explizit auf &quot;false&quot;setzen, damit das Feld während der Ausführung der Kampagne korrekt ausgewertet wird.

1. Klicken Sie auf die Dropdown-Liste und wählen Sie einen Operator aus.

   ![](assets/image2014-9-19-16-3a23-3a29.png)

   >[!CAUTION]
   >
   >Rote eckige Linien zeigen Fehler oder fehlende Informationen an. Wenn die Kampagne nicht korrigiert wird, ist sie ungültig und wird nicht ausgeführt.

   >[!TIP]
   >
   >In einer Smart-Kampagne mit Triggern und Filtern werden die Trigger ganz oben aufgeführt und bei der Auslösung durchlaufen nur Personen, die die Filterkriterien erfüllen.

1. Definieren Sie den Trigger.

   ![](assets/image2014-9-19-16-3a24-3a36.png)

   >[!NOTE]
   >
   >Bei mehreren Triggern durchläuft eine Person den Fluss, wenn **ANDERE** einer der Trigger aktiviert wird.

Um die Kampagne für eine Reihe von Personen gleichzeitig auszuführen, erfahren Sie, wie Sie [Definieren einer Smart-Liste für eine intelligente Kampagne | Charge](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md).

>[!MORELIKETHIS]
>
>[Hinzufügen eines Flussschritts zu einer Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
