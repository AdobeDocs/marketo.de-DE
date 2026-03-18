---
description: Erfahren Sie, wie Sie das automatische Anhängen einer Abmeldenachricht für Verkaufs-E-Mails aktivieren oder deaktivieren.
title: Einstellung für automatisches Anhängen einer Abbestellungsnachricht
feature: Sales Insight Actions
exl-id: 17734f62-74e6-4168-a9c8-7835e3daf5ff
source-git-commit: 03f984d4049c119267c7b2c2baa4e68c7db34ad0
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 4%

---

# Einstellung für automatisches Anhängen einer Abbestellungsnachricht {#auto-append-unsubscribe-message-setting}

Stellen Sie sicher, dass jede gesendete E-Mail mit Insight-Verkaufsaktionen eine Abmelde-Nachricht enthält, damit Empfängerinnen und Empfänger die Möglichkeit haben, sich ganz einfach von der Kommunikation abzumelden. Wenn die Option Abo anhängen aktiviert ist, enthält die gesamte Kommunikation, die Ihr Team von Marketo Sales sendet, eine Abmelde-Nachricht, einschließlich E-Mails, die von der Web-Anwendung und Salesforce gesendet werden.

>[!NOTE]
>
>Wenn Sie das dynamische Feld `{{team_unsubscribe}}` in einer E-Mail-Vorlage verwenden und die Einstellung zum Anhängen von Abmeldenachrichten aktiviert ist, füllt das dynamische Feld Team-Abmeldung Ihre Abmeldenachricht auf _anstatt_ Abmeldenachricht anzuhängen.

## Append aktivieren/deaktivieren {#enable-disable-unsubscribe-append}

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **Einstellungen** aus.

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. Klicken Sie unter „Admin Settings“ auf **unsubscribes**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. Bewegen Sie den Schieberegler auf der Registerkarte Messaging unter Abmeldung anhängen in den gewünschten Status.

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>Wenn Sie die Einstellung „Nachricht anhängen - Abmelden“ deaktivieren, empfehlen wir, eine Fußzeile zum Abmelden zu Ihren Vorlagen hinzuzufügen, um sicherzustellen, dass Ihre Kommunikation über eine Opt-out-Option verfügt. Dazu können Sie jeder Vorlage Ihre eigene Nachricht hinzufügen oder das Feld `{{team_unsubscribe}}`Dynamisch[ ](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"}.
