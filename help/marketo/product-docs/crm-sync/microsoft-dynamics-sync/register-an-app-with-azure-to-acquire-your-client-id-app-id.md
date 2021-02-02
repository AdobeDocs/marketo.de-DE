---
unique-page-id: 12983390
description: Registrieren Sie eine App mit Azurblase, um Ihre Client-ID/App-ID zu erwerben - Marketing Docs - Produktdokumentation
title: Registrieren Sie eine App mit Azurblase, um Ihre Client-ID/App-ID zu erhalten.
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---


# Registrieren Sie eine App mit Azurblase, um Ihre Client-ID/App-ID zu erlangen. {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azurblauer Active Directory erweitert Ihre lokalen Verzeichnisse in die Cloud und bietet Unterstützung für MS Dynamics 365 CRM mit lokale ADFS-Authentifizierung.

## Registrieren einer neuen App {#registering-a-new-app}

1. [Melden Sie sich ](http://manage.windowsazure.com/) beim Microsoft Azurblase Management Portal mit einem Konto mit Administratorberechtigungen an. Sie können auch über das Office 365 Admin Center auf das Microsoft Azurblaus-Portal zugreifen, indem Sie das Element **Admin** im linken Navigationsbereich erweitern und **Azurblaue Anzeige** auswählen.

   >[!CAUTION]
   >
   >Sie müssen ein Konto im selben Office 365-Abonnement verwenden, mit dem Sie die App registrieren möchten.

   >[!NOTE]
   >
   >Wenn Sie kein blaues Konto haben, können Sie [für ein Konto ](https://azure.microsoft.com/en-us/free/) registrieren. Weitere Informationen erhalten Sie in der Microsoft-Dokumentation oder bei Ihrem Microsoft-Kundenbetreuer. Nachdem Sie ein Azurblauer Konto erstellt haben, können Sie eine oder mehrere Apps mit dem unten beschriebenen Verfahren registrieren.
   >
   >
   >Wenn Sie über ein blaues Konto verfügen, aber Ihr Office 365-Abonnement mit Microsoft Dynamics 365 nicht in Ihrem Azurblauen Abonnement verfügbar ist, befolgen Sie [diese Anweisungen](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription), um die beiden Konten zuzuordnen.

1. Klicken Sie im linken Navigationsbereich auf **Blaues Active Directory**.

   ![](assets/two.png)

1. Klicken Sie unter Verwalten auf **App-Registrierungen**.

   ![](assets/three.png)

1. Klicken Sie oben auf der Seite auf **Neue Registrierung**.

   ![](assets/four.png)

1. Geben Sie einen Namen für Ihre App ein, wählen Sie den gewünschten Kontotyp und geben Sie eine Umleitungs-URL ein. Klicken Sie anschließend unten auf der Seite auf **Register**.

   ![](assets/five.png)

1. Sie sollten Ihre App jetzt auf der Registerkarte **App-Registrierungen** sehen.

   ![](assets/six.png)

## Konfigurieren von App-Berechtigungen {#configuring-app-permissions}

1. Klicken Sie auf der Registerkarte **App-Registrierungen** in Ihrem Active Directory auf die App, für die Sie Berechtigungen konfigurieren möchten.

   ![](assets/seven.png)

1. Klicken Sie unter Verwalten auf **API-Berechtigungen**.

   ![](assets/eight.png)

1. Klicken Sie auf die Schaltfläche **Hinzufügen eine Berechtigung**.

   ![](assets/nine.png)

1. Wählen Sie **Dynamics CRM**.

   ![](assets/ten.png)

1. Markieren Sie das Feld **Zugriff auf den allgemeinen Datendienst als Organisationsbenutzer****s** und klicken Sie dann auf **Hinzufügen Berechtigungen.**

   ![](assets/eleven.png)

1. Warten Sie nach dem erfolgreichen Hinzufügen der Berechtigungen mindestens 10 Sekunden.

   ![](assets/twelve.png)

1. Klicken Sie auf die Schaltfläche **Administratorgenehmigung gewähren**.

   ![](assets/thirteen.png)

1. Klicken Sie zur Bestätigung auf **Ja**.

   ![](assets/fourteen.png)

   Und du bist fertig!

   ![](assets/fifteen.png)

