---
description: Verwenden von Vibes-SMS-Nachrichten in Smart List-Triggern und -Filtern - Marketo-Dokumente - Produktdokumentation
title: Verwenden von Vibes-SMS-Nachrichten in Smart List-Triggern und -Filtern
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 1%

---

# Verwenden von Vibes-SMS-Nachrichten in Smart List-Triggern und -Filtern {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

Nach dem [Erstellen einer Vibes-SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md){target="_blank"} sollten Sie die Trigger und Filter der Smart List innerhalb einer Smart Campaign verwenden, um von den Vorteilen zu profitieren. So geht&#39;s.

1. Klicken Sie in My Marketo auf **[!UICONTROL Marketing-Aktivitäten]**.

   ![](assets/use-vibes-sms-messages-in-smart-list-triggers-and-filters-1.png)

1. Wählen Sie eine intelligente Kampagne aus, in der Sie Ihre SMS-Assets verwenden möchten. Ziehen Sie über einen Trigger. In diesem Beispiel verwenden wir **Formular ausfüllen**.

   ![](assets/fills-out-form-pull-over.jpg)

## SMS-Trigger {#sms-triggers}

Es stehen weitere SMS-Trigger zur Verfügung. Die SMS-Trigger werden nur angezeigt, wenn der Vibes-Service aktiviert ist.

SMS-NACHRICHT SENDEN:

* Marketing-Aktivitäten > Neue intelligente Kampagne auswählen
   * Smart List > Choose Vibes List filter &amp; Correct logic > Vibes list: Choose list from drop-down (Liste der mobilen Datenbanken, die von der Vibes-Plattform synchronisiert werden)
      * Kann die Segmentierung verfeinern und SMS- und E-Mail-Filter und -Trigger in einer Kampagne verwenden
      * Vibes-Filter: Abonnierte Vibes-Liste vs. Mitglied der Vibes-Liste - Logik stimmt mit E-Mail überein
         * Abonniert bei Vibes-Liste - Teilnehmer, die sich schon einmal für diese Vibes-Liste angemeldet haben, auch wenn sie sich jetzt abgemeldet haben.  - Wird hauptsächlich für Cross-Channel-Marketing-Maßnahmen verwendet
            * Hinweis: Eine SMS-Nachricht wird an niemanden gesendet, der sich abgemeldet hat, wenn er nicht in der Liste der Vibes Mobile-Datenbanken aufgeführt ist
         * Mitglied der Vibes-Liste - aktiver, bestätigter Abonnent
         * Zur Liste hinzugefügt - Vibes-Listen werden nicht mit diesem Filter befüllt. Dies ist für Marketo-Listen.

![](assets/new-sms-search2.png)

Im Folgenden finden Sie einige Beispiele:

Der **SMS-Nachrichten-Bounces**-Trigger initiiert einen Fluss, z. B. den Versand einer E-Mail, wenn eine SMS-Nachricht Bounces verursacht.

![](assets/sms-message-bounces-real.jpg)

Der **[!UICONTROL Abonniert die Vibes-Liste]**-Trigger initiiert einen Fluss, wenn eine Person ein Abonnement hat.

![](assets/subscribes-to-vibes-list-real.jpg)

Der Trigger **[!UICONTROL Klicks auf Link in SMS]** Nachricht initiiert einen Fluss, wenn eine Person auf einen Link in der SMS-Nachricht klickt.

![](assets/clicks-link-in-sms-message.jpg)

## SMS-Filter {#sms-filters}

Sie können auch Vibes-Filter in Smart-Listen verwenden. Der Filter **[!UICONTROL Abonnierte Vibes-Liste]** findet alle, die *jemals* Vibes abonniert haben. Dazu gehören sowohl abgemeldete als auch gelöschte Personen, auch wenn gelöschte Personen im Fluss weggelassen werden. Dieser Filter eignet sich am besten für das Reporting.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

Der Filter **Mitglied der Vibes-Liste** dagegen findet _alle_ derzeit bei Vibes abonniert und eignet sich am besten für die Verwendung in Smart-Kampagnen oder -Listen.

![](assets/image001.png)

>[!NOTE]
>
>Alle SMS-Filter enthalten standardmäßig **[!UICONTROL Einschränkung]** Datum der Aktivität“.

Nachdem Sie Vibes-Trigger und -Filter in Ihrer Smart-Liste eingerichtet haben, können Sie [Fluss definieren](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Definieren der Smart-Liste für intelligente Kampagnen | Trigger ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Filter suchen und zu einer Smart-Liste hinzufügen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
