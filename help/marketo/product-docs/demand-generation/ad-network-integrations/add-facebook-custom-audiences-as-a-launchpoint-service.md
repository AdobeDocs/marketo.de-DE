---
unique-page-id: 4720257
description: Hinzufügen [!DNL Facebook] benutzerdefinierter Zielgruppen als  [!DNL LaunchPoint] -Service - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen [!DNL Facebook] benutzerdefinierter Zielgruppen als  [!DNL LaunchPoint] -Service
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Hinzufügen [!DNL Facebook] benutzerdefinierten Zielgruppen als [!DNL LaunchPoint] Service {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

Mit dieser Integration können Sie Zielgruppendaten aus statischen und Smart Lists von Marketo an [!DNL Facebook] senden, die als benutzerdefinierte Zielgruppen in [!DNL Facebook] Ad-Kampagnen verwendet werden. So richten Sie es ein.

1. Wechseln Sie zu Marketo **[!UICONTROL Admin]**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Gehen Sie zu **[!UICONTROL LaunchPoint]**, klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neuer Service]** aus.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Geben Sie einen **[!UICONTROL Anzeigenamen]** für Ihren Dienst ein und wählen Sie den Dienst **[!UICONTROL Facebook Custom Audiences]** aus der Dropdown-Liste **[!UICONTROL Dienst]** aus.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Öffnen Sie eine neue Registerkarte im selben Browser und gehen Sie zu [facebook.com](https://www.facebook.com/). Melden Sie sich bei [!DNL Facebook] mit dem Konto an, das Sie für die Integration verwenden möchten.

   >[!CAUTION]
   >
   >Damit Marketo Zielgruppen über mehrere Ad Manager-Konten senden kann, muss der [!DNL Facebook], den Sie in den folgenden Schritten autorisieren, Zugriff auf *alle* dieser Konten haben.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Nachdem Sie sich bei [!DNL Facebook] angemeldet haben, kehren Sie zu Marketo zurück. Klicken Sie **[!UICONTROL Autorisieren]**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >Sie *müssen* ein [!DNL Facebook] Business Manager-Konto verwenden, damit Ihre Integration mit benutzerdefinierten Zielgruppen funktioniert. Informationen zum Einrichten eines Business Manager-Kontos finden Sie unter [[!DNL Facebook] Hilfe](https://www.facebook.com/business/help/1710077379203657).

1. Klicken Sie auf **[!UICONTROL OK]**, um die Installation der Marketo-App in [!DNL Facebook] zu akzeptieren.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Sie sind jetzt autorisiert! Wählen Sie einen passenden Modus aus und klicken Sie auf **[!UICONTROL Erstellen]**.

   >[!NOTE]
   >
   >**[!UICONTROL Einfache Zuordnung]** verwendet nur E-Mail-Adressen. **[!UICONTROL Erweiterter Abgleich]** verwendet sieben zusätzliche Felder, was die Übereinstimmungsrate erhöht, um eine höhere Konversionsrate zu erzielen. Wenn die Datenschutzrichtlinie Ihres Unternehmens jedoch die Freigabe zusätzlicher Felder nicht zulässt oder Ihre Daten diese nicht enthalten, wählen Sie &quot;[!UICONTROL  Übereinstimmung“ ].

   ![](assets/fb-custom-adv-matching-hands.png)

   Gut gemacht! Sie können jetzt zu einer beliebigen statischen oder Smart-Liste in Marketo wechseln und Zielgruppendaten an [!DNL Facebook] senden.

   >[!CAUTION]
   >
   >Ach, bevor Sie gehen, stellen Sie sicher[ dass Sie  [!DNL Facebook]Benutzerdefinierte Zielgruppenbedingungen“ ](https://www.facebook.com/ads/manage/customaudiences/tos.php) Ihrem [!DNL Facebook]-Konto akzeptieren! Andernfalls schlagen die Aktualisierungen der Zielgruppe fehl.

>[!MORELIKETHIS]
>
>* [Erstellen einer benutzerdefinierten Zielgruppe in [!DNL Facebook]](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [Einrichten [!DNL Facebook] Lead-Anzeigen](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
