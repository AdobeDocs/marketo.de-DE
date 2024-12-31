---
unique-page-id: 2949865
description: Erstellen eines Ereignisses mit Adobe Connect - Marketo-Dokumente - Produktdokumentation
title: Erstellen eines Ereignisses mit Adobe Connect
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Erstellen eines Ereignisses mit Adobe Connect {#create-an-event-with-adobe-connect}

Durch die Synchronisierung mit Adobe Connect können Sie Ihre Registrierung und Teilnahme an Webinaren in Marketo verwalten, sodass die Interaktion nicht unverfolgt bleibt.

>[!PREREQUISITES]
>
>* [Verknüpfen von Adobe Connect und Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [Erstellen eines neuen Veranstaltungsprogramms](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)

Stellen Sie zunächst sicher, dass Sie Ihr Meeting oder Seminar in Adobe Connect erstellt haben. Wenn Sie Hilfe benötigen, lesen Sie das [Adobe Connect-Benutzerhandbuch](https://help.adobe.com/en_US/connect/9.0/using/index.html).

Die Meetings und Seminare, die Sie in Adobe Connect erstellen, müssen in dem Ordner erstellt werden, den Sie beim Eingeben Ihrer Anmeldeinformationen in Marketo angegeben haben. Nachdem Sie Ihr Meeting oder Seminar erstellt haben, notieren Sie sich alle relevanten logistischen Informationen (z. B. die Telefonnummer), die Sie in Ihrer Bestätigungs-E-Mail und in Ihrer ICS-Datei verwenden können.

>[!CAUTION]
>
>Stellen Sie als Ereignis-Host sicher, dass Sie der -App aus beitreten und **nicht** über den Link, der an die Teilnehmer gesendet wird.

>[!NOTE]
>
>Adobe Connect On-Site wird derzeit nicht unterstützt.

1. Wählen Sie auf der Startseite eines neuen Ereignisses die Option **Ereignisaktionen** und dann **Ereigniseinstellungen**.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >Wenn in der Dropdown-Liste **Ereigniseinstellungen** nicht angezeigt wird, stellen Sie sicher, dass im Kanal des Ereignisses **Ereignis mit Webinar** unter „Gilt für“ ausgewählt ist.

1. Wählen **unter &quot;**&quot; die Option **Adobe Connect**.

   ![](assets/event-settings-adobe-connect.png)

1. Wählen Sie Ihre **Login** ID und dann Ihr **Ereignis** aus.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/event-settings-overview.png)

   Schön! Ihr Adobe Connect-Ereignis wird jetzt mit Ihrem Marketo-Ereignis synchronisiert.

   >[!NOTE]
   >
   >Die von Marketo gesendeten Felder sind: Vorname, Nachname, E-Mail-Adresse.

   >[!TIP]
   >
   >Um die eindeutige URL der Person in eine E-Mail einzufügen, verwenden Sie dieses Token: `{{member.webinar url}}`. Wenn die E-Mail gesendet wird, löst dieses Token automatisch die eindeutige Bestätigungs-URL der Person aus Adobe Connect auf.
   >
   >Legen Sie Ihre Bestätigungs-E **Mail auf** Betriebsbereit“ fest, um sicherzustellen, dass Personen, die sich registrieren und möglicherweise abgemeldet werden, weiterhin ihre Bestätigungsinformationen erhalten.

   Personen, die sich für Ihr Webinar anmelden, werden über den Schritt „Programmstatus ändern“ an Ihren Webinar-Anbieter weitergeleitet, wenn der neue Status auf „Registriert“ gesetzt ist. Kein anderer Status überträgt die Person. Stellen Sie außerdem sicher, dass Sie den Schritt Programmstatus ändern #1 und den Schritt E-Mail-Fluss senden #2.

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >Vermeiden Sie verschachtelte E-Mail-Programme, um Ihre Bestätigungs-E-Mails zu senden. Verwenden Sie stattdessen die intelligente Kampagne des Ereignisprogramms , wie oben gezeigt.

   >[!TIP]
   >
   >Es kann bis zu 48 Stunden dauern, bis die Daten in Marketo angezeigt werden. Wenn Sie nach so langer Wartezeit immer noch nichts sehen, wählen Sie **Vom Webinar-Anbieter aktualisieren** aus dem Menü Ereignisaktionen auf der Registerkarte Zusammenfassung Ihres Ereignisses aus.

   >[!MORELIKETHIS]
   >
   >* [Adobe Connect als LaunchPoint-Service hinzufügen](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [Bearbeiten eines Ereigniskanals](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)
