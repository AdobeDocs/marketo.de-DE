---
unique-page-id: 4720257
description: Hinzufügen benutzerdefinierter Facebook-Zielgruppen als LaunchPoint-Dienst - Marketo Docs - Produktdokumentation
title: Hinzufügen benutzerdefinierter Facebook-Zielgruppen als LaunchPoint-Dienst
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Hinzufügen benutzerdefinierter Facebook-Zielgruppen als LaunchPoint-Dienst {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

Mit dieser Integration können Sie Zielgruppendaten von statischen und intelligenten Marketo Engage-Listen an Facebook senden, um sie als benutzerdefinierte Zielgruppen in Facebook-Anzeigenkampagnen zu verwenden. So richten Sie es ein.

1. Navigieren Sie zu Marketo **[!UICONTROL Admin]**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Wechseln Sie zu **[!UICONTROL LaunchPoint]**, klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neuer Dienst]** aus.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Geben Sie einen **[!UICONTROL Anzeigenamen]** für Ihren Dienst ein und wählen Sie den Dienst **[!UICONTROL Facebook Custom Audiences]** aus der Dropdownliste **[!UICONTROL Dienst]** aus.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Öffnen Sie eine neue Registerkarte im selben Browser und navigieren Sie zu [facebook.com](https://www.facebook.com/){target="_blank"}. Melden Sie sich mit dem Konto, das Sie für die Integration verwenden möchten, bei Facebook an.

   >[!CAUTION]
   >
   >Damit Marketo Zielgruppen über mehrere Ad Manager-Konten hinweg senden kann, muss der Facebook-Benutzer, den Sie in den folgenden Schritten autorisieren, Zugriff auf *alle* dieser Konten haben.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Nachdem Sie sich bei Facebook angemeldet haben, kehren Sie zu Marketo zurück. Klicken Sie auf **[!UICONTROL Autorisieren]**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >Sie _müssen_ ein Facebook Business Manager-Konto verwenden, damit Ihre benutzerdefinierte Zielgruppenintegration funktioniert. Informationen zum Einrichten eines Business Manager-Kontos finden Sie in der [Hilfe zu Facebook](https://www.facebook.com/business/help/1710077379203657){target="_blank"}.

1. Klicken Sie bei Aufforderung auf **[!UICONTROL OK]** , um die Installation der Marketo-App in Facebook zu akzeptieren.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Du bist jetzt autorisiert! Wählen Sie einen entsprechenden Modus aus und klicken Sie auf **[!UICONTROL Erstellen]**.

   >[!NOTE]
   >
   >**Grundlegende Übereinstimmung** verwendet nur E-Mail-Adressen. **Erweiterte Übereinstimmung** verwendet sieben zusätzliche Felder, wodurch die Übereinstimmungsrate erhöht wird, für mehr Konvertierung. Wenn die Datenschutzrichtlinie Ihres Unternehmens jedoch die Freigabe zusätzlicher Felder nicht zulässt oder Ihre Daten diese nicht enthalten, wählen Sie &quot;Grundlegende Übereinstimmung&quot;.

   ![](assets/fb-custom-adv-matching-hands.png)

   Gut gemacht! Sie können jetzt zu jeder statischen oder intelligenten Liste in Marketo wechseln und Zielgruppendaten an Facebook senden.

   >[!CAUTION]
   >
   >Ach, bevor Sie fortfahren, stellen Sie sicher, dass Sie in Ihrem Facebook-Konto [Benutzerdefinierte Zielgruppenbedingungen von Facebook akzeptieren](https://www.facebook.com/ads/manage/customaudiences/tos.php){target="_blank"}! Andernfalls schlagen die Zielgruppen-Updates fehl.

>[!MORELIKETHIS]
>
>* [Erstellen einer benutzerdefinierten Zielgruppe in Facebook](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md){target="_blank"}
>
>* [Einrichten von Facebook-Lead-Anzeigen](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md){target="_blank"}
