---
unique-page-id: 11376159
description: Bevor Sie Push-Benachrichtigungen und In-App-Nachrichten erstellen - Marketo-Dokumente - Produktdokumentation
title: Vor dem Erstellen von Push-Benachrichtigungen und In-App-Nachrichten
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
feature: Mobile Marketing
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---

# Vor dem Erstellen von Push-Benachrichtigungen und In-App-Nachrichten {#before-you-create-push-notifications-and-in-app-messages}

Das Erstellen von Push-Benachrichtigungen und In-App-Nachrichten ist nicht schwierig, aber Sie müssen alles vorbereitet haben, bevor Sie beginnen können. Der Marketo-Administrator und der Entwickler der mobilen App sollten die folgenden Schritte ausführen, um die erforderlichen Integrationen vorzubereiten.

1. Zunächst fügt der Marketo-Administrator [eine Mobile App hinzu](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. Der Marketo-Administrator [sendet dann ein Codefragment an den Entwickler](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. Der Entwickler lädt die SDK herunter und schließt Snippet und andere Methoden für [Android](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android) oder [iOS](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-ios) ein.

1. Standardmäßig werden In-App-Nachrichten beim Öffnen der App ausgelöst. Wenn Sie Nachrichten für andere Trigger erstellen möchten, z. B. wenn eine bestimmte Seite aufgerufen oder eine bestimmte Schaltfläche gedrückt wird, muss der Entwickler dem Code benutzerdefinierte Ereignisse hinzufügen (siehe [Benutzerspezifische Ereignisse für In-App-Nachrichten](#CustomEvents) unten).

1. Android Der Entwickler [generiert den Server-API-Schlüssel und die Projektnummer für ](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android) oder [die Zertifizierung und das Kennwort für iOS](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/mobile/installation#install-marketo-sdk-on-ios) und sendet sie an den Marketo-Administrator.

1. Der Marketo-Administrator konfiguriert den Zugriff auf Push[Benachrichtigungen (mit dem Server-API-Schlüssel (Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) oder [mit dem Zertifikat (iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>Für einen Marketo-Administrator ist es einfach, zu überprüfen, ob Ihre Push-Konfiguration überprüft wurde. Geh einfach [hier](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## Benutzerdefinierte Ereignisse für In-App-Nachrichten {#custom-events-for-in-app-messages}

Beim In-App-Messaging ist der Display-Trigger standardmäßig auf **App**&quot; eingestellt. Wenn Sie benutzerdefinierte Ereignisse zum Trigger der Anzeige von In-App-Nachrichten verwenden möchten (z. B. **Klicks zum Warenkorb hinzufügen**, **Ansichtseinstellungsseite**), erstellen Sie eine Liste der gewünschten Ereignisse und geben Sie sie an Ihren Mobile-App-Entwickler weiter. Der Entwickler fügt dann die benutzerdefinierten Ereignisse zum Code hinzu. Nachdem sie genehmigt wurden, werden sie beim Einrichten Ihrer Zielgruppe als Display-Trigger angezeigt. **Achtung**: Der Genehmigungsprozess für die benutzerdefinierte Ereigniscodierung kann einige Zeit in Anspruch nehmen.

Nachdem Sie alle Vorbereitungen für In-App-Nachrichten und Push-Benachrichtigungen abgeschlossen haben, ist es an der Zeit, loszulegen!

>[!MORELIKETHIS]
>
>* [Erstellen einer In-App-Nachricht](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [Push-Benachrichtigung erstellen](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)
