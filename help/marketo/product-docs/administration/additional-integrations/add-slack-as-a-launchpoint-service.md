---
unique-page-id: 12983619
description: hinzufügen Slack als LaunchPoint-Dienst - Marketing Docs - Produktdokumentation
title: hinzufügen Slack als LaunchPoint-Dienst
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---


# hinzufügen Slack als LaunchPoint-Dienst {#add-slack-as-a-launchpoint-service}

Die Slack-Integration umfasst zwei Benachrichtigungstypen:

* **Systembenachrichtigungen**: Erhalten Sie Benachrichtigungen über wichtige Ereignis in Ihrer Marketo-Instanz, z. B. Warnungen über den Status der aktuellen Kampagne und Probleme, die sofortige Aufmerksamkeit erfordern (CRM-Fehler und API-Beschränkungen).
* **Interessante Momente**: Wenn ein Marketo Insight von einer bekannten Person aus einem Kundenkonto ausgelöst wurde, können Interessenteninhaber per Slack benachrichtigt werden. Benachrichtigungen enthalten Interessenteninformationen sowie Details zum Kundenkonto.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!PREREQUISITES]
>
>Wenn Sie noch keine Systembenachrichtigungen für Slack aktiviert haben, wenden Sie sich bitte an [MarketingTo Support](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Gehen Sie zu **LaunchPoint** und klicken Sie dann unter **New** auf **New Service**.

   ![](assets/image2017-11-27-14-3a13-3a18.png)

1. Geben Sie einen Anzeigenamen für Ihre Slack-Integration ein. Wählen Sie in der Dropdownliste **Dienst** **Slack**. Klicken Sie auf **Erstellen**.

   ![](assets/image2017-11-27-15-3a54-3a11.png)

1. Klicken Sie auf **Autorisieren**. Dadurch wird der Slack in einer neuen Registerkarte geöffnet, auf der Sie die Autorisierung abschließen und Marketo die Berechtigung zum Abrufen von Informationen aus dem Slack erteilen.

   ![](assets/image2017-11-27-14-3a16-3a6.png)

1. Geben Sie auf der Registerkarte &quot;neuer Slack&quot;die URL Ihres Arbeitsbereichs ein und klicken Sie auf **Weiter**.

   ![](assets/image2017-11-27-15-3a1-3a29.png)

1. Geben Sie Ihre Anmeldeinformationen für den Slack ein und klicken Sie auf **Anmelden**.

   ![](assets/image2017-11-27-15-3a1-3a3.png)

1. Wählen Sie in der Dropdownliste **An** posten den Kanal aus, in dem Benachrichtigungen von Marketing veröffentlicht werden sollen. Überprüfen Sie die angeforderten Berechtigungen und klicken Sie dann auf **Autorisieren**.

   ![](assets/image2018-1-9-13-3a21-3a50.png)

1. Darunter sollte der Bestätigungsbildschirm angezeigt werden. Die Registerkarte wird automatisch geschlossen.

   ![](assets/image2017-11-27-15-3a51-3a57.png)

1. Aktualisieren Sie die Registerkarte &quot;Markieren&quot;und vergewissern Sie sich, dass Slack jetzt als aktiver Dienst in LaunchPoint aufgeführt wird.

   ![](assets/image2017-11-27-15-3a55-3a37.png)

   Benachrichtigungen beginnen nun mit der Veröffentlichung an dem Kanal, den Sie in Schritt 6 ausgewählt haben. Sie werden ungefähr so aussehen:

   ![](assets/samplenotification.png)
