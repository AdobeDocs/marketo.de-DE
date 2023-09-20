---
description: E-Mail-Vorlagen für Transaktionsumsätze - Marketo-Dokumente - Produktdokumentation
title: E-Mail-Vorlagen für Transaktionsumsätze
hide: true
hidefromtoc: true
feature: Marketo Sales Connect
source-git-commit: d6a3d95ed42d1c08d69014e1aa013e7436bd06c2
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# E-Mail-Vorlagen für Transaktionsumsätze {#transactional-sales-email-templates}

Wenn Ihr Team Transaktions- oder nicht kommerzielle E-Mails versendet, können Sie eine E-Mail-Vorlage als nicht kommerziell markieren, damit Abmeldungen umgangen werden können.

## Zu beachten {#things-to-note}

* Nicht-kommerzielle E-Mails umgehen die Abmeldungen von Verkäufen und [Marketo Engage unsubscribe check](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}, but will not bypass [blocked domains](/help/marketo/product-docs/marketo-sales-insight/actions/admin/blocked-domains.md){target="_blank"}.

* Abmelde-Nachrichten werden nicht automatisch an nicht kommerzielle E-Mails angehängt, auch wenn die [An die Admin-Einstellung für Abmelde-Nachrichten anhängen](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} is enabled. However, the `{{team_unsubscribe}}` [dynamic field](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"} wird weiterhin Ihre Team-Abmelde-Nachricht ausfüllen.

## E-Mail-Vorlage für nicht kommerzielle Verwendung konfigurieren {#configure-an-email-template-for-non-commercial-use}

1. Klicken Sie in der Kopfzeile auf **Vorlagen**.

PICC

1. Suchen Sie nach der Vorlage, die Sie aktualisieren möchten.

PICC

1. Wählen Sie die Vorlage aus.

PICC

1. Aktivieren Sie den Umschalter für nicht kommerzielle E-Mails unter Vorlageneinstellungen .

PICC

## Nicht kommerzielle E-Mail senden {#send-a-non-commercial-email}

Wenn eine abgemeldete Person ausgewählt wird, wird sie orange hervorgehoben.

1. Wählen Sie im Komprimierungsfenster die nicht kommerzielle Vorlage aus, die Sie sehen möchten.

PICC

1. Benutzer sehen ein Banner, das ihnen zeigt, dass sie derzeit eine nicht kommerzielle E-Mail-Vorlage ausgewählt haben.

PICC

1. Klicks **Senden**.

PICC

Die E-Mail wird auch dann gesendet, wenn sich die Person abgemeldet hat.
