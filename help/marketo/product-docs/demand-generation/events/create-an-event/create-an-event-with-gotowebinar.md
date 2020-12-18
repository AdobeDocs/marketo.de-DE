---
unique-page-id: 2949874
description: Erstellen Sie ein Ereignis mit GotoWebinar - Marketing Docs - Produktdokumentation
title: Ereignis mit GotoWebinar erstellen
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---


# Ereignis mit GotoWebinar {#create-an-event-with-gotowebinar} erstellen

>[!PREREQUISITES]
>
>* [hinzufügen GoToWebinar als LaunchPoint-Dienst](/help/marketo/product-docs/administration/additional-integrations/add-gotowebinar-as-a-launchpoint-service.md)
>* [Neues Ereignis-Programm erstellen](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Stellen Sie die entsprechenden [Flussaktionen](http://docs.marketo.com/display/DOCS/Flow+Actions)ein, um Interaktionen zu verfolgen.


Erstellen Sie zuerst Ihr Webinar im GoToWebinar. Bestimmte Einstellungen bei der Erstellung Ihres GoToWebinars werden von Marketo verwendet und einige werden nur von GoToWebinar verwendet.

Nachdem Sie ein Marketo-Ereignis erstellt und das GoToWebinar damit verknüpft haben, können die Systeme Registrierungs- und Anwesenheitsdaten gemeinsam nutzen. Hilfe zum Erstellen eines GoToWebinars finden Sie im [GoToWebinar-Benutzerhandbuch](http://docs.marketo.com/display/docs/assets/gotowebinar-user-guide.pdf).

Nachfolgend finden Sie eine Liste der Einstellungen, die von Marketo verwendet werden.

## Titel und Beschreibung {#title-and-description}

**Webinarname** : Geben Sie den Namen für das Webinar ein. Dieser Name wird in Marketo angezeigt.

**Beschreibung**  (optional): Geben Sie die Beschreibung für das Webinar ein. Die Beschreibung ist in Marketo sichtbar.

![](assets/image2015-5-28-15-3a1-3a36.png)

## Datum und Uhrzeit {#date-time}

`Enter the following information for your webinar and it will be pulled into Marketo via the`Adapter. Wenn Sie Änderungen an diesen Informationen vornehmen, müssen Sie unter **Ereignis-Aktionen** auf den Link &quot;**Von Webinar-Provider aktualisieren**&quot;klicken, damit Marketo die Änderungen sehen kann.

**Datum**  des Beginns - geben Sie das Datum Ihres Beginns ein. Dies wird in Marketo sichtbar sein.

**Beginn**  - geben Sie die Uhrzeit Ihres Beginns ein. Dies wird in Marketo sichtbar sein.

**Endzeit**  - Geben Sie Ihre Endzeit ein. Dies wird in Marketo sichtbar sein.

**Zeitzone** : Wählen Sie die gewünschte Zeitzone aus. Es wird in Marketo sichtbar sein.

**Geben Sie -** set to  **One Session** ein.

![](assets/image2015-5-28-15-3a7-3a1.png)

>[!NOTE]
>
>Marketo unterstützt derzeit keine wiederkehrenden Webinare. Sie müssen eine Sitzung zwischen jedem Marketing-Ereignis und jedem GoToWebinar-Webinar einrichten.

>[!TIP]
>
>Es gibt zusätzliche Felder, die Sie in GoToWebinar konfigurieren werden, die sich NICHT auf die Integration auswirken. Weitere Informationen zu diesen Feldern finden Sie im [GoToWebinar Benutzerhandbuch](http://docs.marketo.com/display/docs/assets/gotowebinar-user-guide.pdf), da sie in diesem Artikel nicht behandelt werden. Wenn Sie weitere Hilfe zum GoToWebinar benötigen, besuchen Sie bitte deren [Hilfe-Site](http://support.logmeininc.com/gotowebinar).

Springen wir jetzt nach Marketo!

1. Wählen Sie ein Ereignis aus. Klicken Sie auf **Ereignis Actions** und wählen Sie **Ereignis Settings**.

   ![](assets/image2015-5-14-14-3a53-3a10.png)

   >[!NOTE]
   >
   >Der Kanal des ausgewählten Ereignisses muss **webinar** lauten.

1. Wählen Sie **GoToWebinar** aus der Liste **Ereignis** **Partner**.

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
   >Die Felder, die von Marketo gesendet werden, sind: Vorname, Nachname, E-Mail-Adresse. Diese Felder sind erforderlich und dürfen nicht leer sein.

   >[!TIP]
   >
   >Um Ihre Bestätigungs-E-Mail mit dieser eindeutigen URL zu füllen, verwenden Sie das folgende Token in Ihrer E-Mail: `{{member.webinar url}}`. Wenn die Bestätigungs-URL gesendet wird, wird dieses Token automatisch zur eindeutigen Bestätigungs-URL der Person aufgelöst.
   >
   >Stellen Sie Ihre Bestätigungs-E-Mail auf **Operational** ein, um sicherzustellen, dass Personen, die sich registrieren und abgemeldet werden können, weiterhin ihre Bestätigungsinformationen erhalten.

   ![](assets/goto-webinar.png)

   >[!CAUTION]
   >
   >Vermeiden Sie die Verwendung verschachtelter E-Mail-Programm zum Versenden Ihrer Bestätigungs-E-Mails. Verwenden Sie stattdessen die intelligente Kampagne des Ereignis Programms, wie oben gezeigt.

   >[!TIP]
   >
   >Es kann bis zu 48 Stunden dauern, bis die Daten in Marketo angezeigt werden. Wenn Sie nach dem Warten immer noch nichts sehen, wählen Sie **Von Webinar-Provider aktualisieren** im Menü &quot;Ereignis-Aktionen&quot;auf der Registerkarte **Zusammenfassung** aus.

Personen, die sich für Ihr Webinar anmelden, werden über den Schritt zum Ändern des Status des Programms an Ihren Webinaranbieter weitergeleitet, wenn der neue Status auf &quot;Registriert&quot;eingestellt ist. Kein anderer Status wird die Person übertreiben. Stellen Sie außerdem sicher, dass Sie den Schritt zum Ändern des Status des Programms 1 und zum Senden der E-Mail-Zustellung Schritt 2 durchführen.

## Ansicht des Zeitplans {#viewing-the-schedule}

Klicken Sie in der Ansicht [Programmplanung](http://docs.marketo.com/display/docs/program+schedule+view) auf den Kalendereintrag für Ihr Ereignis. Sie können den Zeitplan auf der rechten Seite des Bildschirms sehen.

>[!NOTE]
>
>Um den Zeitplan für Ihr Ereignis zu ändern, müssen Sie das Webinar im GoToWebinar bearbeiten.

![](assets/image2015-5-14-15-3a3-3a13.png)
