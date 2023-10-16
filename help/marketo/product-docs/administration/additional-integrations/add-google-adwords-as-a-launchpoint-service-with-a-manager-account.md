---
unique-page-id: 7504893
description: "Hinzufügen [!DNL Google AdWords] as a [!DNL Launchpoint] Dienst mit einem Manager-Konto - Marketo Docs - Produktdokumentation"
title: "Hinzufügen [!DNL Google AdWords] as a [!DNL Launchpoint] Dienst mit einem Manager-Konto"
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
feature: Administration, Integrations
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 4%

---

# Hinzufügen [!DNL Google AdWords] as a [!DNL Launchpoint] Dienst mit einem Manager-Konto {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Verknüpfen [!DNL Google AdWords] Konto zu Marketo zum automatischen Hochladen von Offline-Konversionsdaten von Marketo in [!DNL Google AdWords]. Dann aus dem [!DNL AdWords] -Benutzeroberfläche können Sie einfach erkennen, welche Klicks zu qualifizierten Leads, Chancen und neuen Kunden (oder welchen Umsatzstufen Sie verfolgen möchten) geführt haben, nachdem Sie  [Benutzerdefinierte Spalten hinzufügen](https://support.google.com/adwords/answer/3073556){target="_blank"} in [!DNL AdWords]. Diese Informationen werden nicht in der Benutzeroberfläche von Marketo angezeigt.

Wenn Sie mehrere [!DNL Google Adwords] Konten können Sie eine [[!DNL Google AdWords Manager Account]](https://www.google.com/adwords/manager-accounts/){target="_blank"} (früher bekannt als [!DNL My Client Center]), um sie in Marketo zu integrieren.

Weitere Informationen [Google-Funktion für den Offline-Konversionsimport](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>Nicht alle Marketo Engage-Benutzer haben diese Funktion erworben. Weitere Informationen erhalten Sie vom Adobe Account Team (Ihrem Kundenbetreuer).

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!NOTE]
>
>Sie können auch eine [eigenständig [!DNL Google AdWords] als [!DNL Launchpoint] service](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md){target="_blank"}.

1. Navigieren Sie zum **[!UICONTROL Admin]**-Bereich.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-1.png)

1. Auswählen **[!UICONTROL LaunchPoint]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-2.png)

1. Klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neuer Dienst]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-3.png)

1. Geben Sie einen **[!UICONTROL Anzeigename]** und wählen **[!UICONTROL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-4.png)

1. Auswählen **[!UICONTROL Marketo autorisieren]**.

   >[!NOTE]
   >
   >Stellen Sie sicher, dass Sie sich von Ihrem persönlichen [!DNL Gmail] und aktivieren Sie Popups.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-5.png)

1. Wählen Sie Ihr Konto aus, das mit **[!DNL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-6.png)

1. Klicks **[!UICONTROL Accept]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-7.png)

1. Der Status wird als **[!UICONTROL Erfolg]**. Auswählen **[!UICONTROL Nächste]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-8.png)

1. Hochladen der Offline-Konvertierungen von Marketo in [!DNL Google AdWords] **[!UICONTROL Wöchentlich]** oder **[!UICONTROL Täglich]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-9.png)

1. Attributkonvertierung in **[!UICONTROL Erster Klick]** oder **[!UICONTROL Letzter Klick]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-10.png)

   | Typ | Definition |
   |---|---|
   | [!UICONTROL Erster Klick] | Offline-Konversionen werden der ersten [!DNL AdWords] und dass eine Person in den letzten 90 Tagen geklickt hat |
   | [!UICONTROL Letzter Klick] | Offline-Konversionen werden der letzten [!DNL AdWords] und dass eine Person geklickt hat |

   >[!NOTE]
   >
   >[Automatisches Tagging](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"} muss ausgewählt sein, damit diese Funktion funktioniert. Sie muss in [!DNL AdWords].

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-11.png)

1. Deaktivieren Sie die Konten, die Sie nicht aktualisieren möchten. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-12.png)

   Informationen zur Zuordnung finden Sie jetzt im entsprechenden Artikel unten [!DNL AdWords] Offline-Konversionen in Ihrem Umsatzmodell.

   >[!MORELIKETHIS]
   >
   >[Satz [!DNL Google AdWords] Konversionen im Umsatzmodell mit einem Manager-Konto](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md){target="_blank"}
