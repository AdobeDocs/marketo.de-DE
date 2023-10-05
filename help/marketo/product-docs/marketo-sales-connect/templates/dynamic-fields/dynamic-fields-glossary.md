---
unique-page-id: 14352509
description: Glossar zu dynamischen Feldern - Marketo-Dokumente - Produktdokumentation
title: Glossar zu dynamischen Feldern
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: cffe7a8734f79f887f3aad017a16fad4f04cda74
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 1%

---

# Glossar zu dynamischen Feldern {#dynamic-fields-glossary}

Bei der Erstellung einer Vorlage in Sales Connect empfehlen wir immer, dynamische Felder mithilfe der **Dynamische MSE-Felder** Schaltfläche.

Mit diesem Tool wird `auto-personalize your email` und sparen Ihnen unzählige Zeit `pulling information from the People page`.

| Dynamisches Feld | Anwendungsbeispiel für E-Mails |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | Wenn Sie keine E-Mails mehr von uns erhalten möchten, klicken Sie hier . |
| `{{friendly_unsubscribe}}` | Müde von allen E-Mails? Bitte lassen Sie es hier wissen |
| `{{my_name}}` | Keith Flynn |
| `{{my_signature}}` | Keith Flynn, Senior Technical Writer - Adobe |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Senior Technical Writer |
| `{{work_website}}` | https://www.adobe.com |

**Was zu beachten ist**:

* Wenn die Informationen eines Kontakts falsch eingegeben wurden oder auf der Seite &quot;Personen&quot;fehlen, werden sie nicht korrekt in Ihre Vorlage übernommen.
* Der Unterschied zwischen `{{company}}` und `{{company_friendly}}` dass `{{company_friendly}}` wird jeden formalen Titel, wie z.B. Inc., LLC. etc., aus dem Namen Ihres Kontakts entfernen.
* Bei Verwendung von `{{company_friendly}}`, stellen Sie sicher, dass Sie Inc. oder Co. mit einem Komma in den Kontaktdaten trennen. So weiß Sales Connect, was beim Einziehen des Werts entfernt werden muss.
* Das System hängt die Signatur des Benutzers automatisch an jede gesendete E-Mail an. Wenn der Benutzer eine Vorlage mit der Variablen `{{my_signature}}` dynamisches Feld, füllt das System die Signatur, in der die `{{my_signature}}` das dynamische Feld platziert wurde. Es wird dort nur hinzugefügt, um Dopplungen zu vermeiden. Das System verarbeitet `{{team_unsubscribe}}` auf die gleiche Weise wie bei Aktivierung der globalen Einstellung zum Abmelden von Anhängen .

>[!TIP]
>
>Sie können Ihre eigenen [Benutzerdefiniertes dynamisches Feld](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) für alles, was Sie automatisch in Ihre E-Mails gezogen haben möchten
