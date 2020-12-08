---
unique-page-id: 12983390
description: Registrieren Sie eine App mit Azurblase, um Ihre Client-ID/App-ID zu erwerben - Marketing Docs - Produktdokumentation
title: Registrieren Sie eine App mit Azurblase, um Ihre Client-ID/App-ID zu erhalten.
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---


# Registrieren Sie eine App mit Azurblase, um Ihre Client-ID/App-ID zu erhalten. {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azurblauer Active Directory erweitert Ihre lokalen Verzeichnisse in die Cloud und bietet Unterstützung für MS Dynamics 365 CRM mit lokale ADFS-Authentifizierung.

## Registrieren einer neuen App {#registering-a-new-app}

1. [Melden Sie sich](http://manage.windowsazure.com/) mit einem Konto mit Administratorberechtigungen beim Microsoft Azurblase-Verwaltungsportal an. Sie können auch über das Office 365 Admin Center auf das Microsoft Azurblaus-Portal zugreifen, indem Sie das **Admin** -Element im linken Navigationsbereich erweitern und **Azurblauer Anzeige** auswählen.

   >[!CAUTION]
   >
   >Sie müssen ein Konto im selben Office 365-Abonnement verwenden, mit dem Sie die App registrieren möchten.

   >[!NOTE]
   >
   >Wenn Sie kein blaues Konto haben, können Sie sich für ein Konto [registrieren](https://azure.microsoft.com/en-us/free/) . Weitere Informationen erhalten Sie in der Microsoft-Dokumentation oder bei Ihrem Microsoft-Kundenbetreuer. Nachdem Sie ein Azurblauer Konto erstellt haben, können Sie eine oder mehrere Apps mit dem unten beschriebenen Verfahren registrieren.
   >
   >
   >Wenn Sie ein blaues Konto haben, aber Ihr Office 365-Abonnement mit Microsoft Dynamics 365 ist nicht in Ihrem Abonnement verfügbar, folgen Sie [diesen Anweisungen](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription) , um die beiden Konten zu verbinden.

1. Klicken Sie im linken Navigationsbereich auf **Azurblauer Active Directory** .

   ![](assets/two.png)

1. Klicken Sie unter Verwalten auf **App-Registrierungen**.

   ![](assets/three.png)

1. Klicken Sie auf **Neue Registrierung **oben auf der Seite.

   ![](assets/four.png)

1. Geben Sie einen Namen für Ihre App ein, wählen Sie den gewünschten Kontotyp und geben Sie eine Umleitungs-URL ein. Klicken Sie dann unten auf der Seite auf **Registrieren** .

   ![](assets/five.png)

1. Die App sollte jetzt auf der Registerkarte &quot; **App-Registrierungen** &quot;angezeigt werden.

   ![](assets/six.png)

## App-Berechtigungen konfigurieren {#configuring-app-permissions}

1. Klicken Sie im Active Directory auf der Registerkarte &quot; **App-Registrierungen** &quot;auf die App, für die Sie Berechtigungen konfigurieren möchten.

   ![](assets/seven.png)

1. Klicken Sie unter Verwalten auf **API-Berechtigungen**.

   ![](assets/eight.png)

1. Klicken Sie auf die Schaltfläche **Hinzufügen Berechtigung** .

   ![](assets/nine.png)

1. Wählen Sie **Dynamics CRM**.

   ![](assets/ten.png)

1. Markieren Sie das Feld **Zugriff auf allgemeinen Datendienst als Organisationsbenutzer***s** und klicken Sie dann auf **Hinzufügen Berechtigungen.**

   ![](assets/eleven.png)

1. Warten Sie nach dem erfolgreichen Hinzufügen der Berechtigungen mindestens 10 Sekunden.

   ![](assets/twelve.png)

1. Klicken Sie auf die Schaltfläche **Genehmigung** des Administrators.

   ![](assets/thirteen.png)

1. Klicken Sie zur Bestätigung auf **Ja** .

   ![](assets/fourteen.png)

   Und du bist fertig!

   ![](assets/fifteen.png)

