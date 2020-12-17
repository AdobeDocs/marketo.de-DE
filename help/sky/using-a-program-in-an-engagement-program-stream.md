---
title: using-a-Programm-in-an-engagement-Programm-stream
description: Verwenden eines Programms in einem Interaktions-Programm-Stream
translation-type: tm+mt
source-git-commit: 73df78512226c6c57625a73f14ba8b00bea195bd
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---


# Verwenden eines Programms in einem Interaktions-Programm-Stream

## Warum ein verschachteltes Programm in einem Interaktions-Programm-Stream verwenden?

Es ist einfach, eine E-Mail zu einem Stream in einem Interaktions-Programm hinzuzufügen, und es funktioniert einwandfrei. Wenn Ihre geschäftlichen Anforderungen jedoch komplexer sind, kann es sinnvoll sein, die E-Mail in einem Programm zu platzieren. Sie möchten beispielsweise:

* Senden einer E-Mail an eine Untergruppe von Personen im Stream
* _verschiedene_ E-Mails an Untergruppen im Stream senden
* Landingpages, Formulare oder andere Assets in das Interaktions-Programm aufnehmen
* Multitouch-Zuordnung aktivieren
* hinzufügen Schritte mit zusätzlichen Textflüssen, wie z. B. Warnmeldungen

## Was passiert, wenn Sie ein Programm in einem Stream verwenden?

Bei der Verwendung eines verschachtelten Programms hängt die Entscheidung, eine E-Mail an eine Person zu senden, von der Programm-Mitgliedschaft und der Programm-ID ab.

* Wenn Sie nicht Mitglied des Programms sind, erhalten Sie einmal alle E-Mails, die zum Programm gehören
* Wenn Sie Mitglied des Programms sind, erhalten Sie die E-Mail nicht
* Wenn Sie kein Mitglied mehr sind, aber die E-Mail bereits früher über dieses Programm erhalten haben, erhalten Sie die E-Mail nicht

Wenn Sie ein Programm in einem Stream verwenden, spielt es keine Rolle, ob Sie diese bestimmte E-Mail bereits erhalten haben. Solange die E-Mail nicht vor _in diesem Programm_ gesendet wurde, können Sie sie erneut empfangen.

Es kann schwierig werden, E-Mails und Programms in einem Interaktions-Programm zu mischen. Sie sollten das eine oder das andere verwenden.

>[!TIP]
>
>Achten Sie darauf, in Ihrer intelligenten Liste einen Programm-Filter für Interaktionsmitglieder zu verwenden.

## Was passiert mit Leuten, die die Kriterien der intelligenten Liste nicht erfüllen?

In dem Ereignis, dass jemand aus der intelligenten Liste der intelligenten Kampagne eines verschachtelten Programms herausgefiltert wird, wird während der aktuellen Wiedergabe nicht zum nächsten Inhaltselement gewechselt. Sie wechseln zum nächsten Inhaltselement im Stream für den _folgenden_-Guss.

## Was enthält ein verschachteltes Programm?

Ein gut gestaltetes verschachteltes Programm enthält E-Mails, Berichte und intelligente Kampagnen. Es macht Sinn, diese zusammenzuhalten.

Die von Ihnen verwendete E-Mail kann im Programm, in einem anderen Programm oder sogar im Design Studio live geschaltet werden. Wo es lebt, hängt davon ab, wie man es benutzen will.

Der Berichte ändert sich mit dem E-Mail-Speicherort. Wenn sich die E-Mail beispielsweise im Design Studio befindet, werden im Bericht &quot;E-Mail-Leistung&quot;alle Metriken in einer Zeile angezeigt - die verschiedenen Abschnitte werden kombiniert. Im Bericht &quot;Leistung des Interaktionsstreams&quot;werden die verschiedenen Sends jedoch separat angezeigt.

>[!CAUTION]
>
>Wenn Sie etwas erneut senden möchten, ist es am sichersten, ein neues Programm und eine intelligente Kampagne zu erstellen.
