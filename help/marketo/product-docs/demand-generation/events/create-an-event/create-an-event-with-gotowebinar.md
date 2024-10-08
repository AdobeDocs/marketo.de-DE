---
unique-page-id: 2949874
description: Erstellen eines Ereignisses mit GotoWebinar - Marketo Docs - Produktdokumentation
title: Erstellen eines Ereignisses mit GotoWebinar
exl-id: c0f0a202-e416-4523-b7d6-dbcfafc536cd
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Erstellen eines Ereignisses mit GotoWebinar {#create-an-event-with-gotowebinar}

>[!PREREQUISITES]
>
>* [GoToWebinar als LaunchPoint-Dienst hinzufügen](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [Neues Ereignisprogramm erstellen](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Legen Sie die entsprechenden [Fluss-Aktionen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) fest, um die Interaktion zu verfolgen.

Erstellen Sie zunächst Ihr Webinar im GoToWebinar. Bestimmte Einstellungen bei der Erstellung Ihres GoToWebinars werden von Marketo verwendet und einige werden nur von GoToWebinar verwendet.

Nachdem Sie ein Marketo-Ereignis erstellt und das GoToWebinar damit verknüpft haben, können die Systeme Registrierungs- und Anwesenheitsinformationen freigeben.

Nachstehend finden Sie eine Liste der von Marketo verwendeten Einstellungen.

## Titel und Beschreibung {#title-and-description}

**Webinarname** - Geben Sie den Namen für das Webinar ein. Dieser Name ist in Marketo sichtbar.

**Beschreibung** (optional) - Geben Sie die Beschreibung für das Webinar ein. Die Beschreibung wird in Marketo angezeigt.

![](assets/image2015-5-28-15-3a1-3a36.png)

## Datum &amp; Uhrzeit {#date-time}

Geben Sie die folgenden Informationen für Ihr Webinar ein, das über den Adapter nach Marketo gezogen wird. Wenn Sie Änderungen an diesen Informationen vornehmen, müssen Sie unter &quot;**Ereignisaktionen**&quot;auf den Link &quot;**Von Webinar-Anbieter aktualisieren**&quot;klicken, damit Marketo die Änderungen sieht.

**Startdatum** - Geben Sie Ihr Startdatum ein. Dies ist in Marketo sichtbar.

**Startzeit** - Geben Sie Ihre Startzeit ein. Dies ist in Marketo sichtbar.

**Endzeit** - Geben Sie Ihre Endzeit ein. Dies ist in Marketo sichtbar.

**Zeitzone** - Wählen Sie die gewünschte Zeitzone aus. Sie wird in Marketo angezeigt.

**Typ -** auf **Eine Sitzung** eingestellt ist.

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>Marketo unterstützt derzeit keine wiederkehrenden Webinare. Sie müssen für jedes Marketo-Ereignis und jedes GoToWebinar-Webinar eine einzelne Sitzung einrichten.

>[!TIP]
>
>Wenn Sie zusätzliche Hilfe zu GoToWebinar benötigen, besuchen Sie bitte deren [Hilfe-Site](https://support.logmeininc.com/gotowebinar).

Jetzt springen wir in Marketo!

1. Wählen Sie ein Ereignis aus. Klicken Sie auf **Ereignisaktionen** und wählen Sie **Ereigniseinstellungen** aus.

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >Der Kanaltyp des ausgewählten Ereignisses muss **webinar** sein.

1. Wählen Sie **GoToWebinar** aus der Liste **Partner des Ereignisses**.

   ![](assets/image2015-5-14-14-3a55-3a20.png)

1. Wählen Sie das Konto aus.

   ![](assets/rtaimage-2.png)

1. Wählen Sie das Webinar aus.

   ![](assets/image2015-5-14-14-3a57-3a31.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2015-5-14-14-3a58-3a54.png)

1. Ausgezeichnet! Jetzt wird das Ereignis von **GoToWebinar** synchronisiert und geplant.

   ![](assets/image2015-5-14-15-3a0-3a47.png)

   >[!NOTE]
   >
   >Die von Marketo gesendeten Felder sind: Vorname, Nachname, E-Mail-Adresse. Diese Felder sind erforderlich und dürfen nicht leer sein.

   >[!TIP]
   >
   >Um Ihre Bestätigungs-E-Mail mit dieser eindeutigen URL zu füllen, verwenden Sie das folgende Token in Ihrer E-Mail: `{{member.webinar url}}`. Wenn die Bestätigungs-URL gesendet wird, wird dieses Token automatisch in die eindeutige Bestätigungs-URL der Person aufgelöst.
   >
   >Setzen Sie Ihre Bestätigungs-E-Mail auf &quot;**Operativ**&quot;, um sicherzustellen, dass Personen, die sich registrieren und abmelden können, weiterhin ihre Bestätigungsinformationen erhalten.

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   >
   >Vermeiden Sie den Versand von Bestätigungs-E-Mails durch verschachtelte E-Mail-Programme. Verwenden Sie stattdessen die Smart-Kampagne des Ereignisprogramms, wie oben dargestellt.

   >[!TIP]
   >
   >Die Anzeige der Daten in Marketo kann bis zu 48 Stunden dauern. Wenn Sie nach einer Wartezeit immer noch nichts sehen, wählen Sie auf der Registerkarte **Zusammenfassung** Ihres Ereignisses im Menü &quot;Ereignisaktionen&quot;die Option **Von Webinar-Anbieter aktualisieren**.

Personen, die sich für Ihr Webinar anmelden, werden über den Schritt Programmstatus ändern zu Ihrem Webinar-Anbieter gepusht, wenn für Neuen Status &quot;Registriert&quot;festgelegt ist. Kein anderer Status wird die Person überstürzen. Stellen Sie außerdem sicher, dass Sie Schritt 1 zum Ändern des Programmstatus und Schritt 2 zum Senden eines E-Mail-Flusses durchführen.

## Anzeigen des Zeitplans  {#viewing-the-schedule}

Klicken Sie in der Programmplanungsansicht auf den Kalendereintrag für Ihr Ereignis. Sie können den Zeitplan auf der rechten Seite des Bildschirms sehen.

>[!NOTE]
>
>Um Ihren Veranstaltungszeitplan zu ändern, müssen Sie das Webinar im GoToWebinar bearbeiten.

![](assets/image2015-5-14-15-3a3-3a13.png)
