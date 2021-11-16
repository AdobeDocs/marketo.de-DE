---
unique-page-id: 7504893
description: Hinzufügen von Google AdWords als Startpunktdienst mit einem Manager-Konto - Marketo Docs - Produktdokumentation
title: Hinzufügen von Google AdWords als Startpunktdienst mit einem Manager-Konto
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
source-git-commit: ab8eb044b89c925accc3b6a4ac4def53e3927321
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 2%

---

# Hinzufügen von Google AdWords als Startpunktdienst mit einem Manager-Konto {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Verknüpfen Sie Ihr Google AdWords-Konto mit Marketo, um Offline-Konversionsdaten automatisch von Marketo in Google AdWords hochzuladen. Anschließend können Sie in der AdWords-Benutzeroberfläche einfach sehen, welche Klicks zu qualifizierten Leads, Chancen und neuen Kunden (oder welchen Umsatzstufen Sie verfolgen möchten) geführt haben, nachdem Sie  [Benutzerdefinierte Spalten hinzufügen](https://support.google.com/adwords/answer/3073556) in AdWords. Diese Informationen werden nicht in der Benutzeroberfläche von Marketo angezeigt.

Wenn Sie über mehrere Google Adwords -Konten verfügen, können Sie eine [Google AdWords Manager-Konto](https://www.google.com/adwords/manager-accounts/) (ehemals &quot;My Client Center&quot;), um sie in Marketo zu integrieren.

Weitere Informationen [Google-Funktion zum Offline-Konversionsimport](https://support.google.com/adwords/answer/2998031?hl=en).

>[!AVAILABILITY]
>
>Nicht alle Kunden haben diese Funktion erworben. Weitere Informationen erhalten Sie von Ihrem Customer Success Manager.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!NOTE]
>
>Sie können auch eine [eigenständiges Google AdWords-Konto als Startpunktdienst](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md).

1. Navigieren Sie zu **Admin** Abschnitt.

   ![](assets/login-admin-1.png)

1. Auswählen **LaunchPoint**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Auswählen **Neu** und **Neuer Dienst**.

   ![](assets/image2015-2-23-14-3a54-3a50.png)

1. Geben Sie einen Anzeigenamen ein und wählen Sie **Google AdWords**.

   ![](assets/new-service-google-1.png)

1. Auswählen **Marketo autorisieren**.

   >[!NOTE]
   >
   >Melden Sie sich bei Ihrem persönlichen Gmail-Konto ab und aktivieren Sie Pop-ups.

   ![](assets/image2015-2-26-20-3a54-3a1.png)

1. Wählen Sie Ihr Konto aus, das mit **Google AdWords**.

   ![](assets/image2015-2-23-15-3a31-3a16.png)

1. Auswählen **Accept**.

   ![](assets/image2015-2-23-16-3a32-3a45.png)

1. Status wird als **Erfolg**. Auswählen **Nächste**.

   ![](assets/image2015-2-26-20-3a55-3a21.png)

1. Hochladen Ihrer Offline-Konversionen von Marketo in Google AdWords **Wöchentlich** oder **Täglich**.

   ![](assets/image2015-3-27-14-3a7-3a45.png)

1. Attributkonvertierung in **Erster Klick** oder **Letzter Klick**.

   | Typ | Definition |
   |---|---|
   | Erster Klick | Offline-Konversionen werden den ersten AdWords zugeordnet, auf die eine Person in den letzten 90 Tagen geklickt hat. |
   | Letzter Klick | Offline-Konversionen werden den letzten AdWords zugeordnet, auf die eine Person geklickt hat. |

   ![](assets/image2015-3-27-14-3a10-3a46.png)

   >[!NOTE]
   >
   >[Automatisches Tagging](https://support.google.com/adwords/answer/1752125?hl=en) muss ausgewählt sein, damit diese Funktion funktioniert. Sie muss in AdWords aktiviert werden.

1. Klicken **Nächste**.

   ![](assets/image2015-3-27-14-3a11-3a31.png)

1. Deaktivieren Sie die Konten, die Sie nicht aktualisieren möchten. Klicken Sie auf **Erstellen**.

   ![](assets/image2015-3-27-14-3a12-3a51.png)

   Im folgenden Artikel erfahren Sie, wie Sie Offline-Konversionen von AdWords in Ihrem Umsatzmodell zuordnen.

   >[!MORELIKETHIS]
   >
   >[Festlegen von Google AdWords-Konversionen im Umsatzmodell mit einem Manager-Konto](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md)
