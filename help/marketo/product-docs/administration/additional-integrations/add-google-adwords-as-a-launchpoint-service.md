---
unique-page-id: 6095008
description: hinzufügen Google AdWords als LaunchPoint-Dienst - Marketing Docs - Produktdokumentation
title: hinzufügen von Google AdWords als LaunchPoint-Dienst
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---


# hinzufügen von Google AdWords als LaunchPoint-Dienst {#add-google-adwords-as-a-launchpoint-service}

Verknüpfen Sie Ihr Google AdWords-Konto mit Marketo, um automatisch Offline-Konversionsdaten von Marketing zu Google AdWords hochzuladen. In der Benutzeroberfläche von AdWords können Sie dann einfach sehen, welche Klicks zu qualifizierten Interessenten, Chancen und neuen Kunden (oder welchen Umsatzstufen Sie verfolgen möchten) führten, nachdem Sie [benutzerdefinierte Spalten](https://support.google.com/adwords/answer/3073556) in AdWords hinzugefügt haben. Diese Informationen werden nicht in der Benutzeroberfläche von Marketing angezeigt.

Erfahren Sie mehr über die Google Offline-Konversions-Importfunktion[.](https://support.google.com/adwords/answer/2998031?hl=en)

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

>[!NOTE]
>
>Sie können auch einen [Google AdWords als Launchpoint-Dienst mit einem Manager-Konto](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md) integrieren.

1. Gehen Sie zum Abschnitt **Admin**.

   ![](assets/login-admin.png)

1. Wählen Sie **LaunchPoint**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Wählen Sie **Neu** und **Neuer Dienst**.

   ![](assets/image2015-2-23-14-3a54-3a50.png)

1. Geben Sie einen Anzeigenamen ein und wählen Sie **Google AdWords**.

   ![](assets/new-service-google.png)

1. Wählen Sie **Marketo autorisieren**.

   >[!NOTE]
   >
   >Achten Sie darauf, sich von Ihrem persönlichen Gmail-Konto abzumelden und Pop-ups zu aktivieren.

   ![](assets/image2015-2-26-20-3a54-3a1.png)

1. Wählen Sie Ihr mit Google AdWords verknüpftes Konto aus.

   ![](assets/image2015-2-23-15-3a31-3a16.png)

1. Wählen Sie **Accept**.

   ![](assets/image2015-2-23-16-3a32-3a45.png)

1. Der Status wird als **Erfolg** angezeigt. Wählen Sie **Weiter**.

   ![](assets/image2015-2-26-20-3a55-3a21.png)

1. Laden Sie Ihre Offline-Konvertierungen von Marketo zu Google AdWords **Wöchentlich** oder **Täglich** hoch.

   ![](assets/image2015-2-23-16-3a53-3a4.png)

1. Attributkonvertierung auf **Erster Klick** oder **Letzter Klick**.

   | Typ | Definition |
   |---|---|
   | Erster Klick | Offline-Konversionen werden den ersten AdWords zugeordnet, auf die eine Person in den letzten 90 Tagen geklickt hat |
   | Letzter Klick | Offline-Konversionen werden den letzten AdWords-Anzeigen zugeordnet, auf die eine Person geklickt hat |

   >[!NOTE]
   >
   >Die Verwendung eines konsistenten Zuordnungsmodells in Marketing und AdWords bietet die genauesten Daten.

   ![](assets/image2015-2-23-16-3a57-3a49.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/image2015-2-23-17-3a50-3a9.png)

   >[!NOTE]
   >
   >[Damit diese Funktion funktioniert, muss die automatische ](https://support.google.com/adwords/answer/1752125?hl=en) Taggingoption aktiviert sein. Die Deaktivierung muss innerhalb von AdWords erfolgen.

Großartig! Sehen Sie sich nun den entsprechenden Artikel unten an, um zu erfahren, wie Sie AdWords Offline-Konversionen in Ihrem Umsatzmodell zuordnen.

>[!MORELIKETHIS]
>
>[Google AdWords-Konversionen im Umsatzmodell festlegen](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model.md)
