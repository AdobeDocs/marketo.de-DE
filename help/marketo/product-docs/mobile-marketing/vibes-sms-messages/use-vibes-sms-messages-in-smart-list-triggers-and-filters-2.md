---
description: Verwenden von Video-SMS-Nachrichten in Triggern und Filtern mit intelligenter Liste - Marketo Docs - Produktdokumentation
title: Verwenden von Screens-SMS-Nachrichten in Triggern und Filtern mit Smart-Liste
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: fee2d692acd8d54f2e308e2d5edc9876d13d5a4d
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Verwenden von Screens-SMS-Nachrichten in Triggern und Filtern mit Smart-Liste {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

Nachdem Sie [eine SMS-Nachricht vom Typ &quot;Video&quot;](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md){target="_blank"} erstellt haben, sollten Sie Trigger und Filter mit intelligenter Liste in einer Smart-Kampagne verwenden, um die Vorteile zu nutzen. So geht es.

1. Klicken Sie in My Marketo auf **Marketingaktivitäten**.

   ![](assets/use-vibes-sms-messages-in-smart-list-triggers-and-filters-1.png)

1. Wählen Sie eine Smart-Kampagne aus, in der Sie Ihre SMS-Assets verwenden möchten. Ziehen Sie über einen Trigger. In diesem Beispiel verwenden wir **Formular ausfüllen**.

   ![](assets/fills-out-form-pull-over.jpg)

## SMS-Trigger {#sms-triggers}

Es sind weitere SMS-Trigger verfügbar. Die SMS-Trigger werden nur angezeigt, wenn der Vibes-Dienst aktiviert ist.

SMS-NACHRICHTEN SENDEN:

* Marketingaktivitäten > Neue Smart-Kampagne auswählen
   * Smart List > Vibes List filter &amp; Korrekte Logik auswählen > Vibes list: Wählen Sie Liste aus der Dropdown-Liste aus (Liste der mobilen Datenbanken, die von der Vibes-Plattform synchronisiert werden).
      * Kann die Segmentierung verfeinern und SMS- und E-Mail-Filter und -Trigger innerhalb einer Kampagne nutzen
      * Vibes Filters: Abonnieren der Vibes-Liste oder Mitglied der Vibes-Liste - Logik ist konsistent mit E-Mail
         * Abonniert auf der Vibes-Liste - Teilnehmer, die sich für diese Vibes-Liste angemeldet haben, selbst wenn sie sich jetzt abgemeldet haben.  - wird hauptsächlich für kanalübergreifende Marketing-Maßnahmen verwendet.
            * Hinweis: Eine SMS-Nachricht wird an niemanden gesendet, der sich abgemeldet hat, wenn sie nicht in der Liste der mobilen Vibes-Datenbank enthalten ist.
         * Mitglied der Vibes List - aktiver, bestätigter Abonnent
         * Zu Liste hinzugefügt - Die Listen &quot;Besuche&quot;werden nicht mit diesem Filter aufgefüllt. Dies gilt für Marketo-Listen

![](assets/new-sms-search2.png)

Im Folgenden finden Sie einige Beispiele:

Der Trigger **SMS-Nachrichten-Bounces** löst einen Fluss aus, z. B. den Versand einer E-Mail, wenn eine SMS-Nachricht abspringt.

![](assets/sms-message-bounces-real.jpg)

Der Trigger **Abonniert die Vibes-Liste** löst einen Ablauf aus, wenn sich eine Person anmeldet.

![](assets/subscribes-to-vibes-list-real.jpg)

Der Trigger **Klicks auf Link in SMS-Nachricht** löst einen Fluss aus, wenn ein Benutzer auf einen Link in der SMS klickt.

![](assets/clicks-link-in-sms-message.jpg)

## SMS-Filter {#sms-filters}

Sie können auch Vibes-Filter in Smart-Listen verwenden. Der Filter **An die Liste der Segmente angemeldet** findet jeden, der *jemals* für Vibes angemeldet hat. Dies umfasst sowohl abgemeldete als auch gelöschte Personen, auch wenn gelöschte Personen im Fluss weggelassen werden. Dieser Filter eignet sich am besten für Berichte.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

Im Gegensatz dazu findet der Filter **Mitglied der Vibes-Liste** _jeder_ , der sich derzeit für Vibes angemeldet hat, und eignet sich am besten für die Verwendung in Smart-Kampagnen oder Listen.

![](assets/image001.png)

>[!NOTE]
>
>Alle SMS-Filter enthalten standardmäßig die Beschränkung **Datum der Aktivität** .

Nachdem Sie die Trigger und Filter &quot;Vibes&quot;in Ihrer Smart-Liste eingerichtet haben, können Sie [den Fluss definieren](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Definieren einer Smart-Liste für Smart-Campaign | Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Filter suchen und zu einer Smart-Liste hinzufügen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
