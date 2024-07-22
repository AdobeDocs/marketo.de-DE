---
unique-page-id: 2359793
description: Verwenden von E-Mails in Social Promotions - Marketo Docs - Produktdokumentation
title: Verwenden von E-Mails in Social Promotions
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Verwenden von E-Mails in Social Promotions {#use-emails-in-social-promotions}

Wenn Sie ein [Verweisangebot](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) oder ein [Preisausschreiben](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md) erstellen, können Sie E-Mails einfügen, die gesendet werden, wenn sich die Person anmeldet, und erneut, wenn die Person die Belohnung gewonnen hat.

>[!TIP]
>
>Informationen zum Erstellen einer E-Mail finden Sie unter [E-Mail-Versand durchführen](/help/marketo/getting-started/quick-wins/send-an-email.md).

Verwenden Sie in den E-Mails die folgenden Token:

* **Anmelde-E-Mail**: Verwenden Sie **`{{social.Share Url}}`**, um jeder beteiligten Person einen personalisierten Freigabe-Link zu senden.

* **E-Mail zum Ausfüllen**: Verwenden Sie **`{{social.Promo Code}}`**, um jedem Gewinner einen [Promo-Code](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) zu senden.

>[!PREREQUISITES]
>
>Bevor Sie eine E-Mail zu einer Social-App hinzufügen können, muss sie _operativ_ und _genehmigt_ sein. Siehe [Einstellungen für eine E-Mail bearbeiten](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. Wechseln Sie zu **Marketingaktivitäten**.

   ![](assets/ma.png)

1. Wählen Sie die App aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. Navigieren Sie im Social-App-Editor zu **App-Einstellungen > Angebotsdetails** (oder **Preisausschreiben-Details**).

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. Fügen Sie die Anmelde-E-Mail hinzu.

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >Die Bestätigungs-E-Mail wird automatisch gesendet, wenn sich eine Person anmeldet.

1. Fügen Sie die E-Mail zur Erfüllung hinzu.

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. Wählen Sie in einem Verweisangebot aus, ob die Erfüllungs-E-Mail automatisch oder manuell gesendet wird.

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>Bei einem Gewinnspiel wird die Erfüllungs-E-Mail immer automatisch gesendet, wenn Sie [den Gewinner auswählen](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**Definition**
>
>* **auto on target**: Die Erfüllungs-E-Mail wird automatisch gesendet, wenn jeder Teilnehmer das Ziel erfüllt.
>* **manuell senden**: Sobald die Zielgruppe das Ziel erreicht hat, kehren Sie zu Ihrem Verweisangebot zurück, um die Erfüllungs-E-Mail ](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) manuell zu senden.[
>

>[!MORELIKETHIS]
>
>Als Nächstes können Sie [die Freigabe-URL](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) auswählen oder in Ihrem Verweisangebot [die Promo-Codes hochladen](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md), die Sie senden.
