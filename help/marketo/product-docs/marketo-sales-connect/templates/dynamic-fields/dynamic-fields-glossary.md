---
unique-page-id: 14352509
description: Glossar zu dynamischen Feldern - Marketo-Dokumente - Produktdokumentation
title: Glossar zu dynamischen Feldern
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '208'
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
* Wenn Sie die `{{my_signature}}` dynamisches Feld, hängt das System die Signatur des Benutzers nicht automatisch an, um Duplikate zu vermeiden.

>[!TIP]
>
>Sie können Ihre eigenen [Benutzerdefiniertes dynamisches Feld](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) für alles, was Sie automatisch in Ihre E-Mails gezogen haben möchten
