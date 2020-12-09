---
title: understand-batch-and-trigger-smart-Kampagnen
description: Intelligente Batch- und Trigger-Kampagnen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Intelligente Batch- und Trigger-Kampagnen

<br> 

Es gibt zwei Arten intelligenter Kampagnen: Stapel und Auslöser.

## Intelligente Kampagne stapeln

Eine Batch-Kampagne wird zu einem bestimmten Zeitpunkt gestartet und betrifft eine bestimmte Gruppe von Personen gleichzeitig. Ein Beispiel wäre das Senden einer E-Mail an alle in Ihrer Datenbank, die in Kalifornien leben.

Batch-intelligente Kampagnen enthalten nur Filter im Abschnitt &quot;Intelligente Liste&quot;(d. h. keine Auslöser).

![Bild eins](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-1.png)

Durch Klicken auf die Registerkarte &quot; **[!UICONTROL Plan]** &quot;wird bestätigt, dass die intelligente Kampagne auf &quot;Stapel&quot;eingestellt ist.

![Bild zwei](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-2.png)

**Stapelverarbeitung intelligenter Kampagnen**

* Kann für Wiederholungen, z. B. pro Tag, Woche und Monat, geplant werden. Sie können sie auch nur einmal ausführen lassen.
* sind auf der [Programmplanung Ansicht](https://docs.marketo.com/display/DOCS/Navigating+the+Program+Schedule+View)sichtbar.
* Alles, was nach einem &quot;Wait&quot;-Schritt innerhalb der intelligenten Kampagne erfolgt, wird nicht in die Ansicht aufgenommen.

## Auslösen der intelligenten Kampagne

Eine intelligente Auslöser-Kampagne wirkt sich je nach ausgelöstem Ereignis auf eine Person aus. Ein Beispiel für einen Auslöser wäre das Klicken auf einen Link in einer E-Mail.

Wenn eine intelligente Kampagne im Abschnitt &quot;Intelligente Liste&quot;mindestens einen Auslöser verwendet, wird der Modus automatisch auf Auslösen eingestellt.

![Bild drei](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-3.png)

Durch Klicken auf die Registerkarte **[!UICONTROL Plan]** wird bestätigt, dass die intelligente Kampagne auf &quot;Auslöser&quot;eingestellt ist.

![Bild vier](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-4.png)

**Auslösen intelligenter Kampagnen**

* Kann nicht für Wiederholungen geplant werden. Sie können nur als aktiv oder inaktiv eingestellt werden.
* Sie können mehrere Auslöser einstellen. Wenn jedoch _ein_ Auslöser ausgelöst wird, werden die Kampagnen ausgeführt.

>[!TIP]
>
>Verwenden Sie das [Aktivitäten-Protokoll](https://docs.marketo.com/display/DOCS/Locate+the+Activity+Log+for+a+Person) , um Schritt für Schritt in Ihren intelligenten Kampagnen zu sehen. Die Aktivität befindet sich auf der letzten Registerkarte der Detailseite.
