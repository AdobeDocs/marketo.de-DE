---
unique-page-id: 2953132
description: Intelligente Batch- und Trigger-Kampagnen - Marketing-Dokumente - Produktdokumentation
title: Intelligente Kampagnen für Stapel und Trigger
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---


# Smart-Kampagnen für Stapel und Trigger {#understanding-batch-and-trigger-smart-campaigns}

Es gibt zwei Arten intelligenter Kampagnen: Stapel und Trigger.

## Stapel-Smart-Kampagne {#batch-smart-campaign}

>[!NOTE]
>
>**Definition**
>
>Eine Batch-Kampagne wird zu einem bestimmten Zeitpunkt gestartet und betrifft eine bestimmte Gruppe von Personen gleichzeitig. Ein Beispiel wäre das Senden einer E-Mail an alle Menschen in Kalifornien.

Batch-intelligente Kampagnen enthalten nur Filter im Abschnitt &quot;Intelligente Liste&quot;(d. h. keine Trigger).

![](assets/batch-filter.png)

Durch Klicken auf die Registerkarte **Plan** wird bestätigt, dass die intelligente Kampagne auf &quot;Stapel&quot;eingestellt ist.

![](assets/batch-c4.png)

**Stapelverarbeitung intelligenter Kampagnen**

* Kann für Wiederholungen, z. B. pro Tag, Woche und Monat, geplant werden. Sie können sie auch nur einmal ausführen lassen.
* Sind auf der Ansicht [Programmplanung](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md) sichtbar. Alles, was nach einem &quot;Wait&quot;-Schritt innerhalb der intelligenten Kampagne erfolgt, wird nicht in die Ansicht aufgenommen.

<br> 

## Trigger Smart-Kampagne {#trigger-smart-campaign}

>[!NOTE]
>
>**Definition**
>
>Eine intelligente Kampagne eines Triggers betrifft eine Person auf der Grundlage eines ausgelösten Ereignisses. Ein Beispiel für einen Trigger wäre das Klicken auf einen Link in einer E-Mail.

Wenn eine intelligente Kampagne mindestens einen Trigger im Bereich &quot;Intelligente Liste&quot;verwendet, wird der Modus automatisch auf Auslösen eingestellt.

![](assets/trigger.png)

Durch Klicken auf die Registerkarte **Plan** wird bestätigt, dass die intelligente Kampagne auf &quot;Ausgelöst&quot;eingestellt ist.

![](assets/trigger2.png)

**Intelligente Trigger-Kampagnen**

* Kann nicht für Wiederholungen geplant werden. Sie können nur als aktiv oder inaktiv eingestellt werden.
* Sie können mehr als einen Trigger festlegen. Wenn jedoch ein Trigger ausgelöst wird, werden die Kampagnen ausgeführt.

>[!TIP]
>
>Verwenden Sie das [Aktivität-Protokoll](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md), um zu sehen, was in Ihren intelligenten Kampagnen schrittweise passiert ist. Die Aktivität befindet sich auf der letzten Registerkarte der Detailseite.
