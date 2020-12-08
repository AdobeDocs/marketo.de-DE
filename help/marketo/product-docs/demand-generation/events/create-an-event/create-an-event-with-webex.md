---
unique-page-id: 2949863
description: Ereignis mit WebEx - Marketing Docs - Produktdokumentation erstellen
title: Ereignis mit WebEx erstellen
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '941'
ht-degree: 0%

---


# Ereignis mit WebEx erstellen {#create-an-event-with-webex}

>[!NOTE]
>
>**Voraussetzungen**
>
>* [hinzufügen von WebEx als LaunchPoint-Dienst](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Neues Ereignis-Programm erstellen](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Legen Sie die entsprechenden [Flussaktionen](http://docs.marketo.com/display/DOCS/Flow+Actions)zur Verfolgung der Interaktion fest.


Erstellen Sie zunächst ein Webex-Ereignis im WebEx Ereignis Center. Marketo verwendet nur bestimmte Einstellungen und Felder für Ihre Integration, die wir in Kürze durchführen werden. Andere Felder, die Sie für WebEx konfigurieren möchten, werden im [WebEx Ereignis Center Benutzerhandbuch](http://www.cisco.com/c/dam/en/us/td/docs/collaboration/meeting_center/wbs298/wx_ec_host_ug.pdf)beschrieben.

## Basisinformationen {#basic-information}

* **Name des Ereignisses -** Dieser Name wird in Marketo angezeigt.
* **Kontrollkästchen nicht aufgeführt**

   * Es wird empfohlen, dass Sie Ihr Ereignis **nicht** Liste. Dadurch wird sichergestellt, dass sich alle Personen über Ihre Marketo-Landingpage registrieren. Personen, die sich über einen anderen Mechanismus als Marketo registrieren, werden in Marketo nach Abschluss des Ereignisses angezeigt UND nur, wenn sie an dem Ereignis teilgenommen haben.
   * Wenn Sie sich für die Liste des Ereignisses entscheiden, wird es auf der Seite &quot;Liste der Ereignis&quot;für alle Benutzer angezeigt, die Ihre Ereignis Center-Website besuchen.

* **Registrierung -** Aktivieren Sie dieses Kontrollkästchen, um den Wert &quot;Erforderlich&quot;festzulegen. Sie verwenden ein Marketo-Formular/eine Landingpage, um Registrierungsinformationen zu erfassen, die an WebEx gesendet werden.
* **Ereignis Password**- (optional) Wenn Sie dieses Feld verwenden, vergewissern Sie sich, dass es in Ihrer Bestätigungs-E-Mail enthalten ist!

![](assets/image2015-5-28-13-3a30-3a55.png)

## Datum und Uhrzeit {#date-time}

* **Datum** des Beginns - Geben Sie das Datum Ihres Beginns ein. Dies wird in Marketo sichtbar sein.

* **Beginn** - Geben Sie die Uhrzeit Ihres Beginns ein. Dies wird in Marketo sichtbar sein.

* **Geschätzte Dauer** - Geben Sie die Dauer des Ereignisses an. Dies wird in Marketo sichtbar sein.

* **Zeitzonen** - Geben Sie die entsprechenden Zeitzonen ein. Sie werden in Marketo sichtbar sein.

![](assets/image2015-5-28-13-3a37-3a39.png)

## Einstellungen für Audiokonferenzen {#audio-conference-settings}

Diese Einstellungen befinden sich nur in WebEx. Sie werden nicht von Marketo benutzt oder sind in Marketo sichtbar, aber sie können für Ihr Webinar wichtig sein, also überprüfen Sie die Dublette!

## Ereignis - Beschreibung und Optionen  {#event-description-options}

Die folgenden Optionen werden von Marketo verwendet oder können angezeigt werden. Andere Felder befinden sich nur in WebEx.

* **Beschreibung** - Geben Sie eine Beschreibung ein. Dies ist in Marketo sichtbar, aber nicht änderbar.
* **Post-Ereignis-Umfrage** - Marketing ist derzeit nicht in der Lage, die Informationen auf einer WebEx-Post-Ereignis-Umfrage zu erfassen.
* **Ziel-URL** - (optional) Sie können die URL einer Marketing-Landingpage als Ziel-URL eingeben, die nach dem Ende der Sitzung angezeigt werden soll.

![](assets/image2015-5-28-13-3a48-3a49.png)

## Teilnehmer/innen und Registrierung {#attendees-registration}

Sie steuern die Einladungs-Liste, das Registrierungsformular und andere E-Mails mit einem Marketing-Ereignis. Andere Funktionen wie:

* **Maximale Anzahl der Registrierungspflichtigen** - Wird derzeit **nicht** von der Marketing-WebEx-Integration unterstützt.  Die manuelle Zulassung von Registrierungspflichtigen ist über den Status &quot;Ausstehende Genehmigung&quot; in Marketing verfügbar.

* **Registrierungs-ID erforderlich** - Wird derzeit mit der Marketing-WebEx-Integration unterstützt. Sie können Marketo verwenden, um die Bestätigungs-E-Mail für Ihr Ereignis zu senden. Wenn sich die Person registriert, erhält sie eine eindeutige URL, die sie zur Eingabe des Ereignisses verwendet.

   >[!TIP]
   >
   >Um Ihre Bestätigungs-E-Mail mit dieser eindeutigen URL zu füllen, verwenden Sie das folgende Token in Ihrer E-Mail: `{{member.webinar url}}`. Wenn die Bestätigungs-URL gesendet wird, wird dieses Token automatisch zur eindeutigen Bestätigungs-URL der Person aufgelöst.
   >
   >Stellen Sie Ihre Bestätigungs-E-Mail auf **Operational** ein, um sicherzustellen, dass Personen, die sich registrieren und abgemeldet werden können, weiterhin ihre Bestätigungsinformationen erhalten.

* **Registrierungskennwort** - (Optional) Wird derzeit nicht von der Marketing-WebEx-Integration unterstützt.
* **Genehmigungsregeln** - Wird derzeit nicht von der Marketing-WebEx-Integration unterstützt. Sie können jedoch intelligente Kampagnen in Marketing verwenden, um Genehmigungen zu steuern.

![](assets/image2015-5-28-14-3a4-3a41.png)

### Moderatoren und Panelmitglieder {#presenters-panelists}

Die in diesem Abschnitt konfigurierten Informationen werden nicht an Marketo weitergeleitet.

### E-Mail-Nachrichten {#email-messages}

Mit Marketo senden Sie E-Mails an Ihre Registrierungspflichtigen, Bestätigungs-E-Mails usw. Sie müssen nichts in diesem Abschnitt konfigurieren. Deaktivieren (deaktivieren) Sie die Optionen für E-Mail-Nachrichten in WebEx.

![](assets/image2015-5-28-14-3a9-3a14.png)

>[!NOTE]
>
>Die Marketing-WebEx-Integration kann das Senden von Bestätigungs-E-Mails aus WebEx nicht unterstützen. Die Bestätigung muss über Marketo verschickt werden. Nachdem Sie das Ereignis geplant haben, kopieren Sie die Informationen zum Ereignis in die Bestätigungs-E-Mail von Marketing und legen Sie die E-Mail als **Operativ** fest.

Jetzt sind wir bereit, nach Marketo zu springen!

1. Wählen Sie das erstellte Ereignis aus. Öffnen Sie die Dropdownliste **Ereignis-Aktionen** . Wählen Sie &quot; **Ereignis-Einstellungen&quot;.**

   ![](assets/image2015-5-14-16-3a7-3a31.png)

   >[!NOTE]
   >
   >Der Kanal des ausgewählten Ereignisses muss ein **Webinar** sein.

1. Wählen Sie unter **Ereignis Partner** die Option **WebEx**.

   ![](assets/image2015-1-30-13-3a58-3a2.png)

1. Wählen Sie unter **Anmelden** Ihre WebEx-Anmeldung.

   ![](assets/image2015-5-18-12-3a2-3a26.png)

1. Wählen Sie unter **Ereignis** Ihr frisch erstelltes WebEx-Ereignis aus. Wählen Sie dann eine optionale Sicherungsseite und klicken Sie auf **Speichern**.

   ![](assets/image2015-5-14-16-3a15-3a55.png)

1. Wählen Sie eine optionale Sicherungsseite für Ihr WebEx-Ereignis. Wählen Sie aus der Dropdown-Liste der genehmigten Marketo-Landingpages oder geben Sie die URL einer Nicht-Markieren-Landingpage ein.

   >[!TIP]
   >
   >Legen Sie eine Sicherungsseite fest, um ein Mitglied auf eine bestimmte Seite zu leiten, wenn es vor dem Beginn des Ereignisses auf seine benutzerdefinierte Ereignis-URL klickt.

   >[!NOTE]
   >
   >Die Felder, die von Marketo gesendet werden, sind: Vorname, Nachname, E-Mail-Adresse.

   ![](assets/webex.png)

   >[!CAUTION]
   >
   >Vermeiden Sie die Verwendung verschachtelter E-Mail-Programm zum Versenden Ihrer Bestätigungs-E-Mails. Verwenden Sie stattdessen die intelligente Kampagne des Ereignis Programms, wie oben gezeigt.

   >[!TIP]
   >
   >Es kann bis zu 48 Stunden dauern, bis die Daten in Marketo angezeigt werden. Wenn Sie nach einer Wartezeit immer noch nichts sehen, wählen Sie im Menü &quot;Ereignis-Aktionen&quot;auf der Registerkarte &quot; **Zusammenfassung** &quot;Ihres Ereignisses die Option &quot;Von Webinar-Provider **** aktualisieren&quot;aus.

Süß! Ihr WebEx-Ereignis wird jetzt mit Ihrem Marketo-Ereignis synchronisiert.  Personen, die sich für Ihr Webinar anmelden, werden über den Schritt zum Ändern des Status des Programms an Ihren Webinaranbieter weitergeleitet, wenn der neue Status auf &quot;Registriert&quot;eingestellt ist. Kein anderer Status wird die Person übertreiben. Stellen Sie außerdem sicher, dass Sie den Schritt zum Ändern des Status des Programms 1 und zum Senden der E-Mail-Zustellung Schritt 2 durchführen.

## Ansicht des Zeitplans  {#viewing-the-schedule}

Klicken Sie in der Ansicht [Programmplanung](http://docs.marketo.com/display/docs/program+schedule+view)auf den Kalendereintrag für Ihr Ereignis. Sie können den Zeitplan auf der rechten Seite des Bildschirms sehen!

![](assets/image2015-5-14-16-3a21-3a41.png)

>[!NOTE]
>
>Um den Zeitplan Ihres Ereignisses zu ändern, müssen Sie das Webinar auf WebEx bearbeiten.
