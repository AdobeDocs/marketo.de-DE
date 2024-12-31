---
unique-page-id: 2949874
description: Erstellen eines Ereignisses mit GoToWebinar - Marketo-Dokumentation
title: Erstellen eines Ereignisses mit GoToWebinar
exl-id: c0f0a202-e416-4523-b7d6-dbcfafc536cd
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Erstellen eines Ereignisses mit GoToWebinar {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [GoToWebinar als LaunchPoint-Service hinzufügen](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [Erstellen eines neuen Veranstaltungsprogramms](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Legen Sie die entsprechenden [Fluss-Aktionen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) fest, um die Interaktion zu verfolgen

Erstellen Sie zunächst Ihr Webinar in GoToWebinar. Bestimmte Einstellungen bei der Erstellung Ihres GoToWebinars werden von Marketo verwendet, andere werden nur von GoToWebinar verwendet.

Nachdem Sie eine Marketo-Veranstaltung erstellt und das GoToWebinar damit verknüpft haben, können die Systeme Informationen zur Registrierung und Teilnahme austauschen.

Nachstehend finden Sie eine Liste der von Marketo verwendeten Einstellungen.

## Titel und Beschreibung {#title-and-description}

**Name des Webinars** - Geben Sie den Namen für das Webinar ein. Dieser Name wird in Marketo angezeigt.

**Beschreibung** (optional) - Geben Sie eine Beschreibung für das Webinar ein. Die Beschreibung wird in Marketo angezeigt.

![](assets/image2015-5-28-15-3a1-3a36.png)

## Datum und Uhrzeit {#date-time}

Geben Sie die folgenden Informationen für Ihr Webinar ein. Dieses wird dann über den Adapter in Marketo übernommen. Wenn Sie Änderungen an diesen Informationen vornehmen möchten, müssen Sie auf den Link &quot;**Vom Webinar-Anbieter aktualisieren** unter **Ereignisaktionen** klicken, damit die Änderungen in Marketo angezeigt werden.

**Startdatum** - Geben Sie Ihr Startdatum ein. Dieser wird in Marketo angezeigt.

**Startzeit** - Geben Sie Ihre Startzeit ein. Dieser wird in Marketo angezeigt.

**Endzeit** - Geben Sie Ihre Endzeit ein. Dieser wird in Marketo angezeigt.

**Zeitzone** - Wählen Sie die entsprechende Zeitzone aus. Er wird in Marketo angezeigt.

**Typ -** auf &quot;**Sitzung“**.

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>Marketo unterstützt derzeit keine wiederkehrenden Webinare. Sie müssen für jedes Marketo-Ereignis und für jedes GoToWebinar eine einzige Sitzung einrichten.

>[!TIP]
>
>Wenn Sie weitere Hilfe zu GoToWebinar benötigen, besuchen Sie bitte deren [Hilfe-Site](https://support.logmeininc.com/gotowebinar).

Lassen Sie uns jetzt zu Marketo springen!

1. Ereignis auswählen. Klicken Sie auf **Ereignisaktionen** und wählen Sie **Ereigniseinstellungen**.

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >Der Kanaltyp des ausgewählten Ereignisses muss „Webinar **sein**.

1. Wählen Sie **GoToWebinar** aus der Liste **Veranstaltungspartner** aus.

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. Wählen Sie das Konto aus.

   ![](assets/rtaimage-2.png)

1. Webinar auswählen.

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. Ausgezeichnet! Jetzt wird das Ereignis synchronisiert und vom **GoToWebinar** geplant.

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   >
   >Die von Marketo gesendeten Felder sind: Vorname, Nachname, E-Mail-Adresse. Diese Felder sind erforderlich und dürfen nicht leer sein.

   >[!TIP]
   >
   >Um Ihre Bestätigungs-E-Mail mit dieser eindeutigen URL zu füllen, verwenden Sie das folgende Token in Ihrer E-Mail: `{{member.webinar url}}`. Wenn die Bestätigungs-URL gesendet wird, wird dieses Token automatisch zur eindeutigen Bestätigungs-URL der Person aufgelöst.
   >
   >Legen Sie Ihre Bestätigungs-E **Mail auf** Betriebsbereit“ fest, um sicherzustellen, dass Personen, die sich registrieren und möglicherweise abgemeldet werden, weiterhin ihre Bestätigungsinformationen erhalten.

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   >
   >Vermeiden Sie verschachtelte E-Mail-Programme, um Ihre Bestätigungs-E-Mails zu senden. Verwenden Sie stattdessen die intelligente Kampagne des Ereignisprogramms , wie oben gezeigt.

   >[!TIP]
   >
   >Es kann bis zu 48 Stunden dauern, bis die Daten in Marketo angezeigt werden. Wenn Sie nach so langer Wartezeit immer noch nichts sehen, wählen Sie **Vom Webinar-Anbieter aktualisieren** aus dem Menü Ereignisaktionen auf der Registerkarte **Zusammenfassung** Ihres Ereignisses aus.

Personen, die sich für Ihr Webinar anmelden, werden über den Schritt „Programmstatus ändern“ an Ihren Webinar-Anbieter weitergeleitet, wenn der neue Status auf „Registriert“ gesetzt ist. Kein anderer Status überträgt die Person. Stellen Sie außerdem sicher, dass Sie den Schritt Programmstatus ändern #1 und den Schritt E-Mail-Fluss senden #2.

## Zeitplan anzeigen  {#viewing-the-schedule}

Klicken Sie in der Programmplanungsansicht auf den Kalendereintrag für Ihr Ereignis. Der Zeitplan wird auf der rechten Seite des Bildschirms angezeigt.

>[!NOTE]
>
>Um Ihren Veranstaltungskalender zu ändern, müssen Sie das Webinar auf GoToWebinar bearbeiten.

![](assets/image2015-5-14-15-3a3-3a13.png)
