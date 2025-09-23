---
description: Verwenden von SMS-Optionen in einer Smart-Kampagne - Marketo-Dokumente - Produktdokumentation
title: Verwenden von SMS-Optionen in einer intelligenten Kampagne
feature: Mobile Marketing
exl-id: 199b7cae-86d2-42fe-8934-10aa780f4454
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 7%

---

# Verwenden von SMS-Optionen in einer intelligenten Kampagne {#using-sms-options-in-a-smart-campaign}

Nachdem Sie [eine SMS-Nachricht erstellen](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"} sollten Sie die Trigger und Filter der Smart-Liste innerhalb einer Smart-Kampagne verwenden, um von den Vorteilen zu profitieren.

>[!NOTE]
>
>Wenn Sie eine SMS-Nachricht senden möchten, haben wir einen [ Artikel ](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"}.

>[!PREREQUISITES]
>
>SMS-Trigger/-Filter werden nur angezeigt, wenn [Vibes-Service aktiviert wurde](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md){target="_blank"}.

## SMS-Trigger {#sms-triggers}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-1.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-2.png"></td>
  </tr>
</table>

Im Folgenden finden Sie einige Beispiele:

Der **SMS-Nachrichten-Bounces**-Trigger initiiert einen Fluss, z. B. den Versand einer E-Mail, wenn eine SMS-Nachricht Bounces verursacht.

Der **Abonniert die Vibes-Liste**-Trigger initiiert einen Fluss, wenn eine Person ein Abonnement hat.

Der Trigger **Klicks auf Link in SMS** Nachricht initiiert einen Fluss, wenn eine Person auf einen Link in der SMS-Nachricht klickt.

## SMS-Filter {#sms-filters}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-3.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-4.png"></td>
  </tr>
</table>

Der Filter **Abonnierte Vibes-Liste** findet alle, die *jemals* Vibes abonniert haben. Dazu gehören sowohl abgemeldete als auch gelöschte Personen, auch wenn gelöschte Personen im Fluss weggelassen werden. Dieser Filter eignet sich am besten für das Reporting.

Der Filter **Mitglied der Vibes-Liste** dagegen findet *alle* derzeit bei Vibes abonniert und eignet sich am besten für die Verwendung in Smart-Kampagnen oder -Listen.

>[!NOTE]
>
>Alle SMS-Filter enthalten standardmäßig **Einschränkung** Datum der Aktivität“.

## SMS-Flussschritte {#sms-flow-steps}

Es gibt drei SMS-Flussschritte zur Auswahl.

![](assets/using-sms-options-in-a-smart-campaign-5.png)

<table>
<tbody>
  <tr>
    <td style="width:20%"><b>SMS-Nachricht senden</b></td>
    <td>Diese Flussaktion sendet Nachrichten an Personen aus der Smart-Liste von Marketo, die sich für eine Abonnement-Liste mit angemeldeten Benutzern von Vibes angemeldet haben. Der Anmeldevorgang wird nicht initiiert. <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md">Weitere Informationen</a>.</td>
  </tr>

<tr>
    <td style="width:20%"><b>Abonnement der Vibes-Liste</b></td>
    <td>Diese Flussaktion initiiert den SMS-Abonnementprozess über eine vom Benutzer ausgewählte Vibes-Akquise-Kampagne. Vibes sendet dann eine Bestätigungsnachricht, und der Empfänger muss innerhalb von 24 Stunden mit „Y“ antworten, um die Anmeldung zu bestätigen. Nachdem sich der Benutzer angemeldet hat, wird er Mitglied der zugehörigen Vibes-Abonnement-Liste.</td>
  </tr>
  <tr>
    <td style="width:20%"><b>Abbestelltes Abonnement der Vibes-Liste</b></td>
    <td>Mit dieser Flussaktion wird jede Person von einer Abonnement-Liste für angemeldete Benutzer abgemeldet. Wenn ein(e) Benutzende(r) „STOP“ zu Ihrem Code per SMS sendet, wird sein/ihr Personendatensatz aktualisiert, um anzugeben, dass er/sie nicht mehr zur Vibes-Abonnement-Liste gehört.</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>Die **Abonnieren einer Vibes-Liste** und **Abmelden von einer Vibes-Liste** haben unterschiedliche Anforderungen. Für **Abonnieren** müssen Sie die Vibes-Liste und die Vibes-Akquise-Kampagne auswählen. Für **Abmelden** ist nur die Liste Vibes erforderlich.

>[!MORELIKETHIS]
>
>* [Senden einer SMS-Nachricht](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"}
>* [Definieren der Smart-Liste für intelligente Kampagnen | Trigger ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
>* [Definieren der Smart-Liste für intelligente Kampagnen | Batch](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}
