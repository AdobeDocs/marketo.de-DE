---
unique-page-id: 2359791
description: Ziel für Empfehlungsangebot angeben - Marketo-Dokumente - Produktdokumentation
title: Ziel für Empfehlungsangebot angeben
exl-id: 9869eb66-53df-4ea8-903f-e6650add8da2
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 0%

---

# Ziel für Empfehlungsangebot angeben {#specify-goal-for-referral-offer}

Wenn Sie [ein Empfehlungsangebot erstellen](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) müssen Sie das Erfüllungsziel definieren. Das Ziel kann durch die Aktivität einer Person auf der Web-Seite definiert werden, z. B. Seitenbesuche oder Anmeldungen. Sie können auch ein [benutzerdefiniertes JavaScript-Ereignis“ ](/help/marketo/product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md).

>[!IMPORTANT]
>
>Am 31. Juli 2024 haben wir mit der Einstellung dieser Funktion begonnen. Neue Assets können nicht mehr erstellt werden. Vorhandene Assets funktionieren bis zum 31. Januar 2025 weiterhin. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

Alternativ können Sie einen Smart-Listen-Trigger in Marketo Engage verwenden, um auf einen Milestone zu warten, z. B. eine Opportunity, die für die verwiesene Person erstellt wird.

Beispielziele:

* 10 verwiesene Besuche
* 5 empfohlene Anmeldungen
* 1 übermittelte Opportunity
* 2 Empfohlene E-Commerce-Käufe
* 5 Teilnehmer an empfohlenen Webinaren

1. Navigieren Sie **Marketing-Aktivitäten**.

   ![](assets/ma.png)

1. Wählen Sie das Empfehlungsangebot aus und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. Navigieren Sie im Empfehlungsangebotseditor zu **App-Einstellungen** > **Angebotsdetails**.

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. Wählen **unter** einen Ereignistyp aus der Dropdown-Liste **Erfüllungsziel** aus.

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>Wenn Sie den Flussschritt **Dem Referrer zuweisen** verwenden möchten, müssen Sie hier **Smart-Listen-Trigger** als Zieltyp für die Erfüllung auswählen.

* Weitergeleitete Besuche: Angebotsteilnehmer erhalten eine Gutschrift für jeden Besuch von einem Freund auf der Seite, auf der Ihr Angebot gehostet wird.
* Überwiesene Anmeldungen: Angebotsteilnehmer erhalten eine Gutschrift für jeden Freund, der sich für das Angebot anmeldet.
* Smart List Trigger: Angebotsteilnehmer erhalten eine Gutschrift für jeden Freund, der die Bedingungen eines [Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md)-Triggers in einer [Smart Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md) erfüllt. Sie können beispielsweise einen Trigger verwenden, der ausgelöst wird, wenn sich ein empfohlener Interessent für ein Webinar anmeldet.

* Benutzerdefiniertes JavaScript-Ereignis: Angebotsteilnehmer erhalten eine Gutschrift für jeden Trigger eines definierten JavaScript-Ereignisses auf Ihrer Seite. Siehe [Konvertierungsskript für benutzerdefinierte Ereignisse](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!NOTE]
>
>In Smart-Kampagnen stehen neue Filter und Trigger zur Überwachung sozialer Aktivitäten zur Verfügung. Siehe [Verwenden von Triggern und Filtern für soziale Aktivitäten](/help/marketo/product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md).

>[!MORELIKETHIS]
>
>Als Nächstes können Sie [die Anmelde- und Erfüllungs-E-Mails auswählen](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md) die Sie von Ihrem Empfehlungsangebot aus senden möchten.
