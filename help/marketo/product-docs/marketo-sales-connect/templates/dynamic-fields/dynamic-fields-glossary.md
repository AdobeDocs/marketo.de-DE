---
unique-page-id: 14352509
description: Glossar zu dynamischen Feldern - Marketo-Dokumente - Produktdokumentation
title: Glossar zu dynamischen Feldern
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: cffe7a8734f79f887f3aad017a16fad4f04cda74
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 1%

---

# Glossar zu dynamischen Feldern {#dynamic-fields-glossary}

Bei der Erstellung einer Vorlage in Sales Connect empfehlen wir immer, mithilfe der Schaltfläche **Dynamische Felder für MSE** dynamische Felder zu integrieren.

Dieses Tool wird für `auto-personalize your email` verwendet und speichert Ihnen die Tonnen Zeit bis `pulling information from the People page`.

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
* Der Unterschied zwischen `{{company}}` und `{{company_friendly}}` besteht darin, dass `{{company_friendly}}` jeden formalen Titel, wie z. B. Inc., LLC. usw., aus dem Namen des Unternehmens Ihres Kontakts entfernt.
* Stellen Sie bei Verwendung von `{{company_friendly}}` sicher, dass Sie in den Kontaktdetails Inc. oder Co. mit einem Komma trennen. So weiß Sales Connect, was beim Einziehen des Werts entfernt werden muss.
* Das System hängt die Signatur des Benutzers automatisch an jede gesendete E-Mail an. Wenn der Benutzer eine Vorlage mit dem dynamischen Feld `{{my_signature}}` verwendet, füllt das System die Signatur, in der das dynamische Feld `{{my_signature}}` platziert wurde. Es wird dort nur hinzugefügt, um Dopplungen zu vermeiden. Das System verarbeitet `{{team_unsubscribe}}` auf die gleiche Weise, wenn die globale Einstellung zum Abmelden von Anhängen aktiviert ist.

>[!TIP]
>
>Sie können für alles, was Sie automatisch in Ihre E-Mails gezogen haben möchten, ein eigenes dynamisches [Feld erstellen](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md)
