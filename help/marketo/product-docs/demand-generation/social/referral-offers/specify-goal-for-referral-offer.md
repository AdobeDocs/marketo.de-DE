---
unique-page-id: 2359791
description: Ziel für Verweisangebot angeben - Marketo Docs - Produktdokumentation
title: Ziel für Verweisangebot angeben
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Ziel für Verweisangebot angeben {#specify-goal-for-referral-offer}

Wenn Sie [Erstellen eines Verweisangebots](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)müssen Sie das Erfüllungsziel definieren. Das Ziel kann durch die Personenaktivität auf der Webseite definiert werden, z. B. Seitenbesuche oder Anmeldungen. Sie können sogar eine [benutzerdefiniertes JavaScript-Ereignis](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

Alternativ können Sie einen Trigger mit der intelligenten Liste in Marketo verwenden, um auf einen Meilenstein zu warten, z. B. eine Chance, die für die referenzierte Person erstellt wurde.

Beispielziele:

* 10 Besuche
* 5 weitergeleitete Anmeldungen
* 1 überwiesene Chance
* 2 referenzierte E-Commerce-Käufe
* 5 verwiesene Webinarteilnehmer

1. Navigieren Sie zu **Marketingaktivitäten**.

   ![](assets/ma.png)

1. Wählen Sie das Angebot aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. Navigieren Sie im Angebotseditor zu **App-Einstellungen** > **Angebotsdetails**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. under **Einstellungen**, wählen Sie einen Ereignistyp aus der **Erfüllungsziel** angezeigt.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Wenn Sie die **Gutschrift an verweisende Stelle** Flussschritt: Sie müssen **Smart List Trigger** als Zieltyp für die Erfüllung.

* Referred Visits: Angebotsteilnehmer erhalten die Gutschrift für jeden Besuch von einem Freund auf der Seite, auf der Ihr Angebot gehostet wird.
* Referred Sign-Ups: Angebotsteilnehmer erhalten die Gutschrift für jeden Freund, der sich für das Angebot anmeldet.
* Smart List Trigger: Die Teilnehmer des Angebots erhalten die Gutschrift für jeden Freund, der die Bedingungen eines [Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) Trigger in einem [Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md). Sie können beispielsweise einen Trigger verwenden, der ausgelöst wird, wenn sich ein überwiesener Interessent für ein Webinar anmeldet.

* Benutzerspezifisches JavaScript-Ereignis: Die Teilnehmer des Angebots erhalten die Gutschrift für jeden Freund, der ein bestimmtes JavaScript-Ereignis auf Ihrer Seite Trigger. Siehe [Konversionsskript für benutzerspezifische Ereignisse](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>In Smart-Kampagnen stehen neue Filter und Trigger zur Überwachung sozialer Aktivitäten zur Verfügung. Siehe [Verwenden von Triggern und Filtern für Social-Aktivitäten](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>Als Nächstes können Sie [die Anmelde- und Erfüllungs-E-Mails auswählen](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) über Ihr Verweisangebot zu senden.
