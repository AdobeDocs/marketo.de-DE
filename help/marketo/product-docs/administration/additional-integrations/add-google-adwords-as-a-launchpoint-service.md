---
unique-page-id: 6095008
description: Hinzufügen von [!DNL Google AdWords] as a [!DNL LaunchPoint] service - Marketo Docs - Produktdokumentation
title: Hinzufügen von [!DNL Google AdWords] als [!DNL LaunchPoint] Dienst
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
feature: Administration, Integrations
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 2%

---

# Hinzufügen von [!DNL Google AdWords] als [!DNL LaunchPoint]-Dienst {#add-google-adwords-as-a-launchpoint-service}

Verknüpfen Sie Ihr [!DNL Google AdWords] -Konto mit Marketo, um Offline-Konversionsdaten automatisch von Marketo in [!DNL Google AdWords] hochzuladen. Anschließend können Sie in der Benutzeroberfläche von [!DNL AdWords] einfach sehen, welche Klicks zu qualifizierten Leads, Chancen und neuen Kunden (oder welchen Umsatzstufen Sie verfolgen möchten) geführt haben, nachdem Sie [benutzerdefinierte Spalten hinzufügen](https://support.google.com/adwords/answer/3073556){target="_blank"} in [!DNL AdWords]. Diese Informationen werden nicht in der Benutzeroberfläche von Marketo angezeigt.

Erfahren Sie mehr über die Funktion [Google für den Offline-Konversionsimport](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>Nicht alle Marketo Engage-Benutzer haben diese Funktion erworben. Weitere Informationen erhalten Sie vom Adobe Account Team (Ihrem Kundenbetreuer).

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!NOTE]
>
>Sie können auch einen [[!DNL Google AdWords] as a [!DNL Launchpoint] Dienst in ein Managerkonto](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md){target="_blank"} integrieren.

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/add-google-adwords-as-a-launchpoint-service-1.png)

1. Wählen Sie **[!UICONTROL LaunchPoint]** aus.

   ![](assets/add-google-adwords-as-a-launchpoint-service-2.png)

1. Wählen Sie **[!UICONTROL Neu]** und **[!UICONTROL Neuer Dienst]** aus.

   ![](assets/add-google-adwords-as-a-launchpoint-service-3.png)

1. Geben Sie einen [!UICONTROL Anzeigenamen] ein und wählen Sie **[!UICONTROL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-4.png)

1. Wählen Sie **[!UICONTROL Marketo autorisieren]** aus.

   >[!NOTE]
   >
   >Melden Sie sich bei Ihrem persönlichen [!DNL Gmail] -Konto ab und aktivieren Sie Pop-ups.

   ![](assets/add-google-adwords-as-a-launchpoint-service-5.png)

1. Wählen Sie Ihr Konto aus, das mit [!DNL Google AdWords] verknüpft ist.

   ![](assets/add-google-adwords-as-a-launchpoint-service-6.png)

1. Wählen Sie **[!UICONTROL Accept]** aus.

   ![](assets/add-google-adwords-as-a-launchpoint-service-7.png)

1. Der Status wird als **[!UICONTROL Erfolg]** angezeigt. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-8.png)

1. Laden Sie Ihre Offline-Konversionen von Marketo in [!DNL Google AdWords] **[!UICONTROL Wöchentlich]** oder **[!UICONTROL Täglich]** hoch.

   ![](assets/add-google-adwords-as-a-launchpoint-service-9.png)

1. Attributkonvertierung in **[!UICONTROL Ersten Klick]** oder **[!UICONTROL Letzten Klick]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-10.png)

   | Typ | Definition |
   |---|---|
   | [!UICONTROL Erster Klick] | Offline-Konversionen werden der ersten [!DNL AdWords] zugeordnet, auf die eine Person in den letzten 90 Tagen geklickt hat. |
   | [!UICONTROL Letzter Klick] | Offline-Konversionen werden der letzten [!DNL AdWords] zugeordnet, auf die eine Person geklickt hat |

   >[!NOTE]
   >
   >Die Verwendung eines konsistenten Attributionsmodells in Marketo und [!DNL AdWords] liefert die präzisesten Daten.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-11.png)

   >[!NOTE]
   >
   >[Automatisches Tagging](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"} muss ausgewählt sein, damit diese Funktion funktioniert. Die Deaktivierung muss innerhalb von [!DNL AdWords] erfolgen.

Sehr gut! Sehen Sie sich nun den unten stehenden zugehörigen Artikel an, um zu erfahren, wie Sie Offline-Konversionen in Ihrem Umsatzmodell zuordnen können.[!DNL AdWords]

>[!MORELIKETHIS]
>
>[Festlegen [!DNL Google AdWords] der Konversionen im Umsatzmodell](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model.md){target="_blank"}
