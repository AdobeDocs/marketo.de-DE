---
unique-page-id: 2953132
description: Grundlegendes zu Smart Campaign im Batch- und Trigger - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zu Smart Campaign für Batch und Trigger
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
feature: Smart Campaigns
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 1%

---

# Grundlegendes zu Smart Campaign für Batch und Trigger {#understanding-batch-and-trigger-smart-campaigns}

Es gibt zwei Arten von Smart-Kampagnen: Batch und Trigger.

## Stapel-Kampagne {#batch-campaign}

>[!NOTE]
>
>**Definition**
>
>Eine Batch-Kampagne wird zu einem bestimmten Zeitpunkt gestartet und wirkt sich auf eine bestimmte Gruppe von Personen gleichzeitig aus. Ein Beispiel wäre das Senden einer E-Mail an alle Menschen in Kalifornien.

Batch-Kampagnen verfügen nur über Filter innerhalb des Abschnitts Smart-Liste (d. h. keine Trigger).

![](assets/understanding-batch-and-trigger-smart-campaigns-1.png)

Durch Klicken auf **[!UICONTROL Zeitplan]** wird bestätigt, dass die Smart-Kampagne auf „Batch“ eingestellt ist.

![](assets/understanding-batch-and-trigger-smart-campaigns-2.png)

**Batch-Smart-Kampagnen**

* Kann für Wiederholungen geplant werden, z. B. täglich, wöchentlich und monatlich. Sie können sie auch nur einmal ausführen lassen.
* Sind in der Ansicht [Programmzeitplan“ ](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md){target="_blank"}. Alles nach einem „Warten“-Schritt in der Smart-Kampagne wird nicht in die Ansicht aufgenommen.

<br> 

## Auslöser-Kampagne {#trigger-campaign}

>[!NOTE]
>
>**Definition**
>
>Eine Trigger-Kampagne wirkt sich auf der Grundlage eines ausgelösten Ereignisses jeweils auf eine Person aus. Ein Beispiel für einen Trigger wäre das Klicken auf einen Link in einer E-Mail.

Wenn eine Smart-Kampagne mindestens einen Trigger im Abschnitt Smart-Liste verwendet, wird der Modus automatisch auf Ausgelöst gesetzt.

![](assets/understanding-batch-and-trigger-smart-campaigns-3.png)

Durch Klicken auf die **[!UICONTROL Zeitplan]**-Registerkarte wird bestätigt, dass die Smart-Kampagne auf „Ausgelöst“ eingestellt ist.

![](assets/understanding-batch-and-trigger-smart-campaigns-4.png)

**Trigger-Kampagnen**

* Kann nicht für Wiederholungen geplant werden. Sie können nur auf „aktiv“ oder „inaktiv“ gesetzt werden.
* Sie können mehr als einen Trigger festlegen. Wenn jedoch ein Trigger ausgelöst wird, werden die Kampagnenaktionen ausgeführt.

>[!TIP]
>
>Im [Aktivitätsprotokoll](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md){target="_blank"} können Sie Schritt für Schritt sehen, was in Ihren Smart-Kampagnen passiert ist. Das Aktivitätsprotokoll finden Sie auf der letzten Registerkarte der Detailseite einer Person.
