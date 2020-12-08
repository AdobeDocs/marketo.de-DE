---
unique-page-id: 11376159
description: Bevor Sie Push-Benachrichtigungen und In-App-Nachrichten erstellen - Marketing Docs - Produktdokumentation
title: Bevor Sie Push-Benachrichtigungen und In-App-Nachrichten erstellen
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# Bevor Sie Push-Benachrichtigungen und In-App-Nachrichten erstellen {#before-you-create-push-notifications-and-in-app-messages}

Das Erstellen von Push-Benachrichtigungen und In-App-Nachrichten ist nicht schwer, Sie müssen jedoch alles bereit haben, bevor Sie Beginn ausführen können. Der Marketing Admin- und der Mobile App-Entwickler sollten die folgenden Schritte ausführen, um die erforderlichen Integrationen vorzubereiten.

1. Zuerst [fügt der Marketing Admin eine mobile App hinzu](add-a-mobile-app.md)
1. Der Marketing-Administrator [sendet dann ein Codefragment an den Entwickler](send-sdk-code-to-a-developer.md)
1. Der Entwickler lädt das SDK herunter und enthält Snippet und andere Methoden für [Android](http://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) oder [iOS](http://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/)
1. In-App-Nachrichten werden standardmäßig ausgelöst, wenn die App geöffnet wird. Wenn Sie Meldungen für andere Ereignis auslösen möchten, z. B. wenn eine bestimmte Seite angezeigt oder eine bestimmte Schaltfläche gedrückt wird, muss der Entwickler dem Code benutzerdefinierte Ereignis hinzufügen (siehe [Benutzerspezifische Ereignis für In-App-Nachrichten](#CustomEvents) unten)
1. Der Entwickler [generiert den Server-API-Schlüssel und die Projektnummer für Android](http://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) oder [die Zertifizierung und das Kennwort für iOS](http://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) und sendet ihn an den Marketing Admin
1. Der Marketing-Administrator konfiguriert den Zugriff auf Push-Benachrichtigungen [mit dem Server-API-Schlüssel (Android)](configure-mobile-app-android-push-access.md) oder [mit dem Zertifikat (iOS)](configure-mobile-app-ios-push-access.md)

>[!TIP]
>
>Ein Marketing-Administrator kann einfach prüfen, ob Ihre Push-Konfiguration überprüft wurde. Geh einfach [hierher](verify-push-configuration.md).

## Benutzerdefinierte Ereignis für In-App-Nachrichten {#custom-events-for-in-app-messages}

Bei In-App-Nachrichten ist der Anzeigeauslöser standardmäßig auf &quot; **App öffnen** &quot;eingestellt. Wenn Sie benutzerdefinierte Ereignis verwenden möchten, um die Anzeige von In-App-Nachrichten auszulösen (z. B. **Klicks Hinzufügen Warenkorb**, Einstellungsseite **für** Ansichten), erstellen Sie eine Liste der gewünschten Ereignis und geben Sie sie an Ihren Entwickler für mobile Apps weiter. Der Entwickler fügt dann die benutzerdefinierten Ereignis dem Code hinzu. Nachdem sie genehmigt wurden, werden sie beim Einrichten der Audience als Anzeigeauslöser angezeigt. **Vorsicht**: Der Prozess der benutzerdefinierten Ereignis-Kodierung kann einige Zeit in Anspruch nehmen.

Nachdem Sie alle Vorbereitungen für In-App-Nachrichten und Push-Benachrichtigungen abgeschlossen haben, ist es an der Zeit, loszulegen!

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Erstellen einer In-App-Nachricht](http://docs.marketo.com/display/docs/create+an+in-app+message)
   >
   >
* [Push-Benachrichtigung erstellen](../../../product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

>



