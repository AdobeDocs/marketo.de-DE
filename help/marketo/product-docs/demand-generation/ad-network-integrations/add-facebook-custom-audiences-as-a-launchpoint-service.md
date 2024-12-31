---
unique-page-id: 4720257
description: Hinzufügen benutzerdefinierter Facebook-Zielgruppen als LaunchPoint-Service - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen benutzerdefinierter Facebook-Zielgruppen als LaunchPoint-Service
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Hinzufügen benutzerdefinierter Facebook-Zielgruppen als LaunchPoint-Service {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

Mit dieser Integration können Sie Zielgruppendaten von statischen Marketo Engage- und Smart-Listen an Facebook senden, um sie als benutzerdefinierte Zielgruppen in Facebook-Anzeigenkampagnen zu verwenden. So richten Sie es ein.

1. Wechseln Sie zu Marketo **[!UICONTROL Admin]**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Wechseln Sie zu **[!UICONTROL LaunchPoint]**, klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neuer Service]** aus.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Geben Sie einen **[!UICONTROL Anzeigenamen]** für Ihren Dienst ein und wählen Sie den Dienst **[!UICONTROL Benutzerdefinierte Facebook]** Zielgruppen **[!UICONTROL aus der Dropdown-]** Service“ aus.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Öffnen Sie eine neue Registerkarte im selben Browser und navigieren Sie zu [facebook.com](https://www.facebook.com/){target="_blank"}. Melden Sie sich bei Facebook mit dem Konto an, das Sie für die Integration verwenden möchten.

   >[!CAUTION]
   >
   >Damit Marketo Zielgruppen über mehrere Ad Manager-Konten senden kann, muss der Facebook-Benutzer, den Sie in den folgenden Schritten autorisieren, Zugriff auf *alle* dieser Konten haben.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Nachdem Sie bei Facebook angemeldet sind, kehren Sie zu Marketo zurück. Klicken Sie **[!UICONTROL Autorisieren]**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >Sie _müssen_ ein Facebook Business Manager-Konto verwenden, damit Ihre Integration mit benutzerdefinierten Zielgruppen funktioniert. Informationen zum Einrichten eines Business Manager-Kontos finden Sie in der [Facebook-Hilfe](https://www.facebook.com/business/help/1710077379203657){target="_blank"}.

1. Klicken Sie auf **[!UICONTROL OK]**, um die Installation der Marketo-App in Facebook zu akzeptieren.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Sie sind jetzt autorisiert! Wählen Sie einen passenden Modus aus und klicken Sie auf **[!UICONTROL Erstellen]**.

   >[!NOTE]
   >
   >**Einfache Zuordnung** verwendet nur E-Mail-Adressen. **Erweiterter Abgleich** verwendet sieben zusätzliche Felder, was die Übereinstimmungsrate erhöht, um eine höhere Konversionsrate zu erzielen. Wenn die Datenschutzrichtlinie Ihres Unternehmens jedoch die Freigabe zusätzlicher Felder nicht zulässt oder Ihre Daten keine enthalten, wählen Sie die Option Grundlegende Übereinstimmung aus.

   ![](assets/fb-custom-adv-matching-hands.png)

   Gut gemacht! Sie können jetzt zu einer beliebigen statischen oder Smart-Liste in Marketo wechseln und Zielgruppendaten an Facebook senden.

   >[!CAUTION]
   >
   >Bevor Sie loslegen, sollten Sie [Benutzerdefinierte Zielgruppenbedingungen von Facebook akzeptieren](https://www.facebook.com/ads/manage/customaudiences/tos.php){target="_blank"} in Ihrem Facebook-Konto verwenden! Andernfalls schlagen die Aktualisierungen der Zielgruppe fehl.

>[!MORELIKETHIS]
>
>* [Erstellen einer benutzerdefinierten Zielgruppe in Facebook](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md){target="_blank"}
>
>* [Einrichten von Facebook-Lead-Anzeigen](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md){target="_blank"}
