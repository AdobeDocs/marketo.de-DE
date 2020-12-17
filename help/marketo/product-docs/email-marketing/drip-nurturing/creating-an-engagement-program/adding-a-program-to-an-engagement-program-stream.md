---
unique-page-id: 10098134
description: Hinzufügen eines Programms zu einem Interaktions-Programm-Stream - Marketing Docs - Produktdokumentation
title: Hinzufügen eines Programms zu einem Interaktions-Programm-Stream
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


# Hinzufügen eines Programms zu einem Interaktions-Programm-Stream {#adding-a-program-to-an-engagement-program-stream}

## Warum ein verschachteltes Programm in einem Interaktions-Programm-Stream verwenden? {#why-use-a-nested-program-in-an-engagement-program-stream}

Es ist einfach, eine E-Mail zu einem Stream in einem Interaktions-Programm hinzuzufügen, und es funktioniert einwandfrei. Wenn Ihre geschäftlichen Anforderungen jedoch komplexer sind, kann es sinnvoll sein, die E-Mail in einem Programm zu platzieren. Sie möchten beispielsweise:

* Senden einer E-Mail an eine Untergruppe von Personen im Stream
* *verschiedene* E-Mails an Untergruppen im Stream senden
* Landingpages, Formulare oder andere Assets in die Struktur einschließen
* Multitouch-Zuordnung aktivieren
* hinzufügen Schritte für zusätzlichen Textfluss, wie z. B. Warn-E-Mails

## Was passiert, wenn Sie ein Programm in einem Stream verwenden? {#what-happens-when-you-use-a-program-in-a-stream}

Bei der Verwendung eines verschachtelten Programms hängt die Entscheidung, eine E-Mail an eine Person zu senden, von der Programm-Mitgliedschaft und der Programm-ID ab.

* Wenn Sie kein Mitglied eines Programms sind, erhalten Sie einmal alle E-Mails, die Teil des Programms sind
* Wenn Sie Mitglied des Programms sind, erhalten Sie die E-Mail nicht
* Wenn Sie kein Mitglied mehr sind, die E-Mail jedoch früher über dieses Programm erhalten haben, erhalten Sie die E-Mail nicht

Wenn Sie ein Programm in einem Stream verwenden, spielt es keine Rolle, ob Sie diese bestimmte E-Mail bereits erhalten haben. Solange die E-Mail nicht vor *in diesem Programm* gesendet wurde, können Sie sie erneut empfangen.

Es kann schwierig werden, E-Mails und Programms in einem Interaktions-Programm zu mischen. Sie sollten das eine oder das andere verwenden.

>[!TIP]
>
>Stellen Sie sicher, dass Sie in Ihrer intelligenten Liste einen **Programm des Interaktionsmitglieds** verwenden.

## Was passiert mit Leuten, die die Kriterien der intelligenten Liste nicht erfüllen? {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

In dem Ereignis, dass jemand aus der intelligenten Liste der intelligenten Kampagne eines verschachtelten Programms herausgefiltert wird, wird während der aktuellen Wiedergabe nicht zum nächsten Inhaltselement gewechselt. Sie wechseln zum nächsten Inhaltselement im Stream für den *folgenden*-Guss.

## Was enthält ein verschachteltes Programm? {#what-does-a-nested-program-contain}

Ein gut gestaltetes verschachteltes Programm enthält E-Mails, Berichte und intelligente Kampagnen. Es macht Sinn, diese zusammenzuhalten.

Die von Ihnen verwendete E-Mail kann im Programm, in einem anderen Programm oder sogar im Design Studio live geschaltet werden. Wo es lebt, hängt davon ab, wie man es benutzen will.

Der Berichte ändert sich mit dem E-Mail-Speicherort. Wenn sich die E-Mail beispielsweise im Design Studio befindet, werden im Bericht &quot;E-Mail-Leistung&quot;alle Metriken in einer Zeile angezeigt - die verschiedenen Abschnitte werden kombiniert. Im Bericht &quot;Leistung des Interaktionsstreams&quot;werden die verschiedenen Sends jedoch separat angezeigt.

>[!CAUTION]
>
>Wenn Sie etwas erneut senden möchten, ist es am sichersten, ein neues Programm und eine intelligente Kampagne zu erstellen.

>[!MORELIKETHIS]
>
>* [hinzufügen von Inhalten in einem Stream](add-content-to-a-stream.md)
>* [Programme verstehen](../../../../product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)

>



