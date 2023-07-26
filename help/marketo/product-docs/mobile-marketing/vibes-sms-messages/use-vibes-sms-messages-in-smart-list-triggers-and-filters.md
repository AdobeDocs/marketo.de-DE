---
unique-page-id: 11378871
description: Verwenden von Video-SMS-Nachrichten in Triggern und Filtern mit intelligenter Liste - Marketo Docs - Produktdokumentation
title: Verwenden von Screens-SMS-Nachrichten in Triggern und Filtern mit Smart-Liste
exl-id: 9a629a39-fddc-4ec5-b1c5-d5053d676594
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Verwenden von Screens-SMS-Nachrichten in Triggern und Filtern mit Smart-Liste {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

Nach [Erstellen einer Vibes-SMS-Nachricht](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md)verwenden, sollten Sie Trigger und Filter mit Smart-Listen in einer Smart-Kampagne verwenden, um die Vorteile zu nutzen. So geht es.

1. Klicken Sie in My Marketo auf **Marketingaktivitäten**.

   ![](assets/image2016-7-28-9-3a48-3a32.png)

1. Wählen Sie eine Smart-Kampagne aus, in der Sie Ihr SMS-Asset verwenden möchten. Ziehen Sie über einen Trigger, z. B. die beliebte **Formular ausfüllen**.

   ![](assets/fills-out-form-pull-over.jpg)

## SMS-Trigger {#sms-triggers}

Es sind weitere SMS-Trigger verfügbar. Die SMS-Trigger werden nur angezeigt, wenn der Vibes-Dienst aktiviert ist.

![](assets/new-sms-search2.png)

Im Folgenden finden Sie einige Beispiele:

Der Trigger SMS-Nachrichten-Bounces löst einen Fluss aus, z. B. den Versand einer E-Mail, wenn eine SMS-Nachricht Bounces aufweist.

![](assets/sms-message-bounces-real.jpg)

Die **Abonniert die Vibes-Liste** Trigger löst einen Ablauf aus, wenn sich eine Person anmeldet.

![](assets/subscribes-to-vibes-list-real.jpg)

Die **Klicks Link in SMS-Nachricht** Trigger löst einen Fluss aus, wenn ein Besucher auf einen Link in der SMS klickt.

![](assets/clicks-link-in-sms-message.jpg)

## SMS-Filter {#sms-filters}

Sie können auch Vibes-Filter in Smart-Listen verwenden. Die **Abonnieren der Vibes-Liste** filter findet alle Personen, die *ever* abonniert Vibes. Dies umfasst sowohl abgemeldete als auch gelöschte Personen, auch wenn gelöschte Personen im Fluss weggelassen werden. Dieser Filter eignet sich am besten für Berichte.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

Im Gegensatz dazu wird die Variable **Mitglied der Vibes List** filter findet _everyone_ hat sich derzeit für Vibes angemeldet und eignet sich am besten für die Verwendung in Smart-Kampagnen oder Listen.

![](assets/image001.png)

>[!NOTE]
>
>Alle SMS-Filter enthalten **Datum der Aktivität** -Beschränkung standardmäßig.

Nachdem Sie die Video-Trigger und -Filter in Ihrer Smart-Liste eingerichtet haben, können Sie [Fluss definieren](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Definieren einer Smart-Liste für eine intelligente Kampagne | TRIGGER](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Suchen und Hinzufügen von Filtern zu einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
