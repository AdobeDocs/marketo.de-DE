---
unique-page-id: 14745982
description: hinzufügen Workplace By Facebook as a LaunchPoint Service - Marketo Docs - Produktdokumentation
title: hinzufügen Workplace by Facebook als LaunchPoint-Dienst
exl-id: afcc1eca-8927-4a25-af9b-c18cef24b0ae
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 1%

---

# hinzufügen Workplace By Facebook as a LaunchPoint Service {#add-workplace-by-facebook-as-a-launchpoint-service}

Die Integration in Workplace umfasst zwei Benachrichtigungstypen:

* **Systembenachrichtigungen**: Rufen Sie Benachrichtigungen zu wichtigen Ereignissen in Ihrer Marketo-Instanz ab, z. B. Warnungen zu aktuellen Statuswerten der Kampagne und Problemen, die sofortige Aufmerksamkeit erfordern (CRM-Fehler und API-Beschränkungen).
* **Interessante Momente**: Wenn ein Marketo Insight von einer bekannten Person aus einem Kundenkonto ausgelöst wurde, können Interessenteninhaber über Workplace benachrichtigt werden. Benachrichtigungen enthalten Interessenteninformationen sowie Details zum Kundenkonto.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!PREREQUISITES]
>
>Wenn Sie noch keine Workspace-Benachrichtigungen aktiviert haben, wenden Sie sich bitte an den [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Gehen Sie zu **LaunchPoint** und klicken Sie dann unter **New** auf **New Service**.

   ![](assets/image2017-11-27-14-3a13-3a18-1.png)

1. Geben Sie einen Anzeigenamen für Ihre Workplace-Integration ein. Wählen Sie in der Dropdownliste **Dienst** **Arbeitsplatz nach Facebook**. Klicken Sie auf **Erstellen**.

   ![](assets/newservice.png)

1. Um Systembenachrichtigungen und interessante Momente zu erhalten, lassen Sie die Optionen unverändert. Klicken Sie auf **Erstellen**.

   ![](assets/create.png)

1. Klicken Sie auf **Autorisieren**. Dadurch wird Workplace in einer neuen Registerkarte geöffnet, auf der Sie die Autorisierung abschließen und Marketo die Erlaubnis erteilen, Informationen von Workplace zu beziehen.

   ![](assets/authorize.png)

1. Geben Sie auf der neuen Registerkarte &quot;Arbeitsplatz&quot;Ihre geschäftliche E-Mail oder Ihren Arbeitsplatz-Benutzernamen ein und klicken Sie auf **Weiter**.

   ![](assets/workplacelogin.png)

1. Geben Sie Ihre Anmeldeinformationen für den Arbeitsplatz ein und klicken Sie auf **Anmelden**.

   ![](assets/workplacelogininfo.png)

1. Wählen Sie im Popup &quot;Arbeitsplatz&quot;eine Facebook-Gruppe aus, für die Benachrichtigungen von Marketo veröffentlicht werden sollen (z. B. Partnerintegrationen). Klicken Sie auf **Install**.

   ![](assets/installmarketo.png)

1. Die Bestätigungsmeldung wird unten angezeigt. Die Registerkarte wird automatisch geschlossen.

   ![](assets/success.png)

1. Aktualisieren Sie die Registerkarte &quot;Marketo&quot;und stellen Sie sicher, dass &quot;Workplace&quot;jetzt als aktiver Dienst in LaunchPoint aufgeführt wird.

   ![](assets/confirm.png)

   Benachrichtigungen beginnen nun mit der Veröffentlichung für die Facebook-Gruppe, die Sie in Schritt 7 ausgewählt haben. Sie werden ungefähr so aussehen:

   ![](assets/example.png)
