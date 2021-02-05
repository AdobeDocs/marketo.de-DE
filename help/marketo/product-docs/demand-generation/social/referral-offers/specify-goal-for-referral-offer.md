---
unique-page-id: 2359791
description: Ziel für das Referrer-Angebot - Marketing-Dokumente - Produktdokumentation
title: Angebot für Verweis angeben
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Ziel für Referrer-Angebot {#specify-goal-for-referral-offer} angeben

Wenn Sie [ein Verweisziel erstellen, müssen Sie das Fulfillment-Angebot definieren. ](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) Das Ziel kann durch die persönliche Aktivität auf der Webseite definiert werden, z. B. durch Seitenbesuche oder Anmeldungen. Sie können sogar ein [benutzerdefiniertes JavaScript-Ereignis](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md) verwenden.

Alternativ können Sie einen Smart-Liste-Trigger in Marketo verwenden, um auf einen Meilenstein zu warten, z. B. eine Möglichkeit, die für die überweisende Person erstellt wird.

Beispielziele:

* 10 Besuche
* 5 Weitergeleitete Anmeldungen
* 1 benannte Chance
* 2 referenzierte E-Commerce-Käufe
* 5 überwiesene Webinar-Teilnehmer

1. Gehen Sie zu **Marketing-Aktivitäten**.

   ![](assets/ma.png)

1. Wählen Sie das verweisende Angebot aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. Wechseln Sie im Editor für Verweisdokumente zu **App-Einstellungen** > **Angebot-Details**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. Wählen Sie unter **Settings** einen Ereignistyp aus der Dropdownliste **Fulfillment-Ziel**.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Wenn Sie den Flussschritt **Gutschrift an Werber** verwenden möchten, müssen Sie **Trigger für intelligente Liste** als Zieltyp für die Erfüllung hier auswählen.

* Verweisende Besuche: Angebot-Teilnehmer erhalten eine Gutschrift für jeden Besuch von einem Freund auf der Seite, auf der sich Ihr Angebot befindet.
* Referred Sign-Ups: Angebot-Teilnehmer erhalten die Gutschrift für jeden Freund, der sich für das Angebot anmeldet.
* Trigger für intelligente Liste: Angebot-Teilnehmer erhalten die Gutschrift für jeden Freund, der die Voraussetzungen eines [Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md)-Triggers in einer [Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md) erfüllt. Sie können beispielsweise einen Trigger verwenden, der ausgelöst wird, wenn sich ein verwiesener Potenzieller Kunde für ein Webinar anmeldet.

* Benutzerdefiniertes JavaScript-Ereignis: Angebot-Teilnehmer erhalten die Gutschrift für jeden Freund, der ein definiertes JavaScript-Ereignis auf Ihrer Seite Trigger. Siehe [Konvertierungsskript für benutzerdefinierte Ereignis](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>In intelligenten Kampagnen stehen neue Filter und Trigger zur Überwachung der sozialen Aktivität zur Verfügung. Siehe [Verwenden Sie Trigger und Filter für Social-Aktivitäten](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>Als Nächstes können Sie [die Anmelde- und Fulfillment-E-Mails](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) auswählen, die von Ihrem Verweisdokument gesendet werden sollen.
