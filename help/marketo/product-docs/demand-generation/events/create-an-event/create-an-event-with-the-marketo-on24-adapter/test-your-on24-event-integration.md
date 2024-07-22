---
unique-page-id: 10096677
description: Testen der ON24-Ereignisintegration - Marketo Docs - Produktdokumentation
title: Testen der ON24-Ereignisintegration
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---

# Testen der ON24-Ereignisintegration {#test-your-on-event-integration}

Stellen Sie sicher, dass Sie Ihre Ereignisintegration gründlich testen.

## Empfohlene Testsequenz vor Ausführung der ersten Kampagne {#recommended-test-sequence-before-running-your-first-campaign}

1. Füllen Sie das Registrierungsformular des Ereignisses aus und verwenden Sie eine gültige E-Mail-Adresse zum Testen.
1. Vergewissern Sie sich, dass der Testname im Mitgliedschaftsraster Ihres Marketo-Ereignisses mit dem Status **Registered** angezeigt wird.
1. Bestätigen Sie, dass der Testname in ON24 auch als **Registered** angezeigt wird.
1. Vergewissern Sie sich, dass die gültige E-Mail-Adresse, die Sie zur Registrierung des Testnamens verwendet haben, eine Bestätigungs-E-Mail an das Ereignis erhalten hat und dass die eindeutige URL in der E-Mail aufgelöst wurde.

   >[!NOTE]
   >
   >Sie müssen das `{{member.webinar url}}` -Token in Ihrer Bestätigungs-E-Mail verwenden, damit die eindeutige URL in der E-Mail jedes Registrierungspflichtigen angezeigt wird.

## Nach dem Ereignis {#after-the-event}

So werden Daten aktualisiert, nachdem das Ereignis stattgefunden hat:

* Marketo ruft täglich Teilnehmerdaten von ON24 ab.
* Nachdem die Teilnehmerdaten zwischen Marketo und ON24 synchronisiert wurden, aktualisiert Marketo den Mitgliedschaftsstatus auf &quot;Teilnehmer&quot;, &quot;Abonniert On-Demand&quot;oder &quot;Keine Anzeige&quot;. Auf der Registerkarte **Zusammenfassung** des Ereignisses wird der Ereignisstatus auf **Event Complete** aktualisiert.

>[!MORELIKETHIS]
>
>* [Beispiel für ON24-Ereignisintegration](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Grundlegendes zu Marketo ON24-Adapterereignissen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
