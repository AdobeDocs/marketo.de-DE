---
unique-page-id: 10096677
description: Testen der ON24-Ereignisintegration - Marketo-Dokumente - Produktdokumentation
title: Testen der ON24-Ereignisintegration
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---

# Testen der ON24-Ereignisintegration {#test-your-on-event-integration}

Testen Sie die Ereignisintegration gründlich.

## Empfohlene Testsequenz vor dem Ausführen der ersten Kampagne {#recommended-test-sequence-before-running-your-first-campaign}

1. Füllen Sie das Registrierungsformular für die Veranstaltung aus und verwenden Sie eine gültige E-Mail-Adresse zum Testen.
1. Bestätigen Sie, dass der Testname mit **Status „Registriert** im Mitgliedschaftsraster Ihres Marketo-Ereignisses angezeigt wird.
1. Bestätigen Sie, dass der Testname auch als **Registriert** in ON24 angezeigt wird.
1. Vergewissern Sie sich, dass die gültige E-Mail-Adresse, mit der Sie den Testnamen registriert haben, eine Bestätigungs-E-Mail an das Ereignis erhalten hat und dass die eindeutige URL in der E-Mail aufgelöst wurde.

   >[!NOTE]
   >
   >Sie müssen das `{{member.webinar url}}`-Token in Ihrer Bestätigungs-E-Mail verwenden, damit die eindeutige URL in der E-Mail jedes Registrierenden angezeigt wird.

## Nach dem Ereignis {#after-the-event}

So werden Daten nach dem Ereignis aktualisiert:

* Marketo ruft jede Nacht Teilnehmerdaten von ON24 ab.
* Sobald die Teilnehmerdaten zwischen Marketo und ON24 synchronisiert wurden, aktualisiert Marketo den Mitgliedschaftsstatus auf [!UICONTROL Teilgenommen], [!UICONTROL Teilgenommen bei ] oder [!UICONTROL Nicht angezeigt]. Auf der Registerkarte **[!UICONTROL Zusammenfassung]** des Ereignisses wird der Ereignisstatus auf **[!UICONTROL Ereignis abgeschlossen]** aktualisiert.

>[!MORELIKETHIS]
>
>* [Beispiel für die ON24-Ereignisintegration](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Informationen zu Marketo ON24-Adapterereignissen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
