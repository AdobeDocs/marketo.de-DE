---
description: E-Mail-Vorlagen für Transaktionsumsätze - Marketo-Dokumente - Produktdokumentation
title: E-Mail-Vorlagen für Transaktionsumsätze
hide: true
hidefromtoc: true
feature: Sales Insight Actions
source-git-commit: f11e455196cdfb7a6c1054df40344cab5b06772b
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# E-Mail-Vorlagen für Transaktionsumsätze {#transactional-sales-email-templates}

Wenn Ihr Team Transaktions- oder nicht kommerzielle E-Mails versendet, können Sie eine E-Mail-Vorlage als nicht kommerziell markieren, damit Abmeldungen umgangen werden können.

## Zu beachten {#things-to-note}

* Nicht-kommerzielle E-Mails umgehen die Abmeldungen von Verkäufen und [Marketo Engage unsubscribe check](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}, but will not bypass [blocked domains](/help/marketo/product-docs/marketo-sales-insight/actions/admin/blocked-domains.md){target="_blank"}.

* Abmelde-Nachrichten werden nicht automatisch an nicht kommerzielle E-Mails angehängt, auch wenn die [An die Admin-Einstellung für Abmelde-Nachrichten anhängen](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} is enabled. However, the `{{team_unsubscribe}}`[dynamic field](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"} wird weiterhin Ihre Team-Abmelde-Nachricht ausfüllen.

## E-Mail-Vorlage für nicht kommerzielle Verwendung konfigurieren {#configure-an-email-template-for-non-commercial-use}

Navigieren Sie zum Abschnitt Vorlage .

Suchen Sie nach der Vorlage, die Sie aktualisieren möchten.

Wählen Sie die Vorlage aus.

Aktivieren Sie den Umschalter für nicht kommerzielle E-Mails unter Vorlageneinstellungen .

Nicht kommerzielle E-Mail senden

Wenn eine abgemeldete Person ausgewählt wird, wird sie orange hervorgehoben.

Wählen Sie im Komprimierungsfenster die nicht kommerzielle Vorlage aus, die Sie sehen möchten.

Benutzer sehen ein Banner, das ihnen zeigt, dass sie derzeit eine nicht kommerzielle E-Mail-Vorlage ausgewählt haben.

Klicken Sie auf Senden und die E-Mail wird weiterhin gesendet, auch wenn sich die Person abgemeldet hat.
