---
unique-page-id: 2953132
description: Smart-Kampagnen für Batch und Trigger - Marketo-Dokumente - Produktdokumentation
title: Smart-Kampagnen für Batch und Trigger
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
feature: Smart Campaigns
source-git-commit: 75aa1f6c5f7d0c193787978a18900441aa9a8b82
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 3%

---

# Smart-Kampagnen für Batch und Trigger {#understanding-batch-and-trigger-smart-campaigns}

Es gibt zwei Arten von Smart-Kampagnen: Batch und Trigger.

## Stapel-Kampagne {#batch-campaign}

>[!NOTE]
>
>**Definition**
>
>Eine Batch-Kampagne wird zu einem bestimmten Zeitpunkt gestartet und betrifft eine bestimmte Gruppe von Personen auf einmal. Ein Beispiel wäre das Senden einer E-Mail an alle Menschen in Kalifornien.

Batch-Kampagnen enthalten nur Filter im Bereich der intelligenten Liste (d. h. keine Trigger).

![](assets/understanding-batch-and-trigger-smart-campaigns-1.png)

Klicken Sie auf **Zeitplan** bestätigt, dass die Smart-Kampagne auf &quot;Batch&quot;eingestellt ist.

![](assets/understanding-batch-and-trigger-smart-campaigns-2.png)

**Smart-Kampagnen stapeln**

* Kann für Wiederholungen, z. B. täglich, wöchentlich und monatlich, geplant werden. Sie können sie auch nur einmal ausführen lassen.
* sind auf der [Programmplanungsansicht](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md). Alles, was nach einem &quot;Warten&quot;-Schritt innerhalb der Smart-Kampagne erfolgt, wird nicht in die Ansicht aufgenommen.

<br> 

## Auslöser-Kampagne {#trigger-campaign}

>[!NOTE]
>
>**Definition**
>
>Eine Trigger-Kampagne betrifft eine Person auf der Grundlage eines ausgelösten Ereignisses. Ein Trigger könnte beispielsweise auf einen Link in einer E-Mail klicken.

Wenn eine Smart-Kampagne mindestens einen Trigger im Bereich Smart-Liste verwendet, wird der Modus automatisch auf &quot;Ausgelöst&quot;eingestellt.

![](assets/understanding-batch-and-trigger-smart-campaigns-3.png)

Klicken Sie auf **Zeitplan** bestätigt, dass die Smart-Kampagne auf &quot;ausgelöst&quot;gesetzt ist.

![](assets/understanding-batch-and-trigger-smart-campaigns-4.png)

**Auslöserkampagnen**

* Kann nicht für Wiederholungen geplant werden. Sie können nur auf &quot;aktiv&quot;oder &quot;inaktiv&quot;eingestellt werden.
* Sie können mehr als einen Trigger festlegen. Wenn jedoch ein Trigger ausgelöst wird, werden die Kampagnenaktionen ausgeführt.

>[!TIP]
>
>Verwenden Sie die [Aktivitätsprotokoll](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) , um zu sehen, was in Ihren Smart-Kampagnen Schritt für Schritt passiert ist. Das Aktivitätsprotokoll befindet sich im letzten Tab der Detailseite einer Person.
