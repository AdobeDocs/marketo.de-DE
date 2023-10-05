---
description: E-Mail-Vorlagen für Transaktionsumsätze - Marketo-Dokumente - Produktdokumentation
title: E-Mail-Vorlagen für Transaktionsumsätze
feature: Marketo Sales Connect
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---

# E-Mail-Vorlagen für Transaktionsumsätze {#transactional-sales-email-templates}

Wenn Ihr Team Transaktions- oder nicht kommerzielle E-Mails versendet, können Sie eine E-Mail-Vorlage als nicht kommerziell markieren, damit Abmeldungen umgangen werden können.

## Zu beachten {#things-to-note}

* Nicht-kommerzielle E-Mails umgehen die Abmeldungen von Verkäufen und [Marketo Engage unsubscribe check](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}, but will not bypass [blocked domains](/help/marketo/product-docs/marketo-sales-connect/admin/blocked-domains.md){target="_blank"}.

* Abmelde-Nachrichten werden nicht automatisch an nicht kommerzielle E-Mails angehängt, auch wenn die [An die Admin-Einstellung für Abmelde-Nachrichten anhängen](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} is enabled. However, the `{{team_unsubscribe}}` [dynamic field](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/dynamic-fields-glossary.md){target="_blank"} wird weiterhin Ihre Team-Abmelde-Nachricht ausfüllen.

## E-Mail-Vorlage für nicht kommerzielle Verwendung konfigurieren {#configure-an-email-template-for-non-commercial-use}

1. Klicken Sie in der Kopfzeile auf **Vorlagen**.

   ![](assets/transactional-sales-email-templates-1.png)

1. Wählen Sie die zu aktualisierende Vorlage aus.

   ![](assets/transactional-sales-email-templates-2.png)

1. Aktivieren Sie den Umschalter für nicht kommerzielle E-Mails unter Vorlageneinstellungen .

   ![](assets/transactional-sales-email-templates-3.png)

## Nicht kommerzielle E-Mail senden {#send-a-non-commercial-email}

>[!NOTE]
>
>Wenn eine abgemeldete Person ausgewählt wird, wird sie orange hervorgehoben.

1. Klicken Sie in der Kopfzeile auf **Erstellen**. Wählen Sie die gewünschte nicht kommerzielle Vorlage aus.

   ![](assets/transactional-sales-email-templates-4.png)

1. Benutzer sehen ein Banner, das ihnen zeigt, dass sie eine nicht kommerzielle E-Mail-Vorlage ausgewählt haben.

   ![](assets/transactional-sales-email-templates-5.png)

1. Klicks **Senden**.

   ![](assets/transactional-sales-email-templates-6.png)

Die E-Mail wird auch dann gesendet, wenn sich die Person abgemeldet hat.
