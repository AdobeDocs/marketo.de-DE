---
description: On-Demand-Webinare - Marketo-Dokumente - Produktdokumentation
title: On-Demand-Webinare
feature: Interactive Webinars
exl-id: 65bfc1d2-6382-4cfa-9560-69cbb0c37c42
source-git-commit: 7de0aed6be29a304276f2b3f96dd60974b4c4eb6
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# On-Demand-Webinare {#on-demand-webinars}

On-Demand-Webinare erfassen und verfeinern die Leads, die sich für Ihre Veranstaltung registriert haben und nicht teilgenommen haben. Sie möchten jedoch Informationen über die Veranstaltung erhalten, indem Sie sich die Aufzeichnung ansehen. Informationen wie Name, E-Mail-ID und Datum/Dauer der Sendung können auf Marketo Engage erfasst und zum Targeting dieser nicht angezeigten Leads verwendet werden.

Die URL für die Teilnahme am Webinar, die den Teilnehmern vor der Veranstaltung mitgeteilt wurde, kann verwendet werden, um die On-Demand-Aufzeichnung anzusehen. Wenn ein Teilnehmer, der nicht an der Live-Veranstaltung teilgenommen hat (z. B. ein Lead mit dem Programmstatus „No-Show„), auf die URL für die Teilnahme am Webinar klickt, ändert sich der Programmstatus dieses Leads von „No-Show“ in „Attended On-Demand“. Der Programmstatus der Leads, die das Ereignis live gesehen haben und den Status „Teilgenommen“ haben, wird nicht beeinflusst, wenn sie die Joining-URL aufrufen und die On-Demand-Aufzeichnung ansehen.

Adobe Connect, die Technologie für interaktive Webinare, verfolgt den Besuch sowie die Beobachtungsdauer in Bezug auf die Leads, die die Aufzeichnung ansehen, und meldet die Informationen täglich an Marketo Engage. Die Verfolgung von On-Demand-Webinaren wird 30 Tage nach dem Ereignis beendet. Die Dauer kann nicht geändert werden.

Marketo Engage stellt die Statistiken zu Armbanduhren für On-Demand-Webinare auf der Registerkarte Dashboard mithilfe der folgenden Widgets bereit:

* On-Demand-Zusammenfassung : Bietet eine Zusammenfassung der Besucherzahlen (No-Shows), die die Aufzeichnung nach dem Ereignis an einem bestimmten Tag (bestimmten Tagen) ansehen

* On-Demand-Statistiken: Dieses Widget bietet Informationen zu folgenden Themen:
   * Tage, an denen die On-Demand-Aufzeichnung zur Anzeige verfügbar ist - Hilft Marketing-Experten bei der Durchführung von Aktionen, z. B. der Ausführung von E-Mail-Kampagnen kurz vor dem Ende der Aufnahmeverfügbarkeitsdauer von 30 Tagen.
   * Bisherige Gesamtbesucherzahl für On-Demand-Webinare: Die Anzahl aller Nicht-Show-Registranten, die die On-Demand-Aufzeichnung bis heute angesehen haben.
   * Durchschnittliche Dauer der Beobachtung in Minuten für alle Besucher : Gibt Marketing-Experten einen Eindruck davon, wie viel von der Aufzeichnung angezeigt wird und welche Smart-Kampagnen verwendet werden können, um Leads oberhalb einer bestimmten Dauer der Beobachtung anzusprechen.

![](assets/on-demand-webinars-1.png)

>[!NOTE]
>
>Die Ansichten werden nur gezählt, wenn die Dauer der Uhr eine Minute überschreitet.

Die Filter und Trigger für interaktive Webinare wurden geändert, um On-Demand-Webinare zu unterstützen. Der Trigger „nimmt an Ereignis teil“ und der Filter „Hat an Ereignis teilgenommen“ werden mit einer zusätzlichen Einschränkung („Ereignismodus„) hinzugefügt, bei der ein Marketing-Experte auswählen kann, ob es sich bei der Zielgruppe um eine Live-Zielgruppe oder eine On-Demand-Zielgruppe handelt. Wenn die Beschränkung „Ereignismodus“ nicht ausgewählt ist, werden sowohl Live- als auch On-Demand-Zielgruppen angesprochen. Andere Einschränkungen wie „Überwachungsdatum“ und „Überwachungsdauer“ können mit dem Ereignismodus „On-Demand“ verwendet werden. Der Inaktivitätsfilter „Hat an einer Veranstaltung nicht teilgenommen“ kann auch für On-Demand-Webinare mit dem Ereignismodus „Auf-Anfrage“ verwendet werden.
