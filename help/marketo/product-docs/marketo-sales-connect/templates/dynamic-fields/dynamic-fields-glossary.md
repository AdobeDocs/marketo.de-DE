---
unique-page-id: 14352509
description: Glossar für dynamische Felder - Marketo-Dokumente - Produktdokumentation
title: Glossar für dynamische Felder
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: cffe7a8734f79f887f3aad017a16fad4f04cda74
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 2%

---

# Glossar für dynamische Felder {#dynamic-fields-glossary}

Beim Erstellen einer Vorlage in Sales Connect empfehlen wir immer die Integration dynamischer Felder mithilfe der Schaltfläche **MSE Dynamic Fields**.

Dieses Tool wird verwendet, um Ihnen `pulling information from the People page` viel Zeit zu `auto-personalize your email` und zu sparen.

| Dynamisches Feld | Beispiel für das, was in Ihrer E-Mail angezeigt wird |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | Wenn Sie keine E-Mails mehr von uns erhalten möchten, klicken Sie hier |
| `{{friendly_unsubscribe}}` | Müde von all den E-Mails? Bitte lass es mich hier wissen |
| `{{my_name}}` | Keith Flynn |
| `{{my_signature}}` | Keith Flynn, Senior Technical Writer - Adobe |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | leitender technischer Redakteur |
| `{{work_website}}` | https://www.adobe.com |

**Zu beachten**:

* Wenn die Kontaktinformationen falsch eingegeben wurden oder auf der Seite Personen fehlen, werden sie nicht korrekt in Ihre Vorlage übernommen.
* Der Unterschied zwischen `{{company}}` und `{{company_friendly}}` besteht darin, dass `{{company_friendly}}` alle formalen Titel, wie Inc., LLC. usw., aus dem Namen des Unternehmens Ihres Kontakts entfernen.
* Wenn Sie `{{company_friendly}}` verwenden, stellen Sie sicher, dass Sie Inc. oder Co. durch ein Komma in den Kontaktdaten trennen. So weiß Sales Connect, was beim Abrufen des Werts entfernt werden soll.
* Das System hängt die Signatur des Benutzers automatisch an jede gesendete E-Mail an. Wenn der/die Benutzende eine Vorlage mit dem dynamischen Feld `{{my_signature}}` verwendet, füllt das System die Signatur, in der das dynamische Feld `{{my_signature}}` platziert wurde. Er wird nur hinzugefügt, um Duplizierungen zu vermeiden. Das System handhabt `{{team_unsubscribe}}` auf dieselbe Weise, wenn die globale Einstellung zum Abmelden vom Append aktiviert ist.

>[!TIP]
>
>Sie können Ihr eigenes [benutzerdefiniertes dynamisches Feld](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) für alles erstellen, was Sie automatisch in Ihre E-Mails übertragen möchten
