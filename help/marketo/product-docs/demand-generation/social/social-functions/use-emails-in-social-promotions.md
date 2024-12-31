---
unique-page-id: 2359793
description: Verwenden von E-Mails in Social-Media-Werbeaktionen - Marketo-Dokumente - Produktdokumentation
title: Verwenden von E-Mails in Social-Media-Promotions
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Verwenden von E-Mails in Social-Media-Promotions {#use-emails-in-social-promotions}

Wenn Sie ein [Verweisangebot](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) oder ein [Gewinnspiel](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md) erstellen, können Sie E-Mails einfügen, die gesendet werden, wenn sich die Person anmeldet, und erneut, wenn die Person die Belohnung gewonnen hat.

>[!IMPORTANT]
>
>Am 31. Juli 2024 haben wir mit der Einstellung dieser Funktion begonnen. Neue Assets können nicht mehr erstellt werden. Vorhandene Assets funktionieren bis zum 31. Januar 2025 weiterhin. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!TIP]
>
>Informationen zum Erstellen einer E-Mail finden Sie unter [Senden einer E-Mail-Explosion](/help/marketo/getting-started/quick-wins/send-an-email.md).

Verwenden Sie in E-Mails diese Token:

* **Anmelde-E-Mail**: Verwenden Sie **`{{social.Share Url}}`**, um jeder teilnehmenden Person einen personalisierten Freigabe-Link zu senden.

* **Erfüllungs-E**: Verwenden Sie **`{{social.Promo Code}}`**, um jedem Gewinner einen [Promo-Code](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) zu senden.

>[!PREREQUISITES]
>
>Bevor Sie eine E-Mail zu einer Social-Media-App hinzufügen können, muss sie _betriebsbereit_ und _genehmigt_ sein. Siehe [Bearbeiten von Einstellungen für eine E-Mail](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. Navigieren Sie **Marketing-Aktivitäten**.

   ![](assets/ma.png)

1. Wählen Sie die App aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. Wechseln Sie im Social-App-Editor zu **App-Einstellungen >** (oder **Gewinnspieldetails**).

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. Fügen Sie die Anmelde-E-Mail hinzu.

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >Die Bestätigungs-E-Mail wird automatisch gesendet, wenn sich eine Person anmeldet.

1. Erfüllungs-E-Mail hinzufügen.

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. Wählen Sie in einem Empfehlungsangebot aus, ob die Erfüllungs-E-Mail automatisch oder manuell gesendet werden soll.

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>Bei einem Gewinnspiel wird die Erfüllungs-E-Mail immer automatisch gesendet, wenn Sie [Gewinner auswählen](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**Definition**
>
>* **Automatisch bei Ziel**: Die Erfüllungs-E-Mail wird automatisch gesendet, wenn jeder Teilnehmer das Ziel erreicht.
>* **Manuell senden**: Sobald Personen das Ziel erreichen, kehren Sie zu Ihrem Empfehlungsangebot zurück, um die [-E-Mail zur Erfüllung manuell zu ](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md).
>

>[!MORELIKETHIS]
>
>Als Nächstes können Sie [die Freigabe-URL auswählen](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) oder in Ihrem Empfehlungsangebot [die Promo-Codes hochladen](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) die Sie versenden werden.
