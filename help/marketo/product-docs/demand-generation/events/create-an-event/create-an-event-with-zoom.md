---
unique-page-id: 17728023
description: Erstellen eines Ereignisses mit Zoom - Marketing Docs - Produktdokumentation
title: Ereignis mit Zoom erstellen
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---


# Ereignis mit Zoom {#create-an-event-with-zoom} erstellen

>[!PREREQUISITES]
>
>* [hinzufügen Zoom als LaunchPoint-Dienst](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [Neues Ereignis-Programm erstellen](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Stellen Sie die entsprechenden [Flussaktionen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)ein, um Interaktionen zu verfolgen.


Erstellen Sie zuerst Ihr Webinar im Zoom. Bestimmte Einstellungen bei der Erstellung des Zooms werden von Marker verwendet, andere werden nur von Zoom verwendet.

Nachdem Sie ein Marketo-Ereignis erstellt und ein Zoom-Webinar mit ihm verknüpft haben, können die Systeme Registrierungs- und Anwesenheitsinformationen gemeinsam nutzen. Hilfe zum Erstellen eines Webinars finden Sie unter [Erste Schritte mit Zoom-Webinaren](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar).

Geben Sie die folgenden Informationen für Ihr Webinar ein und es wird über den Adapter nach Marketo gezogen. Wenn Sie Änderungen an diesen Informationen vornehmen, müssen Sie auf den Link &quot;Aktualisieren von Webinar-Provider&quot;unter &quot;Ereignis-Aktionen&quot;klicken, damit Marketo die Änderungen sehen kann.

**Titel und Beschreibung**

* **Webinarname**  - Geben Sie den Namen für das Webinar ein. Dieser Name wird in Marketo angezeigt.

* **Beschreibung**  (optional) - Geben Sie die Beschreibung für das Webinar ein. Die Beschreibung ist in Marketo sichtbar.

**Datum und Uhrzeit**

* **Datum**  des Beginns - Geben Sie das Datum Ihres Beginns ein. Dies wird in Marketo sichtbar sein.

* **Beginn**  - Geben Sie die Uhrzeit Ihres Beginns ein. Dies wird in Marketo sichtbar sein.

* **Dauer**  - Geben Sie die Dauer ein. Die Beginn- und Endzeit sind in Marketo sichtbar.

* **Zeitzone** : Wählen Sie die gewünschte Zeitzone aus. Dies wird in Marketo sichtbar sein.

* **Wiederkehrendes Webinar** - Nicht aktivieren.

* **Registrierung**  - Aktivieren Sie dieses Kontrollkästchen, um die Registrierung erforderlich zu machen. Sie können mit einem &quot;Markieren&quot;-Formular/einer &quot;Landingpage&quot;Registrierungsinformationen erfassen, die zum Zoomen weitergeleitet werden.

>[!NOTE]
>
>Marketo unterstützt derzeit keine wiederkehrenden Webinare. Sie müssen für jedes Marketing-Ereignis und jedes Zoom-Webinar eine Sitzung einrichten.

![](assets/overview2.png)

>[!TIP]
>
>Es gibt weitere Felder, die Sie im Zoom konfigurieren werden, die sich NICHT auf die Integration auswirken. Weitere Informationen zu diesen Feldern finden Sie im [Zoom-Webinar-Hilfe-Center](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar).

Springen wir jetzt nach Marketo!

1. Wählen Sie ein Ereignis aus. Klicken Sie auf **Ereignis Actions** und wählen Sie **Ereignis Settings**.

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >Der Kanal des ausgewählten Ereignisses muss **webinar** lauten.

1. Wählen Sie **Zoom** aus der Liste **Ereignis** **Partner**.

   ![](assets/eventsettings1.png)

1. Wählen Sie das Zoomkonto aus, mit dem Sie Ihr Ereignis verknüpfen möchten.

   ![](assets/selectaccount.png)

1. Wählen Sie das Webinar aus.

   ![](assets/selectevent.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/eventsettingssave.png)

   Ausgezeichnet! Jetzt wird das Ereignis durch Zoom synchronisiert und geplant.

   >[!NOTE]
   >
   >Die Felder, die von Marketo gesendet werden, sind: Vorname, Nachname, E-Mail-Adresse.

   >[!TIP]
   >
   >Um Ihre Bestätigungs-E-Mail mit dieser eindeutigen URL zu füllen, verwenden Sie das folgende Token in Ihrer E-Mail: `{{member.webinar url}}`. Wenn die Bestätigungs-URL gesendet wird, wird dieses Token automatisch zur eindeutigen Bestätigungs-URL der Person aufgelöst.
   >
   >Stellen Sie Ihre Bestätigungs-E-Mail auf **Operational** ein, um sicherzustellen, dass Personen, die sich registrieren und abgemeldet werden können, weiterhin ihre Bestätigungsinformationen erhalten.

   Personen, die sich für Ihr Webinar anmelden, werden über den Textfluss **Ändern des Programm-Status** an Ihren Webinar-Provider weitergeleitet, wenn der neue Status auf &quot;Registriert&quot;eingestellt ist. Kein anderer Status wird die Person übertreiben. Stellen Sie außerdem sicher, dass **Change Programm Status** den Flusstest #1 und **Send Email** den Flusstest #2 durchlaufen.

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >Vermeiden Sie die Verwendung verschachtelter E-Mail-Programm zum Versenden Ihrer Bestätigungs-E-Mails. Verwenden Sie stattdessen die intelligente Kampagne des Ereignis Programms, wie oben gezeigt.

   >[!TIP]
   >
   >Es kann bis zu 48 Stunden dauern, bis die Daten in Marketo angezeigt werden. Wenn Sie nach dem Warten immer noch nichts sehen, wählen Sie **Von Webinar-Provider aktualisieren** im Menü &quot;Ereignis-Aktionen&quot;auf der Registerkarte **Zusammenfassung** aus.
