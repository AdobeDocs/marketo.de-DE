---
unique-page-id: 10096681
description: Grundlegendes zum Webinar-Programmstatus - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zum Webinar-Programmstatus
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Grundlegendes zum Webinar-Programmstatus {#understanding-webinar-program-statuses}

Programmstatus stellen die verschiedenen Ereignisstatus dar, die eine Person als Mitglied des Ereignisses durchläuft. Sie sind mit einem Kanaltyp verknüpft. Marketo verfügt über einen integrierten Kanaltyp mit dem Namen **Webinar**. Status können sowohl in Batch- als auch in Trigger-Kampagnen verwendet werden.

Der Programmstatus wird linear durchlaufen, ohne dass der Programmstatus zurückgegeben wird. Beispielsweise kann eine Person mit dem Status **Teilgenommen** nicht zurück in &quot;**&quot;**.

Im Folgenden finden Sie eine kurze Beschreibung der Programmstatus, die mit dem Webinar-Kanal verknüpft sind.

>[!TIP]
>
>Um den Status manuell zu aktualisieren, klicken Sie **Vom Webinar-Anbieter aktualisieren** in der Dropdown-Liste **Ereignisaktionen**.

![](assets/image2015-12-17-13-3a52-3a39.png)

**Nicht im Programm** - Verwenden Sie diesen Status, um Personen aus dem Ereignis zu entfernen.

**Eingeladen** - Verwenden Sie diesen Status, um Personen zur Veranstaltung hinzuzufügen.

**Genehmigung ausstehend** - Verwenden Sie diesen Status, um den Versand einer Bestätigungs-E-Mail an Ihre Kontaktpersonen zu stoppen. Weitere Informationen finden Sie unter „Registranten manuell genehmigen[ in ](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"}-24-Ereignisregistrierungsaktualisierungen.

**Warteliste** - Verwenden Sie diesen Status, damit einige Personen warten, bis weitere Lizenzen verfügbar sind.

**Abgelehnt** - Verwenden Sie diesen Status, um die Registrierung einer Person für Ihre Veranstaltung abzulehnen.

**Registriert** Dieser Status überträgt Personen auf ON24, wenn Sie die ON24-Integration verwenden. Der Status der Person wird aktualisiert, wenn ON24 antwortet, dass die Person erfolgreich registriert wurde.

**Registrierungsfehler** - Dieser Status gibt an, dass der Benutzer beim Versuch, sich für das Ereignis zu registrieren, auf einen Fehler gestoßen ist.

>[!NOTE]
>
>Wenn ein Registrierungsfehler auftritt, können Sie zusätzliche Informationen für diese Person in der Spalte Status-Grund auf der Registerkarte Mitglieder Ihres Programms abrufen. Nachdem der Fehler behoben wurde, können Sie den Programmstatus des Benutzers manuell in In Marketo registriert ändern.

**Teilgenommen** - Am Ende des Webinars gibt ON24 eine Liste der Personen zurück, die teilgenommen haben. Dieser Status wird automatisch in Marketo übernommen.

**Attended On-Demand** - Personen, die an der archivierten Version des Webinars teilgenommen haben, erhalten diesen Status.

**No Show** - Nach Abschluss des Webinars und nachdem die Anwesenheitsdaten von ON24 abgerufen wurden, wird der Status der Personen, die sich registriert haben, aber nicht teilgenommen haben, auf No Show aktualisiert. Die Vorbereitung der endgültigen Anwesenheitsinformationen auf ON24 und deren Bereitstellung in Marketo kann zwischen 30 Minuten und 3 Stunden dauern.

>[!NOTE]
>
>Damit Marketo den Status „No Show“ abrufen kann, müssen die Personen (in Marketo *registriert*. Wir können keine Sendungen erfassen, die aus dem On24-Daten-Feed stammen.

>[!MORELIKETHIS]
>
>[Informationen zu Marketo ON24-Adapterereignissen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
