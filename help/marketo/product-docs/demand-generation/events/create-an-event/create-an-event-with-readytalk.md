---
unique-page-id: 2949870
description: Erstellen Sie ein Ereignis mit ReadyTalk - Marketing Docs - Produktdokumentation
title: Ereignis mit ReadyTalk erstellen
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---


# Ereignis mit ReadyTalk erstellen {#create-an-event-with-readytalk}

>[!PREREQUISITES]
>
>* [hinzufügen ReadyTalk als LaunchPoint-Dienst](/help/marketo/product-docs/administration/additional-integrations/add-readytalk-as-a-launchpoint-service.md)
>* [Neues Ereignis-Programm erstellen](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Legen Sie die entsprechenden [Flussaktionen](http://docs.marketo.com/display/DOCS/Flow+Actions)zur Verfolgung der Interaktion fest.


Richten Sie zuerst Ihr Ereignis im ReadyTalk Konferenzzentrum ein. Wenn Sie Hilfe benötigen, besuchen Sie das [ReadyTalk Resource Center.](https://www.readytalk.com/resources/readytalk)  Wählen Sie bei der Auswahl des Registrierungstyps die Option **Vorregistrierung vor der Sitzung**. Wenn Sie sich zum Zeitpunkt des Treffens ** registrieren lassen, erfasst Marketo **keinen** Status als &quot;Registered&quot; für Ihr Volk und wird erst *nach* Abschluss des Webinars den Status &quot;Person&quot;als &quot;teilgenommen&quot;erhalten.

Lassen Sie mich **über neue Registrierungen per E-Mail** unmarkiert benachrichtigen.

![](assets/image2015-5-28-21-3a18-3a39.png)

Wenn Sie ReadyTalk zum Senden von Bestätigungs-E-Mails verwenden, müssen Sie auch eine Beschreibung hinzufügen. Speichern Sie Ihr Ereignis in ReadyTalk, wenn Sie fertig sind.

>[!NOTE]
>
>Um ein Ereignis mit Operatorunterstützung zu planen, klicken Sie auf den Link **Ereignis-Services** anfordern auf der linken Seite des Home-Bildschirms des Konferenzzentrums, um ein Ereignis mit unserem Ereignisses-Team zu planen.

Jetzt können Sie Ihr Ereignis mit Marketo verknüpfen.

1. Wählen Sie Ihr Ereignis aus, klicken Sie dann auf **Ereignis-Aktionen** und schließlich auf **Ereignis-Einstellungen.**

   ![](assets/image2015-5-18-12-3a46-3a47.png)

   >[!NOTE]
   >
   >Der Kanal des ausgewählten Ereignisses muss ein **Webinar sein.**

1. Wählen Sie unter **Ereignis-Partner die** Option **ReadyTalk**.

   ![](assets/image2015-5-18-12-3a47-3a59.png)

1. Wählen Sie unter **Anmelden** Ihre ReadyTalk-Anmeldung aus.

   ![](assets/image2015-5-18-12-3a48-3a48.png)

1. Wählen Sie unter **Ereignis** das Ereignis aus, das Sie verknüpfen möchten, und klicken Sie dann auf **Speichern**.

   ![](assets/image2015-5-18-12-3a51-3a35.png)

   Schön! Ihr Ereignis wird jetzt synchronisiert.

   >[!NOTE]
   >
   >Die Felder, die von Marketo gesendet werden, sind: Vorname, Nachname, E-Mail-Adresse.

   >[!TIP]
   >
   >Um Ihre Bestätigungs-E-Mail mit dieser eindeutigen URL zu füllen, verwenden Sie das folgende Token in Ihrer E-Mail: `{{member.webinar url}}`. Wenn die Bestätigungs-URL gesendet wird, wird dieses Token automatisch zur eindeutigen Bestätigungs-URL der Person aufgelöst.
   >
   >Stellen Sie Ihre Bestätigungs-E-Mail auf Operational ein, um sicherzustellen, dass Personen, die sich registrieren und möglicherweise abgemeldet werden, ihre Bestätigungsinformationen erhalten.

   ![](assets/readytalk.png)

   >[!CAUTION]
   >
   >Vermeiden Sie die Verwendung verschachtelter E-Mail-Programm zum Versenden Ihrer Bestätigungs-E-Mails. Verwenden Sie stattdessen die intelligente Kampagne des Ereignis Programms, wie oben gezeigt.

   >[!TIP]
   >
   >Es kann bis zu 48 Stunden dauern, bis die Daten in Marketo angezeigt werden. Wenn Sie nach einer Wartezeit immer noch nichts sehen, wählen Sie im Menü &quot;Ereignis-Aktionen&quot;auf der Registerkarte &quot; **Zusammenfassung** &quot;Ihres Ereignisses die Option &quot;Von Webinar-Provider **** aktualisieren&quot;aus.

## Ansicht des Zeitplans  {#viewing-the-schedule}

Klicken Sie in der Ansicht [Programmplanung](http://docs.marketo.com/display/docs/program+schedule+view)auf den Kalendereintrag für Ihr Ereignis. Sie können den Zeitplan auf der rechten Seite des Bildschirms sehen!

![](assets/image2015-5-18-12-9-58.png)

Personen, die sich für Ihr Webinar anmelden, werden über den Schritt zum Ändern des Status des Programms an Ihren Webinaranbieter weitergeleitet, wenn der neue Status auf &quot;Registriert&quot;eingestellt ist. Kein anderer Status wird die Person übertreiben. Stellen Sie außerdem sicher, dass Sie den Schritt zum Ändern des Status des Programms 1 und zum Senden der E-Mail-Zustellung Schritt 2 durchführen.
