---
description: Einstellung zum automatischen Anhängen von Abmelde-Nachrichten - Marketo Docs - Produktdokumentation
title: Einstellung zum automatischen Anhängen von Abmelde-Nachrichten
hide: true
hidefromtoc: true
feature: Marketo Sales Connect
source-git-commit: b0f62abfe04efd8e72ed8e92442d4a46ea118f33
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Einstellung zum automatischen Anhängen von Abmelde-Nachrichten {#auto-append-unsubscribe-message-setting}

Stellen Sie sicher, dass jede gesendete E-Mail eine Abmelde-Nachricht enthält, damit die Empfänger die Möglichkeit haben, sich von der Kommunikation abzumelden. Wenn die Abmelde-Nachricht angehängt ist, enthält die gesamte Kommunikation, die Ihr Team von Marketo Sales sendet, eine Abmelde-Nachricht, einschließlich der von der Webanwendung gesendeten E-Mails, Salesforce, dem Gmail-Plug-in und dem Outlook-Plugin.

## Zu beachten {#things-to-note}

* Bei E-Mails, die von den Plug-ins gesendet werden, wird die Abmeldung nur angehängt, wenn eine Vorlage verwendet wird.

* Wenn Sie die `{{team_unsubscribe}}` dynamisches Feld in einer E-Mail-Vorlage verwenden und die Einstellung zum Anhängen von Abmeldungen aktiviert ist, füllt das dynamische Feld zum Abmelden Ihre Abmelde-Nachricht aus. _anstelle von_ an Ihre Abmelde-Nachricht anhängen.

## Append aktivieren/deaktivieren {#enable-disable-unsubscribe-append}

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **Einstellungen**.

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. Klicken Sie unter &quot;Admin Settings&quot;auf **Abmeldungen**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. Verschieben Sie auf der Registerkarte Messaging unter Unsubscribe-Nachricht anhängen den Regler in den gewünschten Status.

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>Wenn Sie die Einstellung zum Abmelden von Nachrichten anhängen deaktivieren, empfehlen wir, Ihren Vorlagen eine Abmelde-Fußzeile hinzuzufügen, um sicherzustellen, dass Ihre Kommunikation über eine Abmeldeoption verfügt. Sie können dazu Ihre eigene benutzerdefinierte Nachricht zu jeder Vorlage hinzufügen oder die `{{team_unsubscribe}}` dynamisches Feld.
