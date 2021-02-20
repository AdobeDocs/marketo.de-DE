---
unique-page-id: 11378871
description: Verwenden von Vibes SMS-Nachrichten in Triggern und Filtern mit intelligenter Liste - Marketing Docs - Produktdokumentation
title: Verwenden von Vibes-SMS-Nachrichten in Triggern und Filtern mit intelligenter Liste
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---


# Verwenden von Vibes-SMS-Nachrichten in Triggern und Filtern mit intelligenter Liste {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

Nachdem Sie [eine Vibes-SMS-Nachricht ](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md) erstellt haben, sollten Sie intelligente Liste-Trigger und Filter in einer intelligenten Kampagne verwenden, um die Vorteile zu erhalten. So geht es.

1. Klicken Sie in &quot;My Marketo&quot;auf **Marketing-Aktivitäten**.

   ![](assets/image2016-7-28-9-3a48-3a32.png)

1. Wählen Sie eine intelligente Kampagne aus, in der Sie Ihr SMS-Asset verwenden möchten. Ziehen Sie den Mauszeiger über einen Trigger, z. B. das beliebte Formular **Ausfüllen**.

   ![](assets/fills-out-form-pull-over.jpg)

## SMS-Trigger {#sms-triggers}

Es sind weitere SMS-Trigger verfügbar. Die SMS-Trigger werden nur angezeigt, wenn der Dienst Vibes aktiviert ist.

![](assets/new-sms-search2.png)

Im Folgenden finden Sie einige Beispiele:

Der Trigger &quot;SMS-Absprünge&quot;löst einen Fluss aus, z. B. das Senden einer E-Mail, wenn eine SMS-Nachricht abspringt.

![](assets/sms-message-bounces-real.jpg)

Der Trigger **Abonniert die Vibes-Liste** ruft einen Fluss auf, wenn eine Person abonniert.

![](assets/subscribes-to-vibes-list-real.jpg)

Der Trigger **Klickt auf Link in der SMS-Nachricht** löst einen Textfluss aus, wenn eine Person auf einen Link in der SMS klickt.

![](assets/clicks-link-in-sms-message.jpg)

## SMS-Filter {#sms-filters}

Sie können auch Vibes-Filter in intelligenten Listen verwenden. Der Filter **Abonniert bei der Vibes-Liste** findet jeden, der *jemals* abonniert hat. Dies umfasst sowohl abonnierte als auch gelöschte Personen, auch wenn gelöschte Personen aus dem Fluss ausgelassen werden. Dieser Filter eignet sich am besten zum Berichte.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

Im Gegensatz dazu findet der Filter **Member of Vibes Liste** _jedermann_, der zurzeit Vibes abonniert hat, und ist am besten für die Verwendung in Smart-Kampagnen oder -Listen geeignet.

![](assets/image001.png)

>[!NOTE]
>
>Alle SMS-Filter enthalten standardmäßig die Beschränkung **Datum der Aktivität**.

Nachdem Sie in Ihrer Smart-Liste Vibes-Trigger und -Filter eingerichtet haben, können Sie [den Fluss](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md) definieren.

>[!MORELIKETHIS]
>
>* [Intelligente Liste für intelligente Kampagne definieren | Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Filter für eine intelligente Liste suchen und Hinzufügen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)

