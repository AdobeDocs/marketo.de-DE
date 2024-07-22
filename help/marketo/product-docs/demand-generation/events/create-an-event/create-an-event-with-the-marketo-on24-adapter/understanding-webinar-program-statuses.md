---
unique-page-id: 10096681
description: Erläuterungen zum Webinar-Programmstatus - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zum Webinar-Programmstatus
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Grundlegendes zum Webinar-Programmstatus {#understanding-webinar-program-statuses}

Programmstatus stellen die verschiedenen Ereignisstatus dar, die eine Person als Mitglied des Ereignisses durchlaufen kann. Sie sind mit einem Kanaltyp verknüpft. Marketo verfügt über einen integrierten Kanaltyp namens **Webinar**. Status können sowohl in Batch- als auch in Trigger-Kampagnen verwendet werden.

Menschen durchlaufen den Programmstatus linear und gehen nicht in den Status zurück. Beispielsweise kann eine Person mit dem Status &quot;**Angemeldet**&quot; nicht zu &quot;**Registered**&quot; zurückkehren.

Im Folgenden finden Sie eine kurze Beschreibung des Programmstatus im Zusammenhang mit dem Webinar-Kanal.

>[!TIP]
>
>Um den Status manuell zu aktualisieren, klicken Sie in der Dropdown-Liste **Ereignisaktionen** auf **Von Webinar-Anbieter aktualisieren** .

![](assets/image2015-12-17-13-3a52-3a39.png)

**Nicht im Programm** - Verwenden Sie diesen Status, um Personen aus dem Ereignis zu entfernen.

**Eingeladen** - Verwenden Sie diesen Status, um dem Ereignis Personen hinzuzufügen.

**Ausstehende Genehmigung** - Mit diesem Status können Sie verhindern, dass Ihre Personen eine Bestätigungs-E-Mail erhalten. Weitere Informationen finden Sie unter &quot;Manuelles Genehmigen von Registrierungen&quot;in [ON24 Update zur Ereignisregistrierung](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"} .

**Warten auf Liste** - Verwenden Sie diesen Status, um zu verhindern, dass einige Personen warten, bis weitere Plätze verfügbar sind.

**Abgelehnt** - Mit diesem Status können Sie die Registrierung einer Person für Ihr Ereignis ablehnen.

**Registered** - Dieser Status sendet Personen an ON24, wenn Sie die ON24-Integration verwenden. Der Status der Person wird aktualisiert, wenn ON24 antwortet, dass die Person erfolgreich registriert wurde.

**Registrierungsfehler** - Dieser Status zeigt, dass beim Versuch, sich für das Ereignis zu registrieren, ein Fehler aufgetreten ist.

>[!NOTE]
>
>Wenn ein Registrierungsfehler auftritt, können Sie zusätzliche Informationen für diese Person erhalten, indem Sie die Spalte Status Grund auf auf der Registerkarte Mitglieder Ihres Programms ansehen. Nachdem der Fehler behoben wurde, können Sie den Programmstatus des Benutzers manuell in In Marketo registriert ändern.

**Teilnehmer** - Zum Abschluss des Webinars gibt ON24 eine Liste der Teilnehmer zurück. Dieser Status wird automatisch in Marketo abgerufen.

**Teilnehmer On-Demand** - Personen, die an der archivierten Version des Webinars teilgenommen haben, erhalten diesen Status.

**No Show** - Am Ende des Webinars und nach der Erfassung der Anwesenheitsdaten von ON24 wird der Status der Personen, die sich registriert, aber nicht teilgenommen haben, auf &quot;No Show&quot;aktualisiert. Es kann zwischen 30 Minuten und 3 Stunden dauern, bis ON24 die endgültigen Anwesenheitsinformationen vorbereitet und in Marketo verfügbar macht.

>[!NOTE]
>
>Damit Marketo den Status &quot;Keine Anzeige&quot;abrufen kann, müssen die Personen *in Marketo* registriert worden sein. Wir können keine No Shows erfassen, die aus dem On24-Daten-Feed stammen.

>[!MORELIKETHIS]
>
>[Grundlegendes zu Marketo ON24-Adapterereignissen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
