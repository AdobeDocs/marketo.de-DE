---
unique-page-id: 4720257
description: hinzufügen benutzerspezifische Facebook-Audiencen als LaunchPoint-Dienst - Marketing-Dokumente - Produktdokumentation
title: hinzufügen benutzerdefinierter Facebook-Audiencen als LaunchPoint-Dienst
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---


# hinzufügen benutzerspezifische Facebook-Audiencen als LaunchPoint-Dienst {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

Mit dieser Integration können Sie Daten zur Audience von Marketo-statischen und intelligenten Listen an Facebook senden, um sie als benutzerdefinierte Audiencen in Facebook-Werbeanzeigen-Kampagnen zu verwenden. So richten Sie es ein:

1. Gehen Sie zu Markieren **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Gehen Sie zu **LaunchPoint**, klicken Sie auf **New** und wählen Sie **New Service**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Geben Sie einen **Anzeigenamen** für Ihren Dienst ein und wählen Sie den Dienst **Facebook Benutzerspezifische Audiencen** aus der Dropdownliste **Dienst**.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Öffnen Sie eine neue Registerkarte im selben Browser und gehen Sie zu [www.facebook.com.](http://www.facebook.com./) Melden Sie sich bei Facebook mit dem Konto an, das Sie für die Integration verwenden möchten.

   >[!CAUTION]
   >
   >Damit Marketing Audiencen über mehrere Ad Manager-Konten senden kann, muss der Facebook-Benutzer, den Sie in den folgenden Schritten autorisieren, Zugriff auf *alle* dieser Konten haben.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Wenn Sie bei Facebook angemeldet sind, kehren Sie zu Marketo zurück. Klicken Sie auf **Autorisieren**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >Sie müssen *ein Facebook Business Manager-Konto verwenden, damit Ihre Integration mit benutzerspezifischen Audiencen funktioniert.* Informationen zum Einrichten eines Business Manager-Kontos finden Sie in der [Facebook-Hilfe](https://www.facebook.com/business/help/1710077379203657).

1. Wenn Sie dazu aufgefordert werden, klicken Sie auf **OK **OK, um die Installation der Marketing-App in Facebook zu akzeptieren.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Du bist jetzt autorisiert! Wählen Sie einen passenden Modus und klicken Sie auf **Erstellen**.

   >[!NOTE]
   >
   >**Basis-Übereinstimmung** verwendet nur E-Mail-Adressen.**Advanced** Matchinguses verwendet sieben weitere Felder, wodurch die Übereinstimmungsrate erhöht wird, um mehr Konversionen zu erzielen. Wenn die Datenschutzrichtlinien Ihrer Firma die Freigabe zusätzlicher Felder nicht zulassen oder wenn Ihre Daten diese nicht enthalten, wählen Sie &quot;Grundlegende Übereinstimmung&quot;.

   ![](assets/fb-custom-adv-matching-hands.png)

   Gute Arbeit! Sie können jetzt zu jeder statischen oder intelligenten Liste in Marketo wechseln und Daten zur Audience an Facebook senden.

   >[!CAUTION]
   >
   >Ach, bevor Sie gehen, stellen Sie sicher, dass Sie in Ihrem Facebook-Konto [die benutzerspezifischen Audiencen von Facebook akzeptieren](https://www.facebook.com/ads/manage/customaudiences/tos.php)! Andernfalls schlagen die Aktualisierungen der Audience fehl.

>[!MORELIKETHIS]
>
>* [Erstellen einer benutzerspezifischen Audience in Facebook](../../../product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
   >
   >
* [Einrichten von Facebook-Interessentenanzeigen](../../../product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)

>



