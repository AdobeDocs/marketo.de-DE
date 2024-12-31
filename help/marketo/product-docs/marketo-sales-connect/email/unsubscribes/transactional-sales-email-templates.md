---
description: E-Mail-Vorlagen für Transaktionsverkäufe - Marketo-Dokumente - Produktdokumentation
title: E-Mail-Vorlagen für Transaktionsverkäufe
feature: Marketo Sales Connect
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 1%

---

# E-Mail-Vorlagen für Transaktionsverkäufe {#transactional-sales-email-templates}

Wenn Ihr Team Transaktions- oder nicht-kommerzielle E-Mails versendet, können Sie eine E-Mail-Vorlage als nicht-kommerziell markieren, damit Abmeldungen umgangen werden können.

## Zu beachtende Punkte {#things-to-note}

* Nicht-kommerzielle E-Mails umgehen die Abmeldungen von Verkäufen und den [Marketo Engage-Abmelde-Check](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}, umgehen jedoch nicht [blockierte Domains](/help/marketo/product-docs/marketo-sales-connect/admin/blocked-domains.md){target="_blank"}.

* Abmelde-Nachrichten werden nicht automatisch an nicht-kommerzielle E-Mails angehängt, auch wenn die [Admin zum Abmelden von Nachrichten anhängen](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} aktiviert ist. Das Feld `{{team_unsubscribe}}`Dynamisch[ füllt jedoch weiterhin ](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/dynamic-fields-glossary.md){target="_blank"} Nachricht zur Abmeldung Ihres Teams auf.

## Konfigurieren einer E-Mail-Vorlage für die nicht-kommerzielle Verwendung {#configure-an-email-template-for-non-commercial-use}

1. Klicken Sie in der Kopfzeile auf **Vorlagen**.

   ![](assets/transactional-sales-email-templates-1.png)

1. Suchen Sie die Vorlage, die Sie aktualisieren möchten, und wählen Sie sie aus.

   ![](assets/transactional-sales-email-templates-2.png)

1. Aktivieren Sie unter Vorlageneinstellungen den Umschalter Nicht-kommerzielle E-Mail .

   ![](assets/transactional-sales-email-templates-3.png)

## Senden einer nicht-kommerziellen E-Mail {#send-a-non-commercial-email}

>[!NOTE]
>
>Wenn eine abgemeldete Person ausgewählt wird, wird sie orange hervorgehoben.

1. Klicken Sie in der Kopfzeile auf **Erstellen**. Suchen Sie die gewünschte nicht-kommerzielle Vorlage und wählen Sie sie aus.

   ![](assets/transactional-sales-email-templates-4.png)

1. Benutzende sehen ein Banner, das ihnen zeigt, dass sie eine nicht-kommerzielle E-Mail-Vorlage ausgewählt haben.

   ![](assets/transactional-sales-email-templates-5.png)

1. Klicken Sie auf **Senden**.

   ![](assets/transactional-sales-email-templates-6.png)

Die E-Mail wird auch dann gesendet, wenn die Person das Abonnement gekündigt hat.
