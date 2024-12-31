---
description: Einstellung für automatische Abmeldung - Marketo-Dokumente - Produktdokumentation
title: Einstellung für automatische Abmeldung
feature: Marketo Sales Connect
exl-id: 8aa75123-f6b5-4dfe-8fa7-f764620c04e8
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Einstellung für automatische Abmeldung {#auto-append-unsubscribe-message-setting}

Stellen Sie sicher, dass jede gesendete E-Mail eine Abmelde-Nachricht enthält, damit Empfängerinnen und Empfänger die Möglichkeit haben, sich einfach von der Kommunikation abzumelden. Wenn die Option Abmeldung anhängen aktiviert ist, enthält die gesamte Kommunikation, die Ihr Team von Marketo Sales sendet, eine Abmelde-Nachricht, einschließlich E-Mails, die von der Web-Anwendung, Salesforce, dem Gmail-Plug-in und dem Outlook-Plug-in gesendet wurden.

## Zu beachtende Punkte {#things-to-note}

* Bei E-Mails, die über die Plug-ins versendet werden, wird die Abmeldung nur angehängt, wenn eine Vorlage verwendet wird.

* Wenn Sie das dynamische Feld `{{team_unsubscribe}}` in einer E-Mail-Vorlage verwenden und die Einstellung zum Anhängen von Abmeldenachrichten aktiviert ist, füllt das dynamische Feld Team-Abmeldung Ihre Abmeldenachricht auf _anstatt_ Abmeldenachricht anzuhängen.

## Append aktivieren/deaktivieren {#enable-disable-unsubscribe-append}

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. Klicken Sie unter „Admin Settings“ auf **unsubscribes**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. Bewegen Sie den Schieberegler auf der Registerkarte Messaging unter Abmeldung anhängen in den gewünschten Status.

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>Wenn Sie die Einstellung „Nachricht anhängen - Abmelden“ deaktivieren, empfehlen wir, eine Fußzeile zum Abmelden zu Ihren Vorlagen hinzuzufügen, um sicherzustellen, dass Ihre Kommunikation über eine Opt-out-Option verfügt. Dazu können Sie jeder Vorlage Ihre eigene Nachricht hinzufügen oder das Feld `{{team_unsubscribe}}`Dynamisch[ ](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/dynamic-fields-glossary.md){target="_blank"}.
