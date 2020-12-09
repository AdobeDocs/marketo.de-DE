---
unique-page-id: 10096681
description: Erläuterungen zu Webinar-Programm-Statusangaben - Marketing-Dokumente - Produktdokumentation
title: Erläuterungen zu Webinar-Programm-Status
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---


# Erläuterungen zu Webinar-Programm-Status {#understanding-webinar-program-statuses}

Der Status eines Programms stellt die verschiedenen Ereignisses dar, die eine Person als Mitglied des Ereignisses durchläuft. Sie sind mit einem Kanal verknüpft. Marketo verfügt über einen integrierten Kanal namens **Webinar**. Status können sowohl in Batch- als auch in Trigger-Kampagnen verwendet werden.

Die Menschen durchlaufen die Statusangaben des Programms linear und gehen nicht zurück. Beispielsweise kann eine Person mit dem Status &quot; **Teilnehmer** &quot;nicht zu &quot; **Registriert**&quot;zurückkehren.

Im Folgenden werden die mit dem Webinar-Kanal verbundenen Programm-Status kurz beschrieben.

>[!TIP]
>
>Um den Status manuell zu aktualisieren, klicken Sie in der Dropdown-Liste &quot; **Ereignis-Aktionen** &quot;auf &quot;Von Webinar-Provider **** aktualisieren&quot;.

![](assets/image2015-12-17-13-3a52-3a39.png)

**Nicht im Programm** - Verwenden Sie diesen Status, um Personen aus dem Ereignis zu entfernen.

** Eingeladen** - Verwenden Sie diesen Status, um dem Ereignis Personen hinzuzufügen.

**Ausstehende Genehmigung** - Verwenden Sie diesen Status, um die Versendung einer Bestätigungs-E-Mail an Ihre Personen zu unterbrechen. Weitere Informationen finden Sie unter &quot;Manuelles Genehmigen von Registranten&quot;in [ON24 Ereignis Registrierungsupdates](on24-event-registration-updates.md) .

**Warteliste** - Verwenden Sie diesen Status, um einige Personen so lange warten zu lassen, bis weitere Plätze verfügbar sind.

**Abgelehnt** - Verwenden Sie diesen Status, um die Registrierung einer Person für Ihr Ereignis abzulehnen.

**Registriert** - Dieser Status zwingt die Benutzer zu ON24, wenn Sie die ON24-Integration verwenden. Der Status der Person wird aktualisiert, wenn ON24 darauf antwortet, dass die Person erfolgreich registriert wurde.

**Registrierungsfehler** : Dieser Status gibt an, dass beim Versuch, sich für das Ereignis zu registrieren, ein Fehler aufgetreten ist.

>[!NOTE]
>
>Wenn ein Registrierungsfehler auftritt, können Sie weitere Informationen zu dieser Person abrufen, indem Sie die Spalte &quot;Statusgrund&quot;auf der Registerkarte &quot;Mitglieder&quot;Ihres Programms aufrufen. Nachdem der Fehler behoben wurde, können Sie den Status des Programms des Benutzers manuell in &quot;Registered in Marketo&quot;ändern.

**Teilnehmer**: Am Ende des Webinars gibt ON24 eine Liste der Teilnehmenden zurück. Dieser Status wird automatisch nach Marketo gezogen.

**Angezeigt On-Demand** - Personen, die an der archivierten Version des Webinars teilgenommen haben, erhalten diesen Status.

**No Show** - Nach Abschluss des Webinars und nach Eingabe der Anwesenheitsdaten von ON24 wird der Status der Personen, die sich registriert, aber nicht teilgenommen haben, auf No Show aktualisiert. Es kann zwischen 30 Minuten und 3 Stunden dauern, bis ON24 die letzten Anwesenheitsinformationen vorbereitet und in Marketo verfügbar macht.

>[!NOTE]
>
>Damit Marketo den Status &quot;Keine Anzeige&quot;abrufen kann, müssen die Personen *in Marketo* registriert sein. Wir können keine No Shows erfassen, die aus dem On24-Datenfeed stammen.

>[!MORELIKETHIS]
>
>* [Ereignisse des Marketo ON24-Adapters](understanding-marketo-on24-adapter-events.md)

>



