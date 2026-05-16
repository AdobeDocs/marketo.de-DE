---
unique-page-id: 6095008
description: Verknüpfung  [!DNL Google AdWords]  Marketo über LaunchPoint zum Hochladen von Offline-Konversionsdaten für das Reporting in AdWords.
title: ' [!DNL Google AdWords]  as a [!DNL LaunchPoint] Service'
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
feature: Administration, Integrations
TQID: https://experienceleague.adobe.com/gpw57sy3WitNAh6g4mkajXuuFlRFzunZmfedM4aCrCk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 284
ht-degree: 3%

---

# Hinzufügen von [!DNL Google AdWords] as a [!DNL LaunchPoint] Service {#add-google-adwords-as-a-launchpoint-service}

Verknüpfen Sie Ihr [!DNL Google AdWords] mit Marketo, um Offline-Konversionsdaten automatisch von Marketo in [!DNL Google AdWords] hochzuladen. In der [!DNL AdWords]-Benutzeroberfläche können Sie dann sehen, welche Klicks zu qualifizierten Leads, Chancen und neuen Kunden (oder zu welchen Umsatzstadien Sie verfolgen möchten) geführt haben, nachdem Sie [benutzerdefinierte Spalten hinzufügen](https://support.google.com/adwords/answer/3073556){target="_blank"} in [!DNL AdWords] hinzugefügt haben. Diese Informationen werden nicht in der Marketo-Benutzeroberfläche angezeigt.

Erfahren Sie mehr über die Offline-Konversions-Importfunktion von [&#128279;](https://support.google.com/adwords/answer/2998031?hl=en){target="_blank"}.

>[!AVAILABILITY]
>
>Nicht alle Marketo Engage-Benutzer haben diese Funktion erworben. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).

>[!NOTE]
>
>**Admin-Berechtigungen erforderlich**

>[!NOTE]
>
>Sie können auch einen [[!DNL Google AdWords] as a [!DNL Launchpoint] Service mit einem Manager-Konto &#x200B;](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md){target="_blank"}.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-1.png)

1. Wählen Sie **[!UICONTROL LaunchPoint]** aus.

   ![](assets/add-google-adwords-as-a-launchpoint-service-2.png)

1. Wählen Sie **[!UICONTROL Neu]** und **[!UICONTROL Neuer Service]** aus.

   ![](assets/add-google-adwords-as-a-launchpoint-service-3.png)

1. Geben Sie einen [!UICONTROL Anzeigenamen] ein und wählen Sie **[!UICONTROL Google AdWords]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-4.png)

1. Wählen Sie **[!UICONTROL Marketo autorisieren]** aus.

   >[!NOTE]
   >
   >Achten Sie darauf, sich von Ihrem persönlichen [!DNL Gmail]-Konto abzumelden und Popups zu aktivieren.

   ![](assets/add-google-adwords-as-a-launchpoint-service-5.png)

1. Wählen Sie Ihr Konto aus, das mit [!DNL Google AdWords] verknüpft ist.

   ![](assets/add-google-adwords-as-a-launchpoint-service-6.png)

1. Wählen Sie **[!UICONTROL Akzeptieren]** aus.

   ![](assets/add-google-adwords-as-a-launchpoint-service-7.png)

1. Der Status wird als **[!UICONTROL Erfolg]** angezeigt. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-8.png)

1. Laden Sie Ihre Offline-Konversionen von Marketo in [!DNL Google AdWords] **[!UICONTROL wöchentlich]** oder **[!UICONTROL täglich]** hoch.

   ![](assets/add-google-adwords-as-a-launchpoint-service-9.png)

1. Attributkonvertierung in „Erster **[!UICONTROL &quot;]** &quot;**[!UICONTROL letzten]**&quot;.

   ![](assets/add-google-adwords-as-a-launchpoint-service-10.png)

   | Typ | Definition |
   |---|---|
   | [!UICONTROL Erster Klick] | Offline-Konversionen werden der ersten [!DNL AdWords]-Anzeige zugeordnet, auf die eine Person in den letzten 90 Tagen geklickt hat |
   | [!UICONTROL Letzter Klick] | Offline-Konversionen werden der letzten [!DNL AdWords] zugeordnet, auf die eine Person geklickt hat |

   >[!NOTE]
   >
   >Die Verwendung eines konsistenten Attributionsmodells in Marketo und [!DNL AdWords] liefert die genauesten Daten.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/add-google-adwords-as-a-launchpoint-service-11.png)

   >[!NOTE]
   >
   >[Automatisches Tagging](https://support.google.com/adwords/answer/1752125?hl=en){target="_blank"} muss ausgewählt sein, damit diese Funktion funktioniert. Die Deaktivierung muss innerhalb von [!DNL AdWords] erfolgen.

Im folgenden verwandten Artikel erfahren Sie, wie Sie [!DNL AdWords] Offline-Konversionen in Ihrem Umsatzmodell zuordnen.
