---
unique-page-id: 10096677
description: On24-Ereignis-Integration testen - Marketing Docs - Produktdokumentation
title: On24-Ereignis-Integration testen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# On24-Ereignis-Integration testen {#test-your-on-event-integration}

Stellen Sie sicher, dass Sie Ihre Ereignis-Integration gründlich testen.

## Empfohlene Testsequenz vor Ausführung der ersten Kampagne {#recommended-test-sequence-before-running-your-first-campaign}

1. Füllen Sie das Registrierungsformular des Ereignisses aus und verwenden Sie eine gültige E-Mail-Adresse, um es zu testen.
1. Bestätigen Sie, dass der Testname mit dem Status **Registered** im Mitgliederverzeichnis Ihres Marketo-Ereignisses angezeigt wird.
1. Bestätigen Sie, dass der Testname auch in ON24 als **Registered** angezeigt wird.
1. Vergewissern Sie sich, dass die gültige E-Mail-Adresse, die Sie zur Registrierung des Testnamens verwendet haben, eine Bestätigungs-E-Mail an das Ereignis erhalten hat und dass die eindeutige URL in der E-Mail aufgelöst wird.

   >[!NOTE]
   >
   >Sie müssen das Token `{{member.webinar url}}` in Ihrer Bestätigungs-E-Mail verwenden, damit die eindeutige URL in der E-Mail jedes Registrierungspflichtigen angezeigt wird.

## Nach dem Ereignis {#after-the-event}

So werden die Daten nach dem Ereignis aktualisiert:

* Marketo ruft täglich Teilnehmerdaten von ON24 ab.
* Nachdem die Teilnehmerdaten zwischen Marketo und ON24 synchronisiert wurden, aktualisiert Marketo den Status der Mitgliedschaft auf &quot;Anwesend&quot;, &quot;Anwesend On-Demand&quot;oder &quot;Keine Anzeige&quot;. Im Register **Zusammenfassung** des Ereignisses wird der Status des Ereignisses auf **Ereignis Complete** aktualisiert.

>[!MORELIKETHIS]
>
>* [Beispiel für eine ON24-Ereignis-Integration](example-on24-event-integration.md)
>* [Ereignisse des Marketo ON24-Adapters](understanding-marketo-on24-adapter-events.md)

>



