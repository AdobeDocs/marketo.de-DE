---
unique-page-id: 2949863
description: Erstellen eines Ereignisses mit Webex - Marketo Docs - Produktdokumentation
title: Erstellen eines Ereignisses mit Webex
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
feature: Events
source-git-commit: 7edce24c2199a6a2eaa119d3ef77543bbd97999c
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 1%

---

# Erstellen eines Ereignisses mit Webex {#create-an-event-with-webex}

Nachdem Sie ein Webinar in Webex erstellt haben, müssen Sie Ihr Ereignis mit Marketo Engage synchronisieren.

>[!PREREQUISITES]
>
>* [Webex als LaunchPoint-Dienst hinzufügen](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Neues Ereignisprogramm erstellen](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Legen Sie die entsprechenden [Fluss-Aktionen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) fest, um die Interaktion zu verfolgen.

## Webinar planen {#schedule-your-webinar}

Sie planen Ihr Ereignis und wählen Ihre bevorzugten Einstellungen in [Webex](https://www.webex.com/){target="_blank"} aus. In Marketo sind nur die folgenden Informationen sichtbar: Webinarname, Start-/Enddatum/-zeit, Zeitzone und Beschreibung. Weitere Informationen zu Webex-Webinaren [finden Sie hier](https://help.webex.com/en-us/landing/ld-7srxjs-WebexWebinars/Webex-Webinars){target="_blank"}.

### Grundlegende Informationen {#basic-information}

![](assets/create-an-event-with-webex-1.png)

* **Thema**: Dies ist Ihr Ereignisname und kann in Marketo angezeigt werden.
* **Datum und Uhrzeit**: Start-/Enddatum, Start-/Endzeit, Dauer und Zeitzone sind in Marketo alle sichtbar.
* **Maximale Teilnehmer**: Die maximale Anzahl der Teilnehmer bestimmt, welche Webfunktionen unterstützt werden.
* **Webcast-Ansicht für Teilnehmer**: Aktivieren Sie diese Option, damit Ihr Webinar für alle Teilnehmer live gestreamt wird.
* **Panelisten**: Laden Sie bestimmte Personen zu Panelisten in Ihr Webinar ein.
* **Webinar-Agenda**: Füllen Sie diese aus, wenn Sie Kontext in der E-Mail-Einladung bereitstellen möchten, die an Panelisten gesendet wird.

### Sicherheit {#security}

![](assets/create-an-event-with-webex-2.png)

* **Webinar-Kennwort**: (optional) Wenn Sie dieses Feld verwenden, stellen Sie sicher, dass Sie es in Ihre Bestätigungs-E-Mail aufnehmen.
* **Passwort der Bedienfeldliste**: (optional) Wenn Sie dieses Feld verwenden, stellen Sie sicher, dass Sie es in Ihre Webinar-Agenda aufnehmen.
* **Konto anfordern**: Beschränkt die Teilnehmer auf die Teilnehmer, die über ein Webkonto verfügen.

### Optionen zur Audioverbindung {#audio-connection-options}

![](assets/create-an-event-with-webex-3.png)

* **Audio-Verbindungstyp**: Wählen Sie aus, wie Webinar-Teilnehmer am Audio-Teil Ihres Webinars teilnehmen.
* **Ein- und Ausstiegston**: Wählen Sie den Ton aus, den Benutzer verwenden sollen, wenn ein Benutzer das Webinar betritt oder verlässt (Telefonaudioverbindung erforderlich).
* **Stummschaltfläche**: Wählen Sie die gewünschten Einstellungen für die Stummschaltung der Bedienfeldliste aus.

### Erweiterte Optionen {#advanced-options}

![](assets/create-an-event-with-webex-4.png)

* **Automatische Aufzeichnung**: Aktivieren Sie diese Option, damit Ihr Webinar automatisch aufgezeichnet wird.
* **Praktische Sitzung**: Aktivieren Sie diese Option, damit eine Übungssitzung gestartet wird, wenn das Webinar beginnt.
* **Aufschlüsselungssitzungen**: Mithilfe von Aufschlüsselungssitzungen können Sie Panelisten und Teilnehmer vorab zuweisen, bevor das Webinar beginnt, oder ihnen die Teilnahme am Webinar ermöglichen.
* **Webinar-Reihe**: Durch Hinzufügen zu einer Webinar-Reihe können Benutzer sehen, ob Ihr Webinar öffentlich ist oder nicht.
* **Registrierung**: Erfordert, dass sich Teilnehmer registrieren und die Hostgenehmigung erhalten, bevor sie teilnehmen können.
* **E-Mail-Erinnerung**: Wählen Sie eine E-Mail-Erinnerung aus, die zwischen 15 Minuten vor dem Beginn des Webinars und zwei Tagen liegt.
* **Webinaroptionen**: Bestimmen Sie, welche Funktionen den Teilnehmern des Webinars zur Verfügung stehen.
* **Teilnehmerberechtigungen**: Die Teilnehmerberechtigungen bestimmen die Aktionen, die Webinarteilnehmern zur Verfügung stehen.

>[!NOTE]
>
>Die Marketo-Webbex-Integration kann das Senden von Bestätigungs-E-Mails von Webex nicht unterstützen. Die Bestätigung muss über Marketo erfolgen. Nachdem Sie das Ereignis geplant haben, kopieren Sie die Ereignisinformationen in die Marketo-Bestätigungs-E-Mail und stellen Sie die E-Mail auf _Operativ_ ein.

## Ereignis synchronisieren mit Marketo Engage {#sync-your-event-with-marketo-engage}

1. Suchen und wählen Sie in Marketo das gewünschte Veranstaltungsprogramm aus. Wählen Sie in der Dropdown-Liste **Ereignisaktionen** die Option **Ereigniseinstellungen** aus.

   ![](assets/create-an-event-with-webex-5.png)

   >[!NOTE]
   >
   >Der Kanaltyp des ausgewählten Ereignisses muss **webinar** sein.

1. Wählen Sie in der Dropdown-Liste **Partner des Ereignisses** die Option **Webinare des Webex** aus.

   ![](assets/create-an-event-with-webex-6.png)

1. Wählen Sie in der Dropdown-Liste **Anmeldung** Ihre Webanmeldung aus.

   ![](assets/create-an-event-with-webex-7.png)

1. Wählen Sie in der Dropdownliste **Ereignis** Ihr Webex-Ereignis aus.

   ![](assets/create-an-event-with-webex-8.png)

1. Ihre Webinardetails werden ausgefüllt. Klicken Sie auf **Speichern**.

   ![](assets/create-an-event-with-webex-9.png)

Ihr Webex-Ereignis wird jetzt mit Ihrem Marketo-Ereignisprogramm synchronisiert. Personen, die sich für Ihr Webinar anmelden, werden über den Flow-Schritt _Programmstatus ändern_ an Ihren Webinar-Provider gepusht, wenn der neue Status auf &quot;Registriert&quot;gesetzt ist. Kein anderer Status wird die Person überstürzen. Stellen Sie sicher, dass Schritt 1 _Programmstatus ändern_ und Schritt 2: E-Mail senden _ausgeführt werden._

## Zu beachten {#things-to-note}

* Vermeiden Sie den Versand von Bestätigungs-E-Mails durch verschachtelte E-Mail-Programme. Verwenden Sie stattdessen die Smart-Kampagne Ihres Ereignisprogramms.

* Es kann bis zu 48 Stunden dauern, bis Daten in Marketo angezeigt werden. Wenn Sie nach so langer Wartezeit immer noch nichts sehen, klicken Sie auf **Von Webinar-Anbieter aktualisieren** in der Dropdown-Liste **Ereignisaktionen** auf der Registerkarte **Zusammenfassung** Ihres Ereignisprogramms.
