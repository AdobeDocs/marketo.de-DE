---
description: On-Demand-Webinare - Marketo-Dokumente - Produktdokumentation
title: On-Demand-Webinare
hide: true
hidefromtoc: true
feature: Interactive Webinars
source-git-commit: 4dccf70f42153045f630bf646a6a193e27dbf637
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# On-Demand-Webinare {#on-demand-webinars}

On-Demand-Webinare erfassen und verfeinern die Leads, die sich für Ihre Veranstaltung registriert haben und nicht teilgenommen haben, aber Informationen zu der Veranstaltung erhalten möchten, indem sie die Aufzeichnung ansehen. Informationen wie Name, E-Mail-ID und Datum/Dauer der Wiedergabe können in Marketo Engage erfasst und für das Targeting dieser Leads ohne Anzeige verwendet werden.

Über die Webinar-Verbindungs-URL, die vor dem Ereignis für die Registrierungspflichtigen freigegeben wurde, können Sie sich die On-Demand-Aufzeichnung ansehen. Sobald ein Registrant, der nicht an der Live-Veranstaltung teilgenommen hat (z. B. ein Lead mit dem Programmstatus &quot;Keine Sendung&quot;), auf die Webinar-Joining-URL klickt, ändert sich der Programmstatus dieses Leads von &quot;Keine Sendung&quot; zu &quot;Teilnehmer On-Demand&quot;. Der Programmstatus der Leads, die das Ereignis live angesehen haben und den Status &quot;Teilnehmer&quot;haben, wird nicht beeinträchtigt, wenn sie die Joining-URL aufrufen und die On-Demand-Aufzeichnung ansehen.

Adobe Connect, die Technologie für interaktive Webinare, verfolgt den Besuch sowie die Überwachungsdauer in Bezug auf die Leads, die die Aufzeichnung ansehen, und meldet die Informationen täglich an Marketo. Die Aufzeichnung ist 30 Tage nach dem Ereignis unter der Verbindungs-URL verfügbar. Die Dauer kann nicht geändert werden.

Marketo stellt mithilfe der folgenden Widgets die Überwachungsstatistiken für On-Demand-Webinare auf der Registerkarte &quot;Dashboard&quot;bereit:

* On-Demand-Zusammenfassung: Diese Übersicht zeigt die Anzahl der Besucher (keine Aufnahmen), die die Aufzeichnung an einem oder mehreren Tagen nach dem Ereignis ansehen.

* On-Demand-Statistiken: Dieses Widget enthält Informationen zu:
   * Tage, an denen die On-Demand-Aufzeichnung angezeigt werden kann - Hilft Marketingexperten, Aktionen durchzuführen, z. B. E-Mail-Kampagnen auszuführen, die dem Ende der Verfügbarkeitsdauer der Aufzeichnung von 30 Tagen nahe kommen.
   * Gesamtbesucherzahl für On-Demand-Webinare bis heute - Die Anzahl aller Registrierungen ohne Anzeigen, die die On-Demand-Aufzeichnung bisher gesehen haben.
   * Durchschnittliche Überwachungsdauer in Minuten für alle Besucher - gibt Marketing-Experten einen Überblick darüber, wie viel der Aufzeichnung angezeigt wird und welche Smart-Kampagnen verwendet werden können, um Leads über eine bestimmte Überwachungsdauer hinweg als Ziel festzulegen.

![](assets/on-demand-webinars-1.png)

Die Filter und Trigger für interaktive Webinare wurden entsprechend den On-Demand-Webinaren geändert. Der Trigger &quot;Teilnehmer-Ereignis&quot;und der Filter &quot;Hat das Ereignis besucht&quot;werden mit einer zusätzlichen Einschränkung (&quot;Ereignismodus&quot;) hinzugefügt, durch die ein Marketing-Experte auswählen kann, ob es sich um eine Live-Zielgruppe oder eine On-Demand-Zielgruppe handelt. Wenn die Beschränkung &quot;Ereignismodus&quot;nicht ausgewählt ist, werden sowohl die Live- als auch die On-Demand-Zielgruppen angesprochen. Andere Einschränkungen wie &quot;Überwachungsdatum&quot;und &quot;Überwachungsdauer&quot;können mit dem Ereignismodus &quot;On-Demand&quot;verwendet werden. Der Inaktivitätsfilter &quot;Hat kein Ereignis teilgenommen&quot;kann auch für On-Demand-Webinare mit dem Ereignismodus &quot;On-Demand&quot;verwendet werden.
