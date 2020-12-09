---
unique-page-id: 2359791
description: Ziel für das Referrer-Angebot - Marketing-Dokumente - Produktdokumentation
title: Angebot für Verweis angeben
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# Angebot für Verweis angeben {#specify-goal-for-referral-offer}

Beim [Erstellen eines Verweisziels](create-a-referral-offer.md)müssen Sie das Fulfillment-Angebot definieren. Das Ziel kann durch die persönliche Aktivität auf der Webseite definiert werden, z. B. durch Seitenbesuche oder Anmeldungen. Sie können sogar ein [benutzerdefiniertes JavaScript-Ereignis](../../../../product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md)verwenden.

Alternativ können Sie einen [Smart-Liste-Auslöser](specify-goal-for-referral-offer.md) in Marketo verwenden, um auf einen Meilenstein zu warten, z. B. eine Möglichkeit, die für die überweisende Person erstellt wird.

Beispielziele:

* 10 Besuche
* 5 Weitergeleitete Anmeldungen
* 1 benannte Chance
* 2 referenzierte E-Commerce-Käufe
* 5 überwiesene Webinar-Teilnehmer

1. Gehen Sie zu **Marketing-Aktivitäten**.

   ![](assets/ma.png)

1. Wählen Sie das verweisende Angebot aus und klicken Sie auf Entwurf **bearbeiten.**

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. Wechseln Sie im Editor für Verweisdokumente zu **App-Einstellungen** > **Angebot-Details.**

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. Wählen Sie unter **Einstellungen** einen Ereignistyp aus der Dropdownliste **Fulfillment-Ziel** .

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Wenn Sie den Flussschritt **Gutschrift an Werber** geben verwenden möchten, müssen Sie hier den **Smart-Liste-Auslöser** als Zieltyp für die Erfüllung auswählen.

* Verweisende Besuche: Angebot-Teilnehmer erhalten eine Gutschrift für jeden Besuch von einem Freund auf der Seite, auf der sich Ihr Angebot befindet.
* Referred Sign-Ups: Angebot-Teilnehmer erhalten die Gutschrift für jeden Freund, der sich für das Angebot anmeldet.
* Auslöser für intelligente Liste: Angebot-Teilnehmer erhalten die Gutschrift für jeden Freund, der die Bedingungen eines [intelligenten Listen](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) -Auslösers in einer [intelligenten Kampagne](http://docs.marketo.com/display/docs/smart+campaigns)erfüllt. Sie können beispielsweise einen Auslöser verwenden, der ausgelöst wird, wenn sich ein verwiesener Potenzieller Kunde für ein Webinar anmeldet.

* Benutzerdefiniertes JavaScript-Ereignis: Angebot-Teilnehmer erhalten die Gutschrift für jeden Freund, der ein definiertes JavaScript-Ereignis auf Ihrer Seite auslöst. Siehe [Konvertierungsskript für benutzerdefinierte Ereignis](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>In intelligenten Kampagnen stehen neue Filter und Auslöser zur Überwachung der sozialen Aktivität zur Verfügung. Siehe [Verwenden von Triggern und Filtern für Social-Aktivitäten](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>Als Nächstes können Sie die [Anmelde- und Fulfillment-E-Mails](send-referral-offer-fulfillment-email.md) auswählen, die Sie von Ihrem Verweisdokument aus senden möchten.

