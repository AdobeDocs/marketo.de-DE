---
unique-page-id: 6095008
description: Hinzufügen von Google AdWords as a LaunchPoint Service - Marketo Docs - Produktdokumentation
title: Hinzufügen von Google AdWords als LaunchPoint-Dienst
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
source-git-commit: ab8eb044b89c925accc3b6a4ac4def53e3927321
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 2%

---

# Hinzufügen von Google AdWords als LaunchPoint-Dienst {#add-google-adwords-as-a-launchpoint-service}

Verknüpfen Sie Ihr Google AdWords-Konto mit Marketo, um Offline-Konversionsdaten automatisch von Marketo in Google AdWords hochzuladen. Anschließend können Sie in der AdWords-Benutzeroberfläche einfach sehen, welche Klicks zu qualifizierten Leads, Chancen und neuen Kunden (oder welchen Umsatzstufen Sie verfolgen möchten) geführt haben, nachdem Sie [Benutzerdefinierte Spalten hinzufügen](https://support.google.com/adwords/answer/3073556) in AdWords. Diese Informationen werden nicht in der Benutzeroberfläche von Marketo angezeigt.

Weitere Informationen [Google-Funktion zum Offline-Konversionsimport](https://support.google.com/adwords/answer/2998031?hl=en).

>[!AVAILABILITY]
>
>Nicht alle Kunden haben diese Funktion erworben. Weitere Informationen erhalten Sie von Ihrem Customer Success Manager.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!NOTE]
>
>Sie können auch eine [Google AdWords as a Launchpoint-Dienst mit einem Managerkonto](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md).

1. Navigieren Sie zu **Admin** Abschnitt.

   ![](assets/login-admin.png)

1. Auswählen **LaunchPoint**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Auswählen **Neu** und **Neuer Dienst**.

   ![](assets/image2015-2-23-14-3a54-3a50.png)

1. Geben Sie einen Anzeigenamen ein und wählen Sie **Google AdWords**.

   ![](assets/new-service-google.png)

1. Auswählen **Marketo autorisieren**.

   >[!NOTE]
   >
   >Melden Sie sich bei Ihrem persönlichen Gmail-Konto ab und aktivieren Sie Pop-ups.

   ![](assets/image2015-2-26-20-3a54-3a1.png)

1. Wählen Sie Ihr mit Google AdWords verknüpftes Konto aus.

   ![](assets/image2015-2-23-15-3a31-3a16.png)

1. Auswählen **Accept**.

   ![](assets/image2015-2-23-16-3a32-3a45.png)

1. Status wird als **Erfolg**. Auswählen **Nächste**.

   ![](assets/image2015-2-26-20-3a55-3a21.png)

1. Hochladen Ihrer Offline-Konversionen von Marketo in Google AdWords **Wöchentlich** oder **Täglich**.

   ![](assets/image2015-2-23-16-3a53-3a4.png)

1. Attributkonvertierung in **Erster Klick** oder **Letzter Klick**.

   | Typ | Definition |
   |---|---|
   | Erster Klick | Offline-Konversionen werden den ersten AdWords zugeordnet, auf die eine Person in den letzten 90 Tagen geklickt hat. |
   | Letzter Klick | Offline-Konversionen werden den letzten AdWords zugeordnet, auf die eine Person geklickt hat. |

   >[!NOTE]
   >
   >Die Verwendung eines konsistenten Attributionsmodells in Marketo und AdWords liefert die präzisesten Daten.

   ![](assets/image2015-2-23-16-3a57-3a49.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/image2015-2-23-17-3a50-3a9.png)

   >[!NOTE]
   >
   >[Automatisches Tagging](https://support.google.com/adwords/answer/1752125?hl=en) muss ausgewählt sein, damit diese Funktion funktioniert. Die Deaktivierung muss in AdWords erfolgen.

Sehr gut! Im folgenden Artikel erfahren Sie, wie Sie Offline-Konversionen von AdWords in Ihrem Umsatzmodell zuordnen.

>[!MORELIKETHIS]
>
>[Festlegen von Google AdWords-Konversionen im Umsatzmodell](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model.md)
