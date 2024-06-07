---
unique-page-id: 11376159
description: Vor der Erstellung von Push-Benachrichtigungen und In-App-Nachrichten - Marketo-Dokumente - Produktdokumentation
title: Vor der Erstellung von Push-Benachrichtigungen und In-App-Nachrichten
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
feature: Mobile Marketing
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---

# Vor der Erstellung von Push-Benachrichtigungen und In-App-Nachrichten {#before-you-create-push-notifications-and-in-app-messages}

Die Erstellung von Push-Benachrichtigungen und In-App-Nachrichten ist nicht schwierig, aber Sie müssen alles bereit haben, bevor Sie beginnen können. Der Marketo-Administrator und der Entwickler der mobilen App sollten die folgenden Schritte ausführen, um die erforderlichen Integrationen vorzubereiten.

1. Zuerst der Marketo-Administrator [fügt eine mobile App hinzu](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. Der Marketo Admin dann [sendet ein Codefragment an den Entwickler](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. Der Entwickler lädt das SDK herunter und enthält Snippet und andere Methoden für [Android](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android) oder [iOS](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-ios).

1. Standardmäßig werden In-App-Nachrichten beim Öffnen der App ausgelöst. Wenn Sie Meldungen für andere Ereignisse (z. B. wenn eine bestimmte Seite angezeigt oder eine bestimmte Schaltfläche gedrückt wird) Trigger haben möchten, muss der Entwickler benutzerdefinierte Ereignisse zum Code hinzufügen (siehe [Benutzerdefinierte Ereignisse für In-App-Nachrichten](#CustomEvents) unten).

1. Der Entwickler [generiert den Server-API-Schlüssel und die Projektnummer für Android.](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android) oder [Zertifizierung und Kennwort für iOS](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#install-marketo-sdk-on-ios) und sendet es an den Marketo-Administrator.

1. Der Marketo-Administrator konfiguriert den Push-Benachrichtigungszugriff [mit dem Server-API-Schlüssel (Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) oder [mit dem Zertifikat (iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>Ein Marketo-Administrator kann leicht überprüfen, ob Ihre Push-Konfiguration verifiziert ist. Nur gehen [here](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## Benutzerdefinierte Ereignisse für In-App-Nachrichten {#custom-events-for-in-app-messages}

Bei In-App-Nachrichten wird der Trigger der Anzeige auf **App öffnen** Standardmäßig. Wenn Sie benutzerspezifische Ereignisse verwenden möchten, um die Anzeige von In-App-Nachrichten Trigger (z. B. **Klicks zum Warenkorb hinzufügen**, **Seite &quot;Anzeigeeinstellungen&quot;**), erstellen Sie eine Liste der gewünschten Ereignisse und geben Sie sie an Ihren Mobile-App-Entwickler weiter. Der Entwickler fügt dann die benutzerdefinierten Ereignisse zum Code hinzu. Nachdem sie genehmigt wurden, erscheinen sie beim Einrichten Ihrer Audience als Trigger zur Anzeige. **Vorsicht**: Der Validierungsprozess für die Kodierung benutzerdefinierter Ereignisse kann einige Zeit in Anspruch nehmen.

Nachdem Sie alle Ihre Vorbereitung für In-App-Nachrichten und Push-Benachrichtigungen abgeschlossen haben, ist es Zeit zu beginnen!

>[!MORELIKETHIS]
>
>* [In-App-Nachricht erstellen](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [Push-Benachrichtigung erstellen](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)
