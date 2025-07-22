---
unique-page-id: 10098134
description: Hinzufügen eines Programms zu einem Interaktionsprogramm-Stream - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen eines Programms zu einem Interaktionsprogramm-Stream
exl-id: 44c2ce45-439b-4b29-8130-8cc218e04bbf
feature: Engagement Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Hinzufügen eines Programms zu einem Interaktionsprogramm-Stream {#adding-a-program-to-an-engagement-program-stream}

## Warum sollte ein verschachteltes Programm in einem Interaktionsprogramm-Stream verwendet werden? {#why-use-a-nested-program-in-an-engagement-program-stream}

Es ist einfach, eine E-Mail zu einem Stream in einem Interaktionsprogramm hinzuzufügen, und es funktioniert einwandfrei. Wenn Ihre geschäftlichen Anforderungen jedoch komplexer sind, kann es sinnvoll sein, die E-Mail in einem Programm zu platzieren. Sie können beispielsweise Folgendes tun:

* Senden einer E-Mail an eine Untergruppe von Personen im Stream
* Senden *unterschiedlicher* E-Mails an Untergruppen im Stream
* Einbinden von Landingpages, Formularen oder anderen Assets in die Pflege
* Multi-Touch-Attribution aktivieren
* Hinzufügen zusätzlicher Flussschritte, z. B. Benachrichtigungs-E-Mails

## Was passiert, wenn ein Programm in einem Stream verwendet wird? {#what-happens-when-you-use-a-program-in-a-stream}

Bei Verwendung eines verschachtelten Programms basiert die Entscheidung, eine E-Mail an eine Person zu senden, auf der Programmmitgliedschaft und der Programm-ID.

* Wenn Sie kein Programmteilnehmer sind, erhalten Sie alle E-Mails, die Teil des Programms sind, einmal
* Wenn Sie Mitglied des Programms sind, erhalten Sie die E-Mail nicht
* Wenn Sie kein Mitglied mehr sind, aber die E-Mail früher über dieses Programm erhalten haben, erhalten Sie die E-Mail nicht mehr

Wenn Sie ein Programm in einem Stream verwenden, spielt es keine Rolle, ob Sie diese spezifische E-Mail bereits erhalten haben. Solange die E-Mail nicht vor (in *bestimmten Programm) gesendet wurde* können Sie sie erneut erhalten.

Es kann schwierig sein, E-Mails und Programme in einem Interaktionsprogramm zu mischen. Vielleicht möchten Sie das eine oder das andere verwenden.

>[!TIP]
>
>Denken Sie daran, in Ihrer Smart-Liste einen Filter **[!UICONTROL Programm]** Mitglied der Interaktion“ zu verwenden.

## Was passiert mit Leuten, die die Kriterien der Smart List nicht erfüllen? {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

Für den Fall, dass jemand aus der Smart-Liste der Smart-Kampagne eines verschachtelten Programms herausgefiltert wird, geht er während der aktuellen Besetzung nicht zum nächsten Inhaltselement über. Sie gehen zum nächsten Inhaltselement im Stream für die *folgende* Besetzung über.

## Was enthält ein verschachteltes Programm? {#what-does-a-nested-program-contain}

Ein gut konzipiertes verschachteltes Programm enthält E-Mails, Berichte und intelligente Kampagnen. Es ist sinnvoll, diese zusammenzuhalten.

Die E-Mail, die Sie verwenden, kann im Programm, in einem anderen Programm oder sogar im [!UICONTROL Design Studio] live sein. Wo er lebt, hängt davon ab, wie man ihn nutzen möchte.

Änderungen mit E-Mail-Speicherort melden. Wenn sich die E-Mail beispielsweise im [!UICONTROL Design Studio] befindet, werden im E-Mail-Leistungsbericht alle Metriken in einer Zeile angezeigt - die verschiedenen Darstellungen werden kombiniert. Im Bericht zur Interaktions-Stream-Leistung werden die verschiedenen Sendungen jedoch separat angezeigt.

>[!CAUTION]
>
>Wenn Sie etwas erneut senden möchten, ist es am sichersten, ein neues Programm und eine intelligente Kampagne zu erstellen.

>[!MORELIKETHIS]
>
>* [Inhalt zu einem Stream hinzufügen](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [Grundlegendes zu Programmen](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
