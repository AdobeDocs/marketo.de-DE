---
unique-page-id: 11376159
description: Bevor Sie Push-Benachrichtigungen und In-App-Nachrichten erstellen - Marketing Docs - Produktdokumentation
title: Bevor Sie Push-Benachrichtigungen und In-App-Nachrichten erstellen
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---


# Bevor Sie Push-Benachrichtigungen und In-App-Nachrichten erstellen {#before-you-create-push-notifications-and-in-app-messages}

Das Erstellen von Push-Benachrichtigungen und In-App-Nachrichten ist nicht schwer, Sie müssen jedoch alles bereit haben, bevor Sie Beginn ausführen können. Der Marketing Admin- und der Mobile App-Entwickler sollten die folgenden Schritte ausführen, um die erforderlichen Integrationen vorzubereiten.

1. Zuerst fügt der Marketing-Administrator [eine mobile App](add-a-mobile-app.md) hinzu
1. Der Marketing-Administrator, dann [sendet ein Codefragment an den Entwickler](send-sdk-code-to-a-developer.md)
1. Der Entwickler lädt das SDK herunter und enthält Snippet und andere Methoden für [Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) oder [iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/)
1. In-App-Nachrichten werden standardmäßig ausgelöst, wenn die App geöffnet wird. Wenn Sie Meldungen für andere Ereignis, z. B. wenn eine bestimmte Seite angezeigt oder eine bestimmte Schaltfläche gedrückt wird, Trigger erhalten möchten, muss der Entwickler dem  benutzerdefinierte Ereignis hinzufügen (siehe [Benutzerspezifische Ereignis für In-App-Nachrichten](#CustomEvents) unten).
1. Der Entwickler [generiert den Server-API-Schlüssel und die Projektnummer für Android](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) oder [die Zertifizierung und das Kennwort für iOS](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) und sendet ihn an den Marketing-Administrator
1. Der Marketing-Administrator konfiguriert den Zugriff auf Push-Benachrichtigungen mit dem Server-API-Schlüssel (Android)](configure-mobile-app-android-push-access.md) oder [mit dem Zertifikat (iOS)](configure-mobile-app-ios-push-access.md)[

>[!TIP]
>
>Ein Marketing-Administrator kann einfach prüfen, ob Ihre Push-Konfiguration überprüft wurde. Gehen Sie einfach [hier](verify-push-configuration.md).

## Benutzerdefinierte Ereignis für In-App-Nachrichten {#custom-events-for-in-app-messages}

Bei In-App-Nachrichten ist der Trigger für die Anzeige standardmäßig auf **App öffnen** eingestellt. Wenn Sie benutzerspezifische Ereignis verwenden möchten, um die Anzeige von In-App-Nachrichten Trigger (z. B. **Klicks Hinzufügen zum Warenkorb**, **Einstellungsseite für Ansichten**), erstellen Sie eine Liste der gewünschten Ereignis und geben Sie sie an Ihren Entwickler für mobile Apps weiter. Der Entwickler fügt dann die benutzerdefinierten Ereignis dem Code hinzu. Nachdem sie genehmigt wurden, werden sie beim Einrichten Ihrer Audience als Trigger angezeigt. **Vorsicht**: Der Prozess der benutzerdefinierten Ereignis-Kodierung kann einige Zeit in Anspruch nehmen.

Nachdem Sie alle Vorbereitungen für In-App-Nachrichten und Push-Benachrichtigungen abgeschlossen haben, ist es an der Zeit, loszulegen!

>[!MORELIKETHIS]
>
>* [Erstellen einer In-App-Nachricht](https://docs.marketo.com/display/docs/create+an+in-app+message)
   >
   >
* [Push-Benachrichtigung erstellen](../../../product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

>



