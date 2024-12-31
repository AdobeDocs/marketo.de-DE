---
unique-page-id: 2949863
description: Erstellen eines Ereignisses mit WebEx - Marketo-Dokumente - Produktdokumentation
title: Erstellen eines Ereignisses mit WebEx
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
feature: Events
source-git-commit: 7edce24c2199a6a2eaa119d3ef77543bbd97999c
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 1%

---

# Erstellen eines Ereignisses mit WebEx {#create-an-event-with-webex}

Nachdem Sie ein Webinar in WebEx erstellt haben, müssen Sie Ihr Ereignis mit Marketo Engage synchronisieren.

>[!PREREQUISITES]
>
>* [Hinzufügen von WebEx als LaunchPoint-Service](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Erstellen eines neuen Veranstaltungsprogramms](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Legen Sie die entsprechenden [Fluss-Aktionen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) fest, um die Interaktion zu verfolgen

## Planen eines Webinars {#schedule-your-webinar}

Sie planen Ihre Veranstaltung und wählen Ihre bevorzugten Einstellungen in [WebEx](https://www.webex.com/){target="_blank"}. In Marketo können nur die folgenden Informationen angezeigt werden: Name des Webinars, Start-/Enddatum und -zeit, Zeitzone und Beschreibung. Weitere Informationen zu Webinaren [finden Sie hier](https://help.webex.com/en-us/landing/ld-7srxjs-WebexWebinars/Webex-Webinars){target="_blank"}.

### Grundlegende Informationen {#basic-information}

![](assets/create-an-event-with-webex-1.png)

* **Thema**: Dies ist Ihr Ereignisname und kann in Marketo angezeigt werden.
* **Datum und Uhrzeit**: Start-/Enddatum, Start-/Endzeit, Dauer und Zeitzone sind in Marketo verfügbar.
* **Maximale Teilnehmerzahl**: Die maximale Teilnehmerzahl bestimmt, welche WebEx-Funktionen unterstützt werden.
* **Webcast-Ansicht für Teilnehmer**: Vergewissern Sie sich, dass Ihr Webinar live an alle Teilnehmer gestreamt wird.
* **Panelists**: Laden Sie bestimmte Personen ein, an Ihrem Webinar teilzunehmen.
* **Webinar-Agenda**: Füllen Sie diese aus, wenn Sie Kontext in der E-Mail-Einladung bereitstellen möchten, die an Diskussionsteilnehmer gesendet wird.

### Sicherheit {#security}

![](assets/create-an-event-with-webex-2.png)

* **Webinar-Passwort**: (Optional) Wenn Sie dieses Feld verwenden, stellen Sie sicher, dass Sie es in Ihre Bestätigungs-E-Mail aufnehmen.
* **Kennwort der**: (Optional) Wenn Sie dieses Feld verwenden, stellen Sie sicher, dass Sie es in Ihre Webinar-Agenda aufnehmen.
* **Konto verlangen**: Beschränkt Teilnehmer auf diejenigen, die WebEx-Konten haben.

### Audioverbindungsoptionen {#audio-connection-options}

![](assets/create-an-event-with-webex-3.png)

* **Audioverbindungstyp**: Wählen Sie aus, wie die Webinar-Teilnehmer dem Audioteil Ihres Webinars beitreten.
* **Ein- und**: Wählen Sie den Ton aus, den Benutzer hören sollen, wenn jemand das Webinar betritt oder verlässt (Telefonaudioverbindung erforderlich).
* **Bedienfeldliste stummschalten**: Wählen Sie die gewünschten Einstellungen für die Bedienfeldliste mit Stummschaltung aus.

### Erweiterte Optionen {#advanced-options}

![](assets/create-an-event-with-webex-4.png)

* **Automatische Aufzeichnung**: Überprüfen Sie dies, damit Ihr Webinar automatisch aufgezeichnet wird.
* **Übungssitzung** Überprüfen Sie dies, damit zu Beginn des Webinars eine Übungssitzung gestartet wird.
* **Breakout-Sitzungen**: Mit Breakout-Sitzungen können Sie Diskussionsteilnehmer und Teilnehmer vor Beginn des Webinars zuweisen oder ihnen die Teilnahme am Webinar ermöglichen.
* **Webinar-Reihe**: Durch das Hinzufügen zu einer Webinar-Reihe können Benutzer Ihr Webinar sehen, unabhängig davon, ob es öffentlich ist oder nicht.
* **Registrierung**: Teilnehmer müssen sich registrieren und vom Host genehmigen lassen, bevor sie teilnehmen.
* **E-Mail-Erinnerung**: Wählen Sie eine E-Mail-Erinnerung, die zwischen 15 Minuten und dem Beginn des Webinars bis zu zwei Tage dauern soll.
* **Webinar-Optionen**: Bestimmen Sie, welche Funktionen den Teilnehmern am Webinar zur Verfügung stehen.
* **Teilnehmerberechtigungen**: Die Teilnehmerberechtigungen bestimmen die Aktionen, die den Webinar-Teilnehmern zur Verfügung stehen.

>[!NOTE]
>
>Die Marketo-WebEx-Integration unterstützt nicht das Senden von Bestätigungs-E-Mails aus WebEx heraus. Die Bestätigung muss über Marketo gesendet werden. Kopieren Sie nach der Planung der Veranstaltung die Ereignisinformationen in die Marketo-Bestätigungs-E-Mail und setzen Sie die E-Mail auf _Operational_.

## Ereignis mit Marketo Engage synchronisieren {#sync-your-event-with-marketo-engage}

1. Suchen und wählen Sie in Marketo das gewünschte Veranstaltungsprogramm aus. Wählen Sie in **Dropdown** Liste Ereignisaktionen die Option **Ereigniseinstellungen** aus.

   ![](assets/create-an-event-with-webex-5.png)

   >[!NOTE]
   >
   >Der Kanaltyp des ausgewählten Ereignisses muss „Webinar **sein**.

1. Wählen Sie in **Dropdown** Liste „Veranstaltungspartner“ die Option **Webinare**.

   ![](assets/create-an-event-with-webex-6.png)

1. Wählen Sie in **Dropdown-** „Anmelden“ Ihre WebEx-Anmeldung aus.

   ![](assets/create-an-event-with-webex-7.png)

1. Wählen Sie in **Dropdown-** „Ereignis“ Ihr WebEx-Ereignis aus.

   ![](assets/create-an-event-with-webex-8.png)

1. Ihre Webinar-Details werden angezeigt. Klicken Sie auf **Speichern**.

   ![](assets/create-an-event-with-webex-9.png)

Ihr WebEx-Ereignis wird jetzt mit Ihrem Marketo-Veranstaltungsprogramm synchronisiert. Personen, die sich für Ihr Webinar anmelden, werden über den Flussschritt _Programmstatus ändern_ an Ihren Webinar-Anbieter weitergeleitet, wenn der neue Status auf „Registriert“ gesetzt ist. Kein anderer Status überträgt die Person. Stellen Sie sicher _dass Sie den Flussschritt_ Programmstatus ändern#1 und den _E-Mail senden_ #2.

## Zu beachtende Punkte {#things-to-note}

* Vermeiden Sie verschachtelte E-Mail-Programme, um Ihre Bestätigungs-E-Mails zu senden. Verwenden Sie stattdessen die intelligente Kampagne Ihres Veranstaltungsprogramms.

* Es kann bis zu 48 Stunden dauern, bis Daten in Marketo angezeigt werden. Wenn Sie nach so langer Wartezeit immer noch nichts sehen, klicken Sie auf **Vom Webinar-Anbieter aktualisieren** in der Dropdown-Liste **Ereignisaktionen** auf der Registerkarte **Zusammenfassung** Ihres Veranstaltungsprogramms.
