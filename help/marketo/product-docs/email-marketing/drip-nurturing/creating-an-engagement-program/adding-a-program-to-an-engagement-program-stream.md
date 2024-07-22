---
unique-page-id: 10098134
description: Hinzufügen eines Programms zu einem Interaktionsprogramm-Stream - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen eines Programms zu einem Interaktionsprogramm-Stream
exl-id: 44c2ce45-439b-4b29-8130-8cc218e04bbf
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Hinzufügen eines Programms zu einem Interaktionsprogramm-Stream {#adding-a-program-to-an-engagement-program-stream}

## Warum verwenden Sie ein verschachteltes Programm in einem Interaktionsprogramm-Stream? {#why-use-a-nested-program-in-an-engagement-program-stream}

Es ist einfach, in einem Interaktionsprogramm einem Stream eine E-Mail hinzuzufügen, und es funktioniert einwandfrei. Wenn Ihre geschäftlichen Anforderungen jedoch komplexer sind, kann es sinnvoll sein, die E-Mail in einem Programm zu platzieren. Sie können beispielsweise:

* E-Mail an eine Untergruppe von Personen im Stream senden
* Senden von *unterschiedlichen* E-Mails an Untergruppen innerhalb des Streams
* Einschließen von Landingpages, Formularen oder anderen Assets in die Baumstruktur
* Multitouch-Attribution aktivieren
* Zusätzliche Workflow-Schritte hinzufügen, z. B. Warnhinweis-E-Mails

## Was passiert, wenn Sie ein Programm in einem Stream verwenden? {#what-happens-when-you-use-a-program-in-a-stream}

Bei Verwendung eines verschachtelten Programms basiert die Entscheidung, eine E-Mail an eine Person zu senden, auf der Programmmitgliedschaft und der Programm-ID.

* Wenn Sie nicht Mitglied eines Programms sind, erhalten Sie alle E-Mails, die Teil des Programms sind, einmal
* Wenn Sie Mitglied des Programms sind, erhalten Sie die E-Mail nicht
* Wenn Sie kein Mitglied mehr sind, die E-Mail jedoch zuvor über dieses Programm erhalten haben, erhalten Sie die E-Mail nicht

Wenn Sie ein Programm in einem Stream verwenden, spielt es keine Rolle, ob Sie diese E-Mail bereits erhalten haben. Solange die E-Mail nicht vor *in diesem Programm* gesendet wurde, können Sie sie erneut erhalten.

In einem Interaktionsprogramm kann es schwierig werden, E-Mails und Programme zu mischen. Sie können die eine oder die andere verwenden.

>[!TIP]
>
>Stellen Sie sicher, dass Sie in Ihrer intelligenten Liste einen Filter vom Typ **Mitglied des Interaktionsprogramms** verwenden.

## Was passiert mit Leuten, die die Kriterien der intelligenten Liste nicht erfüllen? {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

Falls jemand aus der intelligenten Liste der Smart-Kampagne eines verschachtelten Programms herausgefiltert wird, wird während der aktuellen Wiedergabe nicht zum nächsten Inhaltselement übergegangen. Sie werden zum nächsten Inhaltselement im Stream für den *folgenden*-Guss übergehen.

## Was enthält ein verschachteltes Programm? {#what-does-a-nested-program-contain}

Ein gut konzipiertes verschachteltes Programm enthält E-Mails, Berichte und Smart-Kampagnen. Es macht Sinn, diese zusammenzuhalten.

Die von Ihnen verwendete E-Mail kann im Programm, in einem anderen Programm oder sogar in Design Studio live sein. Wo es lebt, hängt davon ab, wie man es verwenden will.

Berichtsänderungen mit E-Mail-Speicherort. Wenn sich die E-Mail beispielsweise in Design Studio befindet, werden im E-Mail-Leistungsbericht alle Metriken in einer Zeile angezeigt - die verschiedenen Änderungen werden kombiniert. Im Interaktions-Stream-Leistungsbericht werden die verschiedenen Sendungen jedoch separat angezeigt.

>[!CAUTION]
>
>Wenn Sie etwas erneut senden möchten, ist es am sichersten, ein neues Programm und eine intelligente Kampagne zu erstellen.

>[!MORELIKETHIS]
>
>* [Inhalt zu einem Stream hinzufügen](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [Grundlegendes zu Programmen](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
