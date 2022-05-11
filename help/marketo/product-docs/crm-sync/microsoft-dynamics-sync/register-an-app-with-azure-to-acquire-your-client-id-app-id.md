---
unique-page-id: 12983390
description: Registrieren Sie eine App bei Azure, um Ihre Client-ID/App-ID zu erhalten - Marketo Docs - Produktdokumentation
title: Registrieren Sie eine App bei Azure, um Ihre Client-ID/App-ID zu erhalten.
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
source-git-commit: 6f15abf1fed69431b3bbe249c908b0f90a56d391
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# Registrieren Sie eine App bei Azure, um Ihre Client-ID/App-ID zu erhalten. {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory erweitert Ihre lokalen Verzeichnisse in die Cloud und unterstützt MS Dynamics 365 CRM mit On-Premise-ADFS-Authentifizierung.

## Registrieren einer neuen App {#registering-a-new-app}

1. [Anmelden](https://login.microsoftonline.com/){target=&quot;_blank&quot;} für das Verwaltungsportal von Microsoft Azure mit einem Konto mit Administratorberechtigungen. Sie können auch über das Office 365 Admin Center auf das Microsoft Azure-Portal zugreifen, indem Sie die **Admin** Element im linken Navigationsbereich und wählen Sie **Azure AD**.

   >[!CAUTION]
   >
   >Sie müssen ein Konto im selben Office 365-Abonnement verwenden, mit dem Sie die App registrieren möchten.

   >[!NOTE]
   >
   >Wenn Sie kein Azure-Konto haben, können Sie [anmelden](https://azure.microsoft.com/en-us/free/){target=&quot;_blank&quot;} für eine. Weitere Informationen erhalten Sie in der Dokumentation zu Microsoft oder bei Ihrem Microsoft-Support-Mitarbeiter. Nachdem Sie ein Azure-Konto erstellt haben, können Sie eine oder mehrere Apps gemäß dem unten beschriebenen Verfahren registrieren.
   >
   >
   >Wenn Sie über ein Azure-Konto verfügen, Ihr Office 365-Abonnement mit Microsoft Dynamics 365 jedoch nicht in Ihrem Azure-Abonnement verfügbar ist, folgen Sie den Anweisungen. [diese Anweisungen](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target=&quot;_blank&quot;}, um die beiden Konten zuzuordnen.

1. Suchen und Klicken **Azure Active Directory** im linken Navigationsbereich.

   ![](assets/two.png)

1. Klicken Sie unter Verwalten auf **App-Registrierungen**.

   ![](assets/three.png)

1. Klicken **Neue Registrierung** oben auf der Seite.

   ![](assets/four.png)

1. Geben Sie einen Namen für Ihre App ein, wählen Sie den entsprechenden Kontotyp aus und geben Sie eine Umleitungs-URL ein. Klicken Sie anschließend auf **registrieren** unten auf der Seite.

   ![](assets/five.png)

1. Ihre App sollte jetzt im **App-Registrierungen** Registerkarte.

   ![](assets/six.png)

## Konfigurieren von App-Berechtigungen {#configuring-app-permissions}

1. Unter dem **App-Registrierungen** in Ihrem Active Directory auf die App klicken, für die Sie Berechtigungen konfigurieren möchten.

   ![](assets/seven.png)

1. Klicken Sie unter Verwalten auf **API-Genehmigungen**.

   ![](assets/eight.png)

1. Klicken Sie auf **Berechtigung hinzufügen** Schaltfläche.

   ![](assets/nine.png)

1. Auswählen **Dynamics CRM**.

   ![](assets/ten.png)

1. Überprüfen Sie die **Zugriff auf den allgemeinen Datendienst als Organisationsbenutzer***s** und klicken Sie auf **Berechtigungen hinzufügen.**

   ![](assets/eleven.png)

1. Warten Sie mindestens 10 Sekunden, nachdem die Berechtigungen erfolgreich hinzugefügt wurden.

   ![](assets/twelve.png)

1. Klicken Sie auf **Erteilen der Admin-Zustimmung** Schaltfläche.

   ![](assets/thirteen.png)

1. Klicken **Ja** zur Bestätigung.

   ![](assets/fourteen.png)

   Und du bist fertig!

   ![](assets/fifteen.png)
