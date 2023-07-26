---
unique-page-id: 10096681
description: Erläuterungen zum Webinar-Programmstatus - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zum Webinar-Programmstatus
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Grundlegendes zum Webinar-Programmstatus {#understanding-webinar-program-statuses}

Programmstatus stellen die verschiedenen Ereignisstatus dar, die eine Person als Mitglied des Ereignisses durchlaufen kann. Sie sind mit einem Kanaltyp verknüpft. Marketo verfügt über einen integrierten Kanaltyp mit dem Namen **Webinar**. Status können sowohl in Batch- als auch in Trigger-Kampagnen verwendet werden.

Menschen durchlaufen den Programmstatus linear und gehen nicht in den Status zurück. Beispiel: eine Person mit dem Status **Angemeldet** kann nicht zurück zu **Angemeldet**.

Im Folgenden finden Sie eine kurze Beschreibung des Programmstatus im Zusammenhang mit dem Webinar-Kanal.

>[!TIP]
>
>Um den Status manuell zu aktualisieren, klicken Sie auf  **Von Webinar-Anbieter aktualisieren** im **Ereignisaktionen** angezeigt.

![](assets/image2015-12-17-13-3a52-3a39.png)

**Nicht im Programm** - Verwenden Sie diesen Status, um Personen aus dem Ereignis zu entfernen.

**Eingeladen** - Verwenden Sie diesen Status, um Personen zum Ereignis hinzuzufügen.

**Ausstehende Genehmigung** - Verwenden Sie diesen Status, um Ihren Personen eine Bestätigungs-E-Mail zu senden. Siehe &quot;Manuelles Genehmigen von Registranten&quot;in [Aktualisierungen der Ereignisregistrierung in ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"} für weitere Informationen.

**Warteliste** - Verwenden Sie diesen Status, damit einige Personen warten, bis weitere Plätze verfügbar sind.

**Abgelehnt** - Verwenden Sie diesen Status, um die Registrierung einer Person für Ihr Ereignis abzulehnen.

**Angemeldet** - Dieser Status sendet Personen an ON24, wenn Sie die ON24-Integration verwenden. Der Status der Person wird aktualisiert, wenn ON24 antwortet, dass die Person erfolgreich registriert wurde.

**Registrierungsfehler** - Dieser Status spiegelt wider, dass beim Versuch, sich für das Ereignis zu registrieren, ein Fehler aufgetreten ist.

>[!NOTE]
>
>Wenn ein Registrierungsfehler auftritt, können Sie zusätzliche Informationen für diese Person erhalten, indem Sie die Spalte Status Grund auf auf der Registerkarte Mitglieder Ihres Programms ansehen. Nachdem der Fehler behoben wurde, können Sie den Programmstatus des Benutzers manuell in In Marketo registriert ändern.

**Angemeldet** - Zum Abschluss des Webinars gibt ON24 eine Liste der Teilnehmer zurück. Dieser Status wird automatisch in Marketo abgerufen.

**On-Demand teilgenommen** - Personen, die an der archivierten Version des Webinars teilgenommen haben, erhalten diesen Status.

**Keine Sendung** - Am Ende des Webinars und nach der Erfassung der Anwesenheitsdaten von ON24 wird der Status der Personen, die sich registriert, aber nicht teilgenommen haben, auf No Show aktualisiert. Es kann zwischen 30 Minuten und 3 Stunden dauern, bis ON24 die endgültigen Anwesenheitsinformationen vorbereitet und in Marketo verfügbar macht.

>[!NOTE]
>
>Damit Marketo den Status &quot;Keine Anzeige&quot;abrufen kann, müssen die Personen registriert worden sein. *in Marketo*. Wir können keine No Shows erfassen, die aus dem On24-Daten-Feed stammen.

>[!MORELIKETHIS]
>
>[Grundlegendes zu Marketo ON24-Adapterereignissen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
