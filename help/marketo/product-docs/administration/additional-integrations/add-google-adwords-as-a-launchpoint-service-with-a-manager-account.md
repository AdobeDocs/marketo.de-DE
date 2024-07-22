---
unique-page-id: 7504893
description: "Hinzufügen von [!DNL Google AdWords] als [!DNL Launchpoint] Dienst mit einem Manager-Konto - Marketo Docs - Produktdokumentation"
title: "Hinzufügen von [!DNL Google AdWords] als [!DNL Launchpoint] Dienst mit einem Manager-Konto"
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
feature: Administration, Integrations
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 1%

---

# Hinzufügen von [!DNL Google AdWords] als [!DNL Launchpoint]-Dienst mit einem Managerkonto {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Verknüpfen Sie Ihr [!DNL Google AdWords] -Konto mit Marketo, um Offline-Konversionsdaten automatisch von Marketo in [!DNL Google AdWords] hochzuladen. Anschließend können Sie in der Benutzeroberfläche von [!DNL AdWords] einfach sehen, welche Klicks zu qualifizierten Leads, Chancen und neuen Kunden (oder zu welchen Umsatzphasen Sie verfolgen möchten) geführt haben, nachdem Sie [benutzerdefinierte Spalten hinzufügen](https://support.google.com/adwords/answer/3073556){target="_blank"} in [!DNL AdWords]. Diese Informationen werden nicht in der Benutzeroberfläche von Marketo angezeigt.

Wenn Sie mehrere [!DNL Google Adwords] -Konten haben, können Sie eine [[!DNL Google AdWords Manager Account]](https://www.google.com/adwords/manager-accounts/){target="_blank"} (ehemals [!DNL My Client Center]) verwenden, um sie in Marketo zu integrieren.

Erfahren Sie mehr über die Funktion [Google für den Offline-Konversionsimport](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>Nicht alle Marketo Engage-Benutzer haben diese Funktion erworben. Weitere Informationen erhalten Sie vom Adobe Account Team (Ihrem Kundenbetreuer).

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!NOTE]
>
>Sie können auch ein [eigenständiges [!DNL Google AdWords] Konto als  [!DNL Launchpoint] Dienst](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md){target="_blank"} integrieren.

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-1.png)

1. Wählen Sie **[!UICONTROL LaunchPoint]** aus.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-2.png)

1. Klicken Sie auf die Dropdownliste **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neuer Dienst]** aus.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-3.png)

1. Geben Sie einen **[!UICONTROL Anzeigenamen]** ein und wählen Sie **[!UICONTROL Google AdWords]** aus.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-4.png)

1. Wählen Sie **[!UICONTROL Marketo autorisieren]** aus.

   >[!NOTE]
   >
   >Melden Sie sich bei Ihrem persönlichen [!DNL Gmail] -Konto ab und aktivieren Sie Pop-ups.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-5.png)

1. Wählen Sie Ihr Konto aus, das mit **[!DNL Google AdWords]** verknüpft ist.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-6.png)

1. Klicken Sie auf **[!UICONTROL Accept]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-7.png)

1. Der Status wird als **[!UICONTROL Erfolg]** angezeigt. Wählen Sie **[!UICONTROL Weiter]** aus.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-8.png)

1. Laden Sie Ihre Offline-Konversionen von Marketo in [!DNL Google AdWords] **[!UICONTROL Wöchentlich]** oder **[!UICONTROL Täglich]** hoch.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-9.png)

1. Attributkonvertierung in **[!UICONTROL Ersten Klick]** oder **[!UICONTROL Letzten Klick]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-10.png)

   | Typ | Definition |
   |---|---|
   | [!UICONTROL Erster Klick] | Offline-Konversionen werden der ersten [!DNL AdWords] zugeordnet, auf die eine Person in den letzten 90 Tagen geklickt hat. |
   | [!UICONTROL Letzter Klick] | Offline-Konversionen werden der letzten [!DNL AdWords] zugeordnet, auf die eine Person geklickt hat |

   >[!NOTE]
   >
   >[Automatisches Tagging](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"} muss ausgewählt sein, damit diese Funktion funktioniert. Sie muss innerhalb von [!DNL AdWords] aktiviert werden.

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-11.png)

1. Deaktivieren Sie die Konten, die Sie nicht aktualisieren möchten. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-with-a-manager-12.png)

   Im folgenden Artikel erfahren Sie, wie Sie Offline-Konversionen in Ihrem Umsatzmodell zuordnen können.[!DNL AdWords]

   >[!MORELIKETHIS]
   >
   >[Festlegen [!DNL Google AdWords] der Konversionen im Umsatzmodell mit einem Manager-Konto](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md){target="_blank"}
