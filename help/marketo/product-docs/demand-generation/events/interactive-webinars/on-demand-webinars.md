---
description: On-Demand-Webinare - Marketo-Dokumente - Produktdokumentation
title: On-Demand-Webinare
feature: Interactive Webinars
exl-id: 65bfc1d2-6382-4cfa-9560-69cbb0c37c42
source-git-commit: 0bbe8110b7912cfbe04fdfc9b73c90fa9606a6b8
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# On-Demand-Webinare {#on-demand-webinars}

On-Demand-Webinare erfassen und verfeinern die Leads, die sich für Ihre Veranstaltung registriert haben und nicht teilgenommen haben, aber Informationen zu der Veranstaltung erhalten möchten, indem sie die Aufzeichnung ansehen. Informationen wie Name, E-Mail-ID und Datum/Dauer der Wiedergabe können in Marketo Engage erfasst und für das Targeting dieser Leads ohne Anzeige verwendet werden.

Über die Webinar-Verbindungs-URL, die vor dem Ereignis für die Registrierungspflichtigen freigegeben wurde, können Sie sich die On-Demand-Aufzeichnung ansehen. Sobald ein Registrant, der nicht an der Live-Veranstaltung teilgenommen hat (z. B. ein Lead mit dem Programmstatus &quot;Keine Sendung&quot;), auf die Webinar-Joining-URL klickt, ändert sich der Programmstatus dieses Leads von &quot;Keine Sendung&quot; zu &quot;Teilnehmer On-Demand&quot;. Der Programmstatus der Leads, die das Ereignis live angesehen haben und den Status &quot;Teilnehmer&quot;haben, wird nicht beeinträchtigt, wenn sie die Joining-URL aufrufen und die On-Demand-Aufzeichnung ansehen.

Adobe Connect, die Technologie für interaktive Webinare, verfolgt den Besuch und die Überwachungsdauer in Bezug auf die Leads, die die Aufzeichnung ansehen, und meldet die Informationen täglich an Marketo Engage. Das Tracking von On-Demand-Webinaren endet 30 Tage nach dem Ereignis. Die Dauer kann nicht geändert werden.

Marketo Engage stellt mithilfe der folgenden Widgets die Überwachungsstatistiken für On-Demand-Webinare auf der Registerkarte Dashboard bereit:

* On-Demand-Zusammenfassung: Diese Übersicht zeigt die Anzahl der Besucher (keine Aufnahmen), die die Aufzeichnung an einem oder mehreren Tagen nach dem Ereignis ansehen.

* On-Demand-Statistiken: Dieses Widget enthält Informationen zu:
   * Tage, an denen die On-Demand-Aufzeichnung angezeigt werden kann - Hilft Marketingexperten, Aktionen durchzuführen, z. B. E-Mail-Kampagnen auszuführen, die dem Ende der Verfügbarkeitsdauer der Aufzeichnung von 30 Tagen nahe kommen.
   * Gesamtbesucherzahl für On-Demand-Webinare bis heute - Die Anzahl aller Registrierungen ohne Anzeigen, die die On-Demand-Aufzeichnung bisher gesehen haben.
   * Durchschnittliche Überwachungsdauer in Minuten für alle Besucher - gibt Marketing-Experten einen Überblick darüber, wie viel der Aufzeichnung angezeigt wird und welche Smart-Kampagnen verwendet werden können, um Leads über eine bestimmte Überwachungsdauer hinweg als Ziel festzulegen.

![](assets/on-demand-webinars-1.png)

Die Filter und Trigger für interaktive Webinare wurden entsprechend den On-Demand-Webinaren geändert. Der Trigger &quot;Teilnehmer-Ereignis&quot;und der Filter &quot;Hat das Ereignis besucht&quot;werden mit einer zusätzlichen Einschränkung (&quot;Ereignismodus&quot;) hinzugefügt, durch die ein Marketing-Experte auswählen kann, ob es sich um eine Live-Zielgruppe oder eine On-Demand-Zielgruppe handelt. Wenn die Beschränkung &quot;Ereignismodus&quot;nicht ausgewählt ist, werden sowohl die Live- als auch die On-Demand-Zielgruppen angesprochen. Andere Einschränkungen wie &quot;Überwachungsdatum&quot;und &quot;Überwachungsdauer&quot;können mit dem Ereignismodus &quot;On-Demand&quot;verwendet werden. Der Inaktivitätsfilter &quot;Hat kein Ereignis teilgenommen&quot;kann auch für On-Demand-Webinare mit dem Ereignismodus &quot;On-Demand&quot;verwendet werden.
