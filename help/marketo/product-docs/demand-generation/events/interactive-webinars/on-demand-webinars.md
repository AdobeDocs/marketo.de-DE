---
description: On-Demand-Webinare - Marketo-Dokumente - Produktdokumentation
title: On-Demand-Webinare
hide: true
hidefromtoc: true
feature: Interactive Webinars
source-git-commit: 49a75b6aef25787a68554dff3a847279ef8ba12a
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# On-Demand-Webinare {#on-demand-webinars}

On-Demand-Webinare erfassen und verfeinern die Leads, die sich für Ihre Veranstaltung registriert haben und nicht teilgenommen haben, aber Informationen zu der Veranstaltung erhalten möchten, indem sie die Aufzeichnung ansehen. Informationen wie Name, E-Mail-ID und Datum/Dauer der Wiedergabe können in Marketo Engage erfasst und für das Targeting dieser Leads ohne Anzeige verwendet werden.

Die Webinar-Verbindungs-URL, die vor dem Ereignis für die Registrierungspflichtigen freigegeben wurde, kann als Link zur Wiedergabe der On-Demand-Aufzeichnung verwendet werden. Sobald ein Registrant, der nicht an der Live-Veranstaltung teilgenommen hat, d. h. ein Lead mit dem Programmstatus &quot;Keine Sendung&quot;, auf die Webinar-Join-URL klickt, ändert sich der Programmstatus eines solchen Leads von &quot;Keine Sendung&quot; in &quot;Teilnehmer On-Demand&quot;. Beachten Sie, dass der Programmstatus der Leads, die das Ereignis live angesehen haben und den Status &quot;Teilnehmer&quot;haben, nicht beeinträchtigt würde, selbst wenn sie die Join-URL besuchen und sich die On-Demand-Aufzeichnung ansehen würden.

Adobe Connect, die Technologie für interaktive Webinare, verfolgt den Besuch sowie die Überwachungsdauer der Leads, die die Aufzeichnung gesehen haben, und meldet diese täglich an Marketo. Die Aufzeichnung ist für einen Zeitraum von 30 Tagen nach dem Ereignis unter der Verbindungs-URL verfügbar und die Dauer ist festgelegt.

Marketo stellt mithilfe der beiden folgenden Widgets die Überwachungsstatistiken für On-Demand-Webinare auf der Registerkarte &quot;Dashboard&quot;bereit:
1. On-Demand-Zusammenfassung: Diese Übersicht zeigt die Anzahl der Besucher (keine Aufnahmen), die den aufgezeichneten Beitrag zum Ereignis gesehen haben.
2. On-Demand-Statistiken: Diese Widgets bieten Informationen zu: a. Tagen, an denen die On-Demand-Aufzeichnung zur Anzeige verfügbar ist. Dies kann Marketingexperten dabei helfen, Aktionen wie das Ausführen von E-Mail-Kampagnen näher am Ende der Verfügbarkeitsdauer der Aufzeichnung von 30 Tagen durchzuführen.
b. Gesamtbesucherzahl für On-Demand-Webinare bis zum Datum. Dies wäre die Anzahl aller No-Show-Registrierungspflichtigen, die die On-Demand-Aufzeichnung bis dato gesehen haben.
c. Durchschnittliche Überwachungsdauer in Minuten für alle Besucher. Dadurch erhalten Marketingexperten einen Eindruck davon, wie viel der Aufzeichnung angezeigt wird und welche intelligenten Kampagnen verwendet werden können, um Leads über einer bestimmten Überwachungsdauer auszuwählen.

SCREENSHOT

Die Filter und Trigger für interaktive Webinare wurden entsprechend den On-Demand-Webinaren geändert. Der Trigger &quot;Teilnehmer-Ereignis&quot;und der Filter &quot;Hat teilgenommen Ereignis&quot;werden mit der zusätzlichen Einschränkung &quot;Ereignismodus&quot;hinzugefügt, durch die ein Marketing-Experte auswählen kann, ob es sich um eine Live-Zielgruppe oder eine On-Demand-Zielgruppe handelt. Wenn die Beschränkung &quot;Ereignismodus&quot;nicht ausgewählt ist, werden sowohl die Live- als auch die On-Demand-Zielgruppen angesprochen. Andere Einschränkungen wie &quot;Überwachungsdatum&quot;und &quot;Überwachungsdauer&quot;können mit dem Ereignismodus &quot;On-Demand&quot;verwendet werden. Der Inaktivitätsfilter &quot;Hat kein Ereignis teilgenommen&quot;kann auch für On-Demand-Webinare mit dem Ereignismodus &quot;On-Demand&quot;verwendet werden.
