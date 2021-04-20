---
title: understand-batch-and-Trigger-smart-Kampagnen
description: Intelligente Kampagnen für Stapel und Trigger
exl-id: 54f38ecc-1b4c-4944-9f42-d8c1190c99d0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Intelligente Kampagnen für Stapel und Trigger

<br> 

Es gibt zwei Arten intelligenter Kampagnen: Stapel und Trigger.

## Intelligente Kampagne stapeln

Eine Batch-Kampagne wird zu einem bestimmten Zeitpunkt gestartet und betrifft eine bestimmte Gruppe von Personen gleichzeitig. Ein Beispiel wäre das Senden einer E-Mail an alle in Ihrer Datenbank, die in Kalifornien leben.

Batch-intelligente Kampagnen enthalten nur Filter im Abschnitt &quot;Intelligente Liste&quot;(d. h. keine Trigger).

![Bild eins](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-1.png)

Durch Klicken auf die Registerkarte **[!UICONTROL Plan]** wird bestätigt, dass die intelligente Kampagne auf &quot;Stapel&quot;eingestellt ist.

![Bild zwei](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-2.png)

**Stapelverarbeitung intelligenter Kampagnen**

* Kann für Wiederholungen, z. B. pro Tag, Woche und Monat, geplant werden. Sie können sie auch nur einmal ausführen lassen.
* Sind auf der Ansicht [Programmplanung](https://docs.marketo.com/display/DOCS/Navigating+the+Program+Schedule+View) sichtbar.
* Alles, was nach einem &quot;Wait&quot;-Schritt innerhalb der intelligenten Kampagne erfolgt, wird nicht in die Ansicht aufgenommen.

## Intelligente Trigger-Kampagne

Eine intelligente Kampagne eines Triggers betrifft eine Person auf der Grundlage eines ausgelösten Ereignisses. Ein Beispiel für einen Trigger wäre das Klicken auf einen Link in einer E-Mail.

Wenn eine intelligente Kampagne mindestens einen Trigger im Bereich &quot;Intelligente Liste&quot;verwendet, wird der Modus automatisch auf Auslösen eingestellt.

![Bild drei](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-3.png)

Durch Klicken auf die Registerkarte **[!UICONTROL Plan]** wird bestätigt, dass die intelligente Kampagne auf &quot;Trigger&quot;eingestellt ist.

![Bild vier](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-4.png)

**Intelligente Trigger-Kampagnen**

* Kann nicht für Wiederholungen geplant werden. Sie können nur als aktiv oder inaktiv eingestellt werden.
* Sie können mehr als einen Trigger festlegen. Wenn jedoch ein _beliebiger_-Trigger ausgelöst wird, werden die Kampagnen ausgeführt.

>[!TIP]
>
>Verwenden Sie das [Aktivität-Protokoll](https://docs.marketo.com/display/DOCS/Locate+the+Activity+Log+for+a+Person), um zu sehen, was in Ihren intelligenten Kampagnen schrittweise passiert ist. Die Aktivität befindet sich auf der letzten Registerkarte der Detailseite.
