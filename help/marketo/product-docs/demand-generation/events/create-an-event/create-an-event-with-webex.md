---
unique-page-id: 2949863
description: Erstellen eines Ereignisses mit WebEx - Marketo Docs - Produktdokumentation
title: Erstellen eines Ereignisses mit WebEx
exl-id: 25266a6b-3951-46d1-8700-b36d7086ad2c
source-git-commit: ed9146f48aecd34025d61abf14d76a714726dcc9
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# Erstellen eines Ereignisses mit WebEx {#create-an-event-with-webex}

>[!PREREQUISITES]
>
>* [Hinzufügen von WebEx als LaunchPoint-Dienst](/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md)
>* [Neues Ereignisprogramm erstellen](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Legen Sie die entsprechende [Flussaktionen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) Interaktion verfolgen
>* Stellen Sie sicher, dass Sie Webex-Ereignisse (klassisch) verwenden


Erstellen Sie zunächst ein Webex-Ereignis im WebEx Event Center. Marketo verwendet nur bestimmte Einstellungen und Felder für Ihre Integration, die wir in Kürze durchgehen werden. Andere Felder, die Sie für WebEx konfigurieren möchten, werden im Abschnitt [WebEx Event Center-Benutzerhandbuch](https://www.cisco.com/c/dam/en/us/td/docs/collaboration/meeting_center/wbs298/wx_ec_host_ug.pdf).

>[!IMPORTANT]
>
>Marketo Engage unterstützt nur Ereignisse, die in Webex-Ereignissen (klassisch) erstellt wurden. Marketo unterstützt derzeit keine in Webex-Ereignissen (neu) erstellten Ereignisse.

## Grundlegende Informationen {#basic-information}

* **Ereignisname -** Dieser Name ist in Marketo sichtbar.
* **Kontrollkästchen &quot;Nicht aufgeführt&quot;**

   * Es wird empfohlen, **not** auflisten. Dadurch wird sichergestellt, dass sich alle Personen über Ihre Marketo-Landingpage registrieren. Personen, die sich über einen anderen Mechanismus als Marketo registrieren, werden in Marketo angezeigt, nachdem das Ereignis abgeschlossen wurde UND nur, wenn sie an dem Ereignis teilgenommen haben.
   * Wenn Sie das Ereignis auflisten, wird es auf der Seite &quot;Ereignisliste&quot;für jeden angezeigt, der Ihre Website im Ereigniszentrum besucht.

* **Registrierung -** Aktivieren Sie dieses Kontrollkästchen, um &quot;erforderlich&quot;festzulegen. Sie verwenden ein Marketo-Formular/eine Landingpage, um Registrierungsinformationen zu erfassen, die an WebEx gesendet werden.
* **Ereigniskennwort**- (optional) Wenn Sie dieses Feld verwenden, stellen Sie sicher, dass Sie es in Ihre Bestätigungs-E-Mail aufnehmen!

![](assets/image2015-5-28-13-3a30-3a55.png)

## Datum &amp; Uhrzeit {#date-time}

* **Startdatum** - Geben Sie Ihr Startdatum ein. Dies ist in Marketo sichtbar.

* **Startzeit** - Geben Sie Ihre Startzeit ein. Dies ist in Marketo sichtbar.

* **Geschätzte Dauer** - Geben Sie die Dauer des Ereignisses an. Dies ist in Marketo sichtbar.

* **Zeitzonen** - Geben Sie die entsprechenden Zeitzonen an. Sie werden in Marketo sichtbar sein.

![](assets/image2015-5-28-13-3a37-3a39.png)

## Einstellungen für Audiokonferenzen {#audio-conference-settings}

Diese Einstellungen befinden sich nur in WebEx. Sie werden nicht von Marketo verwendet oder können in angezeigt werden, aber sie können für Ihr Webinar wichtig sein. Überprüfen Sie sie also!

## Ereignisbeschreibung und -optionen  {#event-description-options}

Die folgenden Optionen werden von Marketo verwendet oder können in angezeigt werden. Andere Felder befinden sich nur in WebEx.

* **Beschreibung** - Geben Sie eine Beschreibung ein. Dies ist in Marketo sichtbar, kann aber nicht geändert werden.
* **Umfrage nach Ereignissen** - Marketo kann die Informationen zu einer WebEx-Post-Event-Umfrage derzeit nicht erfassen.
* **Ziel-URL** - (optional) Sie können die URL einer Marketo-Landingpage eingeben, die als Ziel-URL dienen soll, die nach dem Ende der Sitzung angezeigt wird.

![](assets/image2015-5-28-13-3a48-3a49.png)

## Teilnehmer und Registrierung {#attendees-registration}

Mit einem Marketo-Ereignis steuern Sie die Einladungsliste, das Registrierungsformular und andere E-Mails. Andere Funktionen werden von Marketo nicht unterstützt, darunter:

* **Höchstzahl der Registranten** - Derzeit **not** unterstützt über die Marketo-WebEx-Integration.  Die manuelle Validierung von Registrierungspflichtigen ist über den Fortschrittsstatus Ausstehende Genehmigung in Marketo verfügbar.

* **Registrierungs-ID erforderlich** - Wird derzeit mit der Marketo-WebEx-Integration unterstützt. Sie können Marketo verwenden, um die Bestätigungs-E-Mail für Ihr Ereignis zu senden. Wenn sich die Person registriert, erhält sie eine eindeutige URL, mit der sie das Ereignis aufruft.

   >[!TIP]
   >
   >Um Ihre Bestätigungs-E-Mail mit dieser eindeutigen URL zu füllen, verwenden Sie das folgende Token in Ihrer E-Mail: `{{member.webinar url}}`. Wenn die Bestätigungs-URL gesendet wird, wird dieses Token automatisch in die eindeutige Bestätigungs-URL der Person aufgelöst.
   >
   >Setzen Sie Ihre Bestätigungs-E-Mail auf **Betrieb** sicherzustellen, dass Personen, die sich registrieren und abgemeldet werden können, weiterhin ihre Bestätigungsinformationen erhalten.

* **Registrierungskennwort** - (Optional) Derzeit nicht unterstützt, wenn die Marketo-WebEx-Integration verwendet wird.
* **Validierungsregeln** - Derzeit nicht unterstützt durch die Marketo-WebEx-Integration. Sie können jedoch Smart-Kampagnen in Marketo verwenden, um Genehmigungen zu steuern.

![](assets/image2015-5-28-14-3a4-3a41.png)

### Moderatoren und Panelisten {#presenters-panelists}

Die in diesem Abschnitt konfigurierten Informationen werden nicht an Marketo übergeben.

### E-Mail-Nachrichten {#email-messages}

Sie verwenden Marketo, um E-Mails an Ihre Registrierungspflichtigen, Bestätigungs-E-Mails usw. zu senden. In diesem Abschnitt müssen Sie nichts konfigurieren. Deaktivieren Sie die E-Mail-Nachrichtenoptionen in WebEx.

![](assets/image2015-5-28-14-3a9-3a14.png)

>[!NOTE]
>
>Die Marketo-WebEx-Integration kann das Senden von Bestätigungs-E-Mails von WebEx nicht unterstützen. Die Bestätigung muss über Marketo erfolgen. Nachdem Sie das Ereignis geplant haben, kopieren Sie die Ereignisinformationen in die Marketo-Bestätigungs-E-Mail und stellen Sie die E-Mail auf **Betrieb**.

Jetzt sind wir bereit, in Marketo zu springen!

1. Wählen Sie das von Ihnen erstellte Ereignis aus. Öffnen Sie die **Ereignisaktionen** Dropdown-Liste. Auswählen **Ereigniseinstellungen.**

   ![](assets/image2015-5-14-16-3a7-3a31.png)

   >[!NOTE]
   >
   >Der Kanaltyp des ausgewählten Ereignisses muss **Webinar**.

1. under **Veranstaltungspartner** auswählen **WebEx**.

   ![](assets/image2015-1-30-13-3a58-3a2.png)

1. under **Anmelden**, wählen Sie Ihre WebEx-Anmeldung.

   ![](assets/image2015-5-18-12-3a2-3a26.png)

1. under **Ereignis** wählen Sie das neu erstellte WebEx-Ereignis aus. Wählen Sie dann eine optionale Sicherungsseite aus und klicken Sie auf **Speichern**.

   ![](assets/image2015-5-14-16-3a15-3a55.png)

1. Wählen Sie eine optionale Sicherungsseite für Ihr WebEx-Ereignis aus. Wählen Sie aus der Dropdown-Liste der genehmigten Marketo-Landingpages aus oder geben Sie die URL einer Nicht-Marketo-Landingpage ein.

   >[!TIP]
   >
   >Legen Sie eine Sicherungsseite fest, um ein Mitglied auf eine bestimmte Seite weiterzuleiten, wenn es vor der Startzeit des Ereignisses auf seine benutzerdefinierte Ereignis-URL klickt.

   >[!NOTE]
   >
   >Die von Marketo gesendeten Felder sind: Vorname, Nachname, E-Mail-Adresse.

   ![](assets/webex.png)

   >[!CAUTION]
   >
   >Vermeiden Sie den Versand von Bestätigungs-E-Mails durch verschachtelte E-Mail-Programme. Verwenden Sie stattdessen die Smart-Kampagne des Ereignisprogramms, wie oben dargestellt.

   >[!TIP]
   >
   >Es kann bis zu 48 Stunden dauern, bis die Daten in Marketo angezeigt werden. Wenn Sie nach so langer Wartezeit immer noch nichts sehen, wählen Sie **Von Webinar-Anbieter aktualisieren** über das Menü &quot;Ereignisaktionen&quot;im **Zusammenfassung** Registerkarte Ihres Ereignisses.

Süß! Ihr WebEx-Ereignis wird jetzt mit Ihrem Marketo-Ereignis synchronisiert.  Personen, die sich für Ihr Webinar anmelden, werden über den Schritt Programmstatus ändern zu Ihrem Webinar-Anbieter gepusht, wenn für Neuen Status &quot;Registriert&quot;festgelegt ist. Kein anderer Status wird die Person überstürzen. Stellen Sie außerdem sicher, dass Sie Schritt 1 zum Ändern des Programmstatus und Schritt 2 zum Senden eines E-Mail-Flusses durchführen.

## Anzeigen des Zeitplans  {#viewing-the-schedule}

Klicken Sie in der Programmplanungsansicht auf den Kalendereintrag für Ihr Ereignis. Sie können den Zeitplan auf der rechten Seite des Bildschirms sehen!

![](assets/image2015-5-14-16-3a21-3a41.png)

>[!NOTE]
>
>Um Ihren Ereigniszeitplan zu ändern, müssen Sie das Webinar auf WebEx bearbeiten.
