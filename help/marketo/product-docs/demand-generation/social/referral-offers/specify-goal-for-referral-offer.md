---
unique-page-id: 2359791
description: Ziel für Verweisangebot angeben - Marketo Docs - Produktdokumentation
title: Ziel für Verweisangebot angeben
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 0%

---

# Ziel für Verweisangebot angeben {#specify-goal-for-referral-offer}

Wenn Sie [ein Verweisangebot erstellen](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md), müssen Sie das Erfüllungsziel definieren. Das Ziel kann durch die Personenaktivität auf der Webseite definiert werden, z. B. Seitenbesuche oder Anmeldungen. Sie können sogar ein [benutzerspezifisches JavaScript-Ereignis](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md) verwenden.

>[!IMPORTANT]
>
>Am 31. Juli 2024 begannen wir mit der Einstellung dieser Funktion. Neue Assets können nicht mehr erstellt werden. Vorhandene Assets werden bis zum 31. Januar 2025 weiterhin funktionieren. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

Alternativ können Sie einen Smart-List-Trigger in Marketo Engage verwenden, um auf einen Meilenstein zu warten, z. B. eine Chance, für die referenzierte Person erstellt zu werden.

Beispielziele:

* 10 Besuche
* 5 weitergeleitete Anmeldungen
* 1 überwiesene Chance
* 2 referenzierte E-Commerce-Käufe
* 5 verwiesene Webinarteilnehmer

1. Wechseln Sie zu **Marketingaktivitäten**.

   ![](assets/ma.png)

1. Wählen Sie das Verweisangebot aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. Navigieren Sie im Editor für Verweise zu **App-Einstellungen** > **Angebotsdetails**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. Wählen Sie unter **Einstellungen** einen Ereignistyp aus der Dropdown-Liste **Erfüllungsziel** aus.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Wenn Sie den Flussschritt **Gutschrift für verweisende Stelle** verwenden möchten, müssen Sie hier **Trigger für intelligente Liste** als Zieltyp für die Erfüllung auswählen.

* Referred Visits: Angebotsteilnehmer erhalten die Gutschrift für jeden Besuch von einem Freund auf der Seite, auf der Ihr Angebot gehostet wird.
* Referred Sign-Ups: Angebotsteilnehmer erhalten die Gutschrift für jeden Freund, der sich für das Angebot anmeldet.
* Smart List Trigger: Angebotsteilnehmer erhalten die Gutschrift für jeden Freund, der die Voraussetzungen eines [Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) -Triggers in einer [Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md) erfüllt. Sie können beispielsweise einen Trigger verwenden, der ausgelöst wird, wenn sich ein überwiesener Interessent für ein Webinar anmeldet.

* Benutzerspezifisches JavaScript-Ereignis: Die Angebotsteilnehmer erhalten die Gutschrift für jeden Freund, der ein bestimmtes JavaScript-Ereignis auf Ihrer Seite Trigger. Siehe [Konvertierungsskript für benutzerdefinierte Ereignisse](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>In Smart-Kampagnen stehen neue Filter und Trigger zur Überwachung sozialer Aktivitäten zur Verfügung. Siehe [Verwenden von Triggern und Filtern für soziale Aktivitäten](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>Als Nächstes können Sie [die Anmelde- und Erfüllungs-E-Mails auswählen](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md), die von Ihrem Verweisangebot gesendet werden sollen.
