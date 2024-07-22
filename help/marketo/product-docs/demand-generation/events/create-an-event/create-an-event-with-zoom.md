---
unique-page-id: 17728023
description: Erstellen eines Ereignisses mit Zoom - Marketo Docs - Produktdokumentation
title: Erstellen eines Ereignisses mit Zoom
exl-id: 6a2aec58-902c-4e40-ab59-9cc33ec83cea
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# Erstellen eines Ereignisses mit Zoom {#create-an-event-with-zoom}

>[!PREREQUISITES]
>
>* [Zoom als LaunchPoint-Dienst hinzufügen](/help/marketo/product-docs/administration/additional-integrations/add-zoom-as-a-launchpoint-service.md)
>* [Neues Ereignisprogramm erstellen](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)
>* Legen Sie die entsprechenden [Fluss-Aktionen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md) fest, um die Interaktion zu verfolgen.

Erstellen Sie zunächst Ihr Webinar im Zoom. Bestimmte Einstellungen bei der Erstellung Ihres Zooms werden von Marketo verwendet, andere nur beim Zoomen.

Nachdem Sie ein Marketo-Ereignis erstellt und ein Zoom-Webinar damit verknüpft haben, können die Systeme Registrierungs- und Anwesenheitsinformationen freigeben. Hilfe zum Erstellen eines Webinars finden Sie unter [Erste Schritte mit Zoom-Webinaren](https://support.zoom.us/hc/en-us/articles/200917029-Getting-Started-With-Webinar).

Geben Sie die folgenden Informationen für Ihr Webinar ein, das über den Adapter nach Marketo gezogen wird. Wenn Sie Änderungen an diesen Informationen vornehmen, müssen Sie unter &quot;Ereignisaktionen&quot;auf den Link &quot;Von Webinar-Anbieter aktualisieren&quot;klicken, damit Marketo die Änderungen sieht.

**Titel und Beschreibung**

* **Webinarname** - Geben Sie den Namen für das Webinar ein. Dieser Name ist in Marketo sichtbar.

* **Beschreibung** (optional) - Geben Sie die Beschreibung für das Webinar ein. Die Beschreibung wird in Marketo angezeigt.

**Datum und Uhrzeit**

* **Startdatum** - Geben Sie Ihr Startdatum ein. Dies ist in Marketo sichtbar.

* **Startzeit** - Geben Sie Ihre Startzeit ein. Dies ist in Marketo sichtbar.

* **Dauer** - Geben Sie die Dauer ein. Die Start- und Endzeit sind in Marketo sichtbar.

* **Zeitzone** - Wählen Sie die gewünschte Zeitzone aus. Dies ist in Marketo sichtbar.

* **Wiederkehrender Webinar** - Lassen Sie die Markierung deaktiviert.

* **Registrierung** - Aktivieren Sie dieses Kontrollkästchen, um die Registrierung erforderlich zu machen. Sie verwenden ein Marketo-Formular/eine Landingpage, um Registrierungsinformationen zu erfassen, die in den Zoom gepusht werden.

>[!NOTE]
>
>Marketo unterstützt derzeit keine wiederkehrenden Webinare. Sie müssen für jedes Marketo Event- und Zoom-Webinar eine einzelne Sitzung einrichten.

![](assets/overview2.png)

>[!TIP]
>
>Es gibt zusätzliche Felder, die Sie im Zoom konfigurieren werden, die sich NICHT auf die Integration auswirken. Weitere Informationen zu diesen Feldern finden Sie im [Zoom Webinar Help Center](https://support.zoom.us/hc/en-us/sections/200324965-Video-Webinar) .

Jetzt springen wir in Marketo!

1. Wählen Sie ein Ereignis aus. Klicken Sie auf **Ereignisaktionen** und wählen Sie **Ereigniseinstellungen** aus.

   ![](assets/image2015-5-14-14-3a53-3a10-1.png)

   >[!NOTE]
   >
   >Der Kanaltyp des ausgewählten Ereignisses muss **webinar** sein.

1. Wählen Sie **Zoom** aus der Liste **Ereignis** **Partner** aus.

   ![](assets/eventsettings1.png)

1. Wählen Sie das Zoom-Konto aus, mit dem Sie Ihr Ereignis verknüpfen möchten.

   ![](assets/selectaccount.png)

1. Wählen Sie das Webinar aus.

   ![](assets/selectevent.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/eventsettingssave.png)

   Ausgezeichnet! Jetzt wird das Ereignis durch Zoom synchronisiert und geplant.

   >[!NOTE]
   >
   >Die von Marketo gesendeten Felder sind: Vorname, Nachname, E-Mail-Adresse.

   >[!TIP]
   >
   >Um Ihre Bestätigungs-E-Mail mit dieser eindeutigen URL zu füllen, verwenden Sie das folgende Token in Ihrer E-Mail: `{{member.webinar url}}`. Wenn die Bestätigungs-URL gesendet wird, wird dieses Token automatisch in die eindeutige Bestätigungs-URL der Person aufgelöst.
   >
   >Setzen Sie Ihre Bestätigungs-E-Mail auf &quot;**Operativ**&quot;, um sicherzustellen, dass Personen, die sich registrieren und abmelden können, weiterhin ihre Bestätigungsinformationen erhalten.

   Personen, die sich für Ihr Webinar anmelden, werden über den Flow-Schritt &quot;**Programmstatus ändern**&quot;an Ihren Webinar-Provider gepusht, wenn der neue Status auf &quot;Registriert&quot;gesetzt ist. Kein anderer Status wird die Person überstürzen. Stellen Sie außerdem sicher, dass Sie den Fluss &quot;**Programmstatus ändern**&quot; Schritt 1 und den Fluss &quot;**E-Mail senden**&quot; Schritt 2 durchlaufen.

   ![](assets/goto-webinar-1.png)

   >[!CAUTION]
   >
   >Vermeiden Sie den Versand von Bestätigungs-E-Mails durch verschachtelte E-Mail-Programme. Verwenden Sie stattdessen die Smart-Kampagne des Ereignisprogramms, wie oben dargestellt.

   >[!TIP]
   >
   >Die Anzeige der Daten in Marketo kann bis zu 48 Stunden dauern. Wenn Sie nach einer Wartezeit immer noch nichts sehen, wählen Sie auf der Registerkarte **Zusammenfassung** Ihres Ereignisses im Menü &quot;Ereignisaktionen&quot;die Option **Von Webinar-Anbieter aktualisieren**.
