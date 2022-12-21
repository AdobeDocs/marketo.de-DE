---
unique-page-id: 2953132
description: Smart-Kampagnen für Batch und Trigger - Marketo-Dokumente - Produktdokumentation
title: Smart-Kampagnen für Batch und Trigger
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Smart-Kampagnen für Batch und Trigger {#understanding-batch-and-trigger-smart-campaigns}

Es gibt zwei Arten von Smart-Kampagnen: Batch und Trigger.

## Smart-Batch-Kampagne {#batch-smart-campaign}

>[!NOTE]
>
>**Definition**
>
>Eine Batch-Kampagne wird zu einem bestimmten Zeitpunkt gestartet und betrifft eine bestimmte Gruppe von Personen auf einmal. Ein Beispiel wäre das Senden einer E-Mail an alle Menschen in Kalifornien.

Batch-Smart-Kampagnen verfügen nur über Filter im Bereich der intelligenten Liste (d. h. keine Trigger).

![](assets/batch-filter.png)

Klicken Sie auf die **Zeitplan** bestätigt, dass die Smart-Kampagne auf &quot;Batch&quot;eingestellt ist.

![](assets/batch-c4.png)

**Smart-Kampagnen stapeln**

* Kann für Wiederholungen, z. B. täglich, wöchentlich und monatlich, geplant werden. Sie können sie auch nur einmal ausführen lassen.
* sind auf der [Programmplanungsansicht](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md). Alles, was nach einem &quot;Warten&quot;-Schritt innerhalb der intelligenten Kampagne erfolgt, wird nicht in die Ansicht aufgenommen.

<br> 

## Smart Campaign für Trigger {#trigger-smart-campaign}

>[!NOTE]
>
>**Definition**
>
>Eine Trigger-Smart-Kampagne wirkt sich auf Basis eines ausgelösten Ereignisses immer nur auf eine Person aus. Ein Trigger könnte beispielsweise auf einen Link in einer E-Mail klicken.

Wenn eine Smart-Kampagne mindestens einen Trigger im Bereich &quot;Smart-Liste&quot;verwendet, wird der Modus automatisch auf &quot;Ausgelöst&quot;eingestellt.

![](assets/trigger.png)

Klicken Sie auf die **Zeitplan** bestätigt, dass die Smart-Kampagne auf &quot;Ausgelöst&quot;gesetzt ist.

![](assets/trigger2.png)

**Smart-Kampagnen für Trigger**

* Kann nicht für Wiederholungen geplant werden. Sie können nur auf &quot;aktiv&quot;oder &quot;inaktiv&quot;eingestellt werden.
* Sie können mehr als einen Trigger festlegen. Wenn jedoch ein Trigger ausgelöst wird, werden die Kampagnenaktionen ausgeführt.

>[!TIP]
>
>Verwenden Sie die [Aktivitätsprotokoll](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) , um zu sehen, was in Ihren Smart-Kampagnen Schritt für Schritt passiert ist. Das Aktivitätsprotokoll befindet sich im letzten Tab der Detailseite einer Person.
