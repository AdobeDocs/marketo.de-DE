---
description: Einstellung zum automatischen Anhängen von Abmelde-Nachrichten - Marketo Docs - Produktdokumentation
title: Einstellung zum automatischen Anhängen von Abmelde-Nachrichten
feature: Marketo Sales Connect
exl-id: 8aa75123-f6b5-4dfe-8fa7-f764620c04e8
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Einstellung zum automatischen Anhängen von Abmelde-Nachrichten {#auto-append-unsubscribe-message-setting}

Stellen Sie sicher, dass jede gesendete E-Mail eine Abmelde-Nachricht enthält, damit die Empfänger die Möglichkeit haben, sich von der Kommunikation abzumelden. Wenn die Abmelde-Nachricht angehängt ist, enthält die gesamte Kommunikation, die Ihr Team von Marketo Sales sendet, eine Abmelde-Nachricht, einschließlich der von der Webanwendung gesendeten E-Mails, Salesforce, dem Gmail-Plug-in und dem Outlook-Plugin.

## Zu beachten {#things-to-note}

* Bei E-Mails, die von den Plug-ins gesendet werden, wird die Abmeldung nur angehängt, wenn eine Vorlage verwendet wird.

* Wenn Sie das dynamische Feld `{{team_unsubscribe}}` in einer E-Mail-Vorlage verwenden und die Einstellung zum Anhängen der Abmelde-Nachricht aktiviert ist, füllt das dynamische Feld zum Abmelden von Nachrichten das Feld zum Abmelden von Nachrichten _anstelle von_ aus, um Ihre Abmelde-Nachricht anzuhängen.

## Append aktivieren/deaktivieren {#enable-disable-unsubscribe-append}

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. Klicken Sie unter &quot;Admin Settings&quot;auf **Unsubscribes**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. Verschieben Sie auf der Registerkarte Messaging unter Unsubscribe-Nachricht anhängen den Regler in den gewünschten Status.

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>Wenn Sie die Einstellung zum Abmelden von Nachrichten anhängen deaktivieren, empfehlen wir, Ihren Vorlagen eine Abmelde-Fußzeile hinzuzufügen, um sicherzustellen, dass Ihre Kommunikation über eine Abmeldeoption verfügt. Fügen Sie dazu Ihre eigene benutzerdefinierte Nachricht zu jeder Vorlage hinzu oder verwenden Sie das dynamische Feld `{{team_unsubscribe}}` [2}.](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/dynamic-fields-glossary.md){target="_blank"}
