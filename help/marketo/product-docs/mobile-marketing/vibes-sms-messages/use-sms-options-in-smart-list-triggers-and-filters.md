---
description: Verwenden von SMS-Optionen in Triggern und Filtern mit intelligenter Liste - Marketo-Dokumente - Produktdokumentation
title: Verwenden von SMS-Optionen in Smart List-Triggern und -Filtern
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 8e56b571a34451d6b0436dc041efaf0fd575db36
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Verwenden von SMS-Optionen in Smart List-Triggern und -Filtern {#use-sms-options-in-smart-list-triggers-and-filters}

NEUES DOC

Nach [SMS erstellen](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}verwenden, sollten Sie Smart-List-Trigger und -Filter in einer Smart-Kampagne verwenden, um die Vorteile zu nutzen.

>[!PREREQUISITES]
>
>SMS-Trigger/-Filter werden nur angezeigt, wenn die Variable [Der Dienst &quot;Vibes&quot;wurde aktiviert](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md).

## SMS-Trigger {#sms-triggers}

<table>
  <tr>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-1.png"></td>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-2.png"></td>
  </tr>
</table>

Im Folgenden finden Sie einige Beispiele:

Die **SMS-Nachrichtenabsprünge** Trigger startet einen Fluss, z. B. das Senden einer E-Mail, wenn eine SMS-Nachricht abbricht.

Die **Abonniert die Vibes-Liste** Trigger löst einen Ablauf aus, wenn sich eine Person anmeldet.

Die **Klicks Link in SMS-Nachricht** Trigger löst einen Fluss aus, wenn ein Besucher auf einen Link in der SMS klickt.

## SMS-Filter {#sms-filters}

<table>
  <tr>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-3.png"></td>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-4.png"></td>
  </tr>
</table>

Sie können auch Filter &quot;Vibes&quot;in Smart-Listen verwenden. Die **Abonnieren der Vibes-Liste** filter findet alle Personen, die *ever* abonniert Vibes. Dies umfasst sowohl abgemeldete als auch gelöschte Personen, auch wenn gelöschte Personen im Fluss weggelassen werden. Dieser Filter eignet sich am besten für Berichte.

Im Gegensatz dazu wird die Variable **Mitglied der Vibes List** filter findet _everyone_ hat sich derzeit für Vibes angemeldet und eignet sich am besten für die Verwendung in Smart-Kampagnen oder -Listen.

>[!NOTE]
>
>Alle SMS-Filter enthalten **Datum der Aktivität** -Beschränkung standardmäßig.

Nachdem Sie die Video-Trigger und -Filter in Ihrer Smart-Liste eingerichtet haben, können Sie [Fluss definieren](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [SMS-Nachricht senden](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md)
>* [Definieren einer Smart-Liste für eine intelligente Kampagne | TRIGGER](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Suchen und Hinzufügen von Filtern zu einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
