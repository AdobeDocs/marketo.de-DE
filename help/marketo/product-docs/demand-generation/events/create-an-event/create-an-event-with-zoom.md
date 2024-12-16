---
unique-page-id: 17728023
description: Erstellen eines Ereignisses mit Zoom - Marketo-Dokumente - Produktdokumentation
title: Erstellen eines Ereignisses mit Zoom
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
feature: Events
source-git-commit: c10ecc0ccad28f2e480343acefe10f5eca2ae578
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# Erstellen eines Ereignisses mit Zoom {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [Zoom als LaunchPoint-Service hinzufügen](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [Erstellen eines neuen Veranstaltungsprogramms](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Legen Sie die entsprechenden [Fluss-Aktionen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) fest, um die Interaktion zu verfolgen

Erstellen Sie zunächst Ihr Webinar im Zoom-Modus. Bestimmte Einstellungen bei der Erstellung Ihres Zooms werden von Marketo verwendet, andere werden nur von Zoom verwendet.

Nachdem Sie eine Marketo-Veranstaltung erstellt und ein Zoom-Webinar damit verknüpft haben, können die Systeme Informationen zur Registrierung und Teilnahme austauschen. Hilfe beim Erstellen eines Webinars finden Sie unter [Erste Schritte mit Zoom-Webinaren](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar).

Geben Sie die folgenden Informationen für Ihr Webinar ein. Dieses wird dann über den Adapter in Marketo übernommen. Wenn Sie Änderungen an diesen Informationen vornehmen möchten, müssen Sie auf den Link „Vom Webinar-Anbieter aktualisieren“ unter „Ereignisaktionen“ klicken, damit die Änderungen in Marketo angezeigt werden.

**Titel und Beschreibung**

* **Name des Webinars** - Geben Sie den Namen für das Webinar ein. Dieser Name wird in Marketo angezeigt.

* **Beschreibung** (optional) - Geben Sie eine Beschreibung für das Webinar ein. Die Beschreibung wird in Marketo angezeigt.

**Datum und Uhrzeit**

* **Startdatum** - Geben Sie Ihr Startdatum ein. Dieser wird in Marketo angezeigt.

* **Startzeit** - Geben Sie Ihre Startzeit ein. Dieser wird in Marketo angezeigt.

* **Dauer** - Geben Sie die Dauer ein. Die Start- und Endzeit werden in Marketo angezeigt.

* **Zeitzone** - Wählen Sie die entsprechende Zeitzone aus. Dieser wird in Marketo angezeigt.

* **Wiederkehrendes Webinar** - Deaktivieren Sie diese Option.

* **Registrierung** - Aktivieren Sie dieses Kontrollkästchen, um eine Registrierung erforderlich zu machen. Sie verwenden ein Marketo-Formular/eine Landingpage, um Registrierungsinformationen zu erfassen, die zum Zoomen übertragen werden.

>[!NOTE]
>
>Marketo unterstützt derzeit keine wiederkehrenden Webinare. Sie müssen für jedes Marketo-Ereignis und jedes Zoom-Webinar eine einzige Sitzung einrichten.

![](assets/overview2.png)

>[!TIP]
>
>Es gibt zusätzliche Felder, die Sie in Zoom konfigurieren werden und die sich NICHT auf die Integration auswirken. Weitere Informationen zu diesen Feldern [ Sie im Hilfezentrum ](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar)Zoom-Webinar“.

Lassen Sie uns jetzt zu Marketo springen!

1. Ereignis auswählen. Klicken Sie auf **Ereignisaktionen** und wählen Sie **Ereigniseinstellungen**.

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >Der Kanaltyp des ausgewählten Ereignisses muss „Webinar **sein**.

1. Wählen Sie **Zoom** aus der **Ereignis** **Partner** Liste aus.

   ![](assets/eventsettings1.png)

1. Wählen Sie das Zoom-Konto aus, mit dem Sie Ihr Ereignis verknüpfen möchten.

   ![](assets/selectaccount.png)

1. Webinar auswählen.

   ![](assets/selectevent.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/eventsettingssave.png)

   Ausgezeichnet! Jetzt wird das Ereignis synchronisiert und von Zoom geplant.

   >[!NOTE]
   >
   >Die von Marketo gesendeten Felder sind: Vorname, Nachname, E-Mail-Adresse.

   >[!TIP]
   >
   >Um Ihre Bestätigungs-E-Mail mit dieser eindeutigen URL zu füllen, verwenden Sie das folgende Token in Ihrer E-Mail: `{{member.webinar url}}`. Wenn die Bestätigungs-URL gesendet wird, wird dieses Token automatisch zur eindeutigen Bestätigungs-URL der Person aufgelöst.
   >
   >Legen Sie Ihre Bestätigungs-E **Mail auf** Betriebsbereit“ fest, um sicherzustellen, dass Personen, die sich registrieren und möglicherweise abgemeldet werden, weiterhin ihre Bestätigungsinformationen erhalten.

   Personen, die sich für Ihr Webinar anmelden, werden über den Flussschritt **Programmstatus ändern** an Ihren Webinar-Anbieter weitergeleitet, wenn der neue Status auf „Registriert“ gesetzt ist. Kein anderer Status überträgt die Person. Stellen Sie außerdem sicher, dass **Programmstatus ändern** Flussschritt #1 und **E-Mail senden** Flussschritt #2.

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >Vermeiden Sie verschachtelte E-Mail-Programme, um Ihre Bestätigungs-E-Mails zu senden. Verwenden Sie stattdessen die intelligente Kampagne des Ereignisprogramms , wie oben gezeigt.

   >[!TIP]
   >
   >Es kann bis zu 48 Stunden dauern, bis die Daten in Marketo angezeigt werden. Wenn Sie nach so langer Wartezeit immer noch nichts sehen, wählen Sie **Vom Webinar-Anbieter aktualisieren** aus dem Menü Ereignisaktionen auf der Registerkarte **Zusammenfassung** Ihres Ereignisses aus und klicken Sie dann auf das Aktualisierungssymbol unten rechts im Bildschirm.
