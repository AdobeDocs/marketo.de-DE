---
unique-page-id: 2949865
description: Erstellen Sie ein Ereignis mit Adobe Connect - Marketing Docs - Produktdokumentation
title: Ereignis mit Adobe Connect erstellen
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---


# Ereignis mit Adobe Connect {#create-an-event-with-adobe-connect} erstellen

Die Synchronisierung mit Adobe Connect ermöglicht es Ihnen, Ihre Webinarregistrierung und -teilnahme innerhalb von Marketo zu verwalten, wodurch sichergestellt wird, dass Interaktionen nicht rückverfolgt werden.

>[!PREREQUISITES]
>
>* [Adobe Connect und Marketo verknüpfen](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [Neues Ereignis-Programm erstellen](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)


Vergewissern Sie sich zunächst, dass Sie Ihr Meeting oder Seminar in Adobe Connect erstellt haben. Wenn Sie Hilfe benötigen, sehen Sie sich das [Adobe Connect Benutzerhandbuch](http://help.adobe.com/en_US/connect/9.0/using/index.html) an. Die Meetings und Seminare, die Sie in Adobe Connect erstellen, müssen in dem Ordner erstellt werden, den Sie bei der Eingabe Ihrer Anmeldedaten in Marketing angegeben haben. Nachdem Sie Ihr Meeting oder Seminar erstellt haben, notieren Sie sich alle relevanten Logistikinformationen (z. B. die Telefonnummer), die Sie in Ihrer Bestätigungs-E-Mail und in Ihrer ICS-Datei verwenden können.

>[!NOTE]
>
>Wir **unterstützen derzeit nicht** Adobe Connect On-Site.

1. Wählen Sie auf der Startseite eines neuen Ereignisses **Ereignis Actions** und dann **Ereignis Settings**.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >Wenn Sie in der Dropdownliste nicht **Ereignis-Einstellungen** sehen, stellen Sie sicher, dass im Kanal des Ereignisses **Ereignis mit Webinar** unter &quot;Gilt für&quot;ausgewählt ist.

1. Wählen Sie unter **Ereignis-Partner** **Adobe Connect**.

   ![](assets/event-settings-adobe-connect.png)

1. Wählen Sie Ihre **Login**-ID und wählen Sie Ihr **Ereignis**.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/event-settings-overview.png)

   Schön! Ihr Adobe Connect-Ereignis wird jetzt mit Ihrem Marketing-Ereignis synchronisiert.

   >[!NOTE]
   >
   >Die Felder, die von Marketo gesendet werden, sind: Vorname, Nachname, E-Mail-Adresse.

   >[!TIP]
   >
   >Verwenden Sie das folgende Token, um die eindeutige URL der Person in eine E-Mail einzufügen: `{{member.webinar url}}`. Wenn die E-Mail gesendet wird, löst dieses Token automatisch die eindeutige Bestätigungs-URL der Person aus Adobe Connect.
   >
   >Stellen Sie Ihre Bestätigungs-E-Mail auf **Operational** ein, um sicherzustellen, dass Personen, die sich registrieren und abgemeldet werden können, weiterhin ihre Bestätigungsinformationen erhalten.

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >Vermeiden Sie die Verwendung verschachtelter E-Mail-Programm zum Versenden Ihrer Bestätigungs-E-Mails. Verwenden Sie stattdessen die intelligente Kampagne des Ereignis Programms, wie oben gezeigt.

   >[!TIP]
   >
   >Es kann bis zu 48 Stunden dauern, bis die Daten in Marketo angezeigt werden. Wenn Sie nach einer Wartezeit immer noch nichts sehen, wählen Sie **Von Webinar-Provider aktualisieren** aus dem Menü &quot;Ereignis-Aktionen&quot;auf der Registerkarte &quot;Zusammenfassung&quot;Ihres Ereignisses.

   >[!MORELIKETHIS]
   >
   > * [hinzufügen Adobe Connect als LaunchPoint-Dienst](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   > * [Bearbeiten eines Ereignis-Kanals](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)


Personen, die sich für Ihr Webinar anmelden, werden über den Schritt zum Ändern des Status des Programms an Ihren Webinaranbieter weitergeleitet, wenn der neue Status auf &quot;Registriert&quot;eingestellt ist. Kein anderer Status wird die Person übertreiben. Stellen Sie außerdem sicher, dass Sie den Schritt zum Ändern des Status des Programms 1 und zum Senden der E-Mail-Zustellung Schritt 2 durchführen.
