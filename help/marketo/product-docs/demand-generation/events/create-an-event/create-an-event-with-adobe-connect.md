---
unique-page-id: 2949865
description: Erstellen eines Ereignisses mit Adobe Connect - Marketo Docs - Produktdokumentation
title: Erstellen eines Ereignisses mit Adobe Connect
exl-id: 196b1640-9cfd-4485-9bc4-e907d3ac1f16
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Erstellen eines Ereignisses mit Adobe Connect {#create-an-event-with-adobe-connect}

Durch die Synchronisierung mit Adobe Connect können Sie Ihre Webinarregistrierung und -teilnahme innerhalb von Marketo verwalten. Dadurch wird sichergestellt, dass Interaktionen nicht rückverfolgt werden.

>[!PREREQUISITES]
>
>* [Verknüpfen von Adobe Connect und Marketo](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
>* [Neues Ereignisprogramm erstellen](/help/marketo/product-docs/demand-generation/events/understanding-events/create-a-new-event-program.md)

Stellen Sie zunächst sicher, dass Sie Ihr Meeting oder Seminar in Adobe Connect erstellt haben. Wenn Sie Hilfe benötigen, sehen Sie sich das [Adobe Connect-Benutzerhandbuch](https://help.adobe.com/en_US/connect/9.0/using/index.html) an.

Die in Adobe Connect erstellten Meetings und Seminare müssen in dem Ordner erstellt werden, den Sie bei der Eingabe Ihrer Anmeldedaten in Marketo angegeben haben. Nachdem Sie Ihr Meeting oder Seminar erstellt haben, notieren Sie sich alle relevanten Logistikinformationen (wie die Telefonnummer), die Sie in Ihrer Bestätigungs-E-Mail und in der ICS-Datei verwenden können.

>[!CAUTION]
>
>Stellen Sie als Ereignishost sicher, dass Sie über den an die Teilnehmer gesendeten Link in der App beitreten und **nicht** beitreten.

>[!NOTE]
>
>Adobe Connect On-site wird derzeit nicht unterstützt.

1. Wählen Sie auf der Startseite eines neuen Ereignisses **Ereignisaktionen** und dann **Ereigniseinstellungen** aus.

   ![](assets/image2015-1-30-15-3a34-3a28.png)

   >[!NOTE]
   >
   >Wenn in der Dropdown-Liste die Option **Ereigniseinstellungen** nicht angezeigt wird, stellen Sie sicher, dass im Kanal des Ereignisses unter &quot;Gilt für&quot;die Option **Ereignis mit Webinar** ausgewählt ist.

1. Wählen Sie unter **Ereignispartner** die Option **Adobe Connect** aus.

   ![](assets/event-settings-adobe-connect.png)

1. Wählen Sie Ihre **Anmelde**-ID und dann Ihr **Ereignis** aus.

   ![](assets/event-settings-select-event-adobe-connect.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/event-settings-overview.png)

   Gut! Ihr Adobe Connect-Ereignis wird jetzt mit Ihrem Marketo-Ereignis synchronisiert.

   >[!NOTE]
   >
   >Die von Marketo gesendeten Felder sind: Vorname, Nachname, E-Mail-Adresse.

   >[!TIP]
   >
   >Verwenden Sie dieses Token, um die eindeutige URL der Person in eine E-Mail einzufügen: `{{member.webinar url}}`. Wenn die E-Mail gesendet wird, löst dieses Token automatisch die eindeutige Bestätigungs-URL der Person aus Adobe Connect auf.
   >
   >Setzen Sie Ihre Bestätigungs-E-Mail auf &quot;**Operativ**&quot;, um sicherzustellen, dass Personen, die sich registrieren und abmelden können, weiterhin ihre Bestätigungsinformationen erhalten.

   Personen, die sich für Ihr Webinar anmelden, werden über den Schritt Programmstatus ändern zu Ihrem Webinar-Anbieter gepusht, wenn für Neuen Status &quot;Registriert&quot;festgelegt ist. Kein anderer Status wird die Person überstürzen. Stellen Sie außerdem sicher, dass Sie Schritt 1 zum Ändern des Programmstatus und Schritt 2 zum Senden eines E-Mail-Flusses durchführen.

   ![](assets/adobe.png)

   >[!CAUTION]
   >
   >Vermeiden Sie den Versand von Bestätigungs-E-Mails durch verschachtelte E-Mail-Programme. Verwenden Sie stattdessen die Smart-Kampagne des Ereignisprogramms, wie oben dargestellt.

   >[!TIP]
   >
   >Die Anzeige der Daten in Marketo kann bis zu 48 Stunden dauern. Wenn Sie nach einer Wartezeit immer noch nichts sehen, wählen Sie auf der Registerkarte &quot;Zusammenfassung&quot;Ihres Ereignisses im Menü &quot;Ereignisaktionen&quot;die Option **Von Webinar-Anbieter aktualisieren**.

   >[!MORELIKETHIS]
   >
   >* [Hinzufügen von Adobe Connect als LaunchPoint-Dienst](/help/marketo/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.md)
   >* [Bearbeiten eines Ereigniskanals](/help/marketo/product-docs/demand-generation/events/understanding-events/edit-an-event-channel.md)
