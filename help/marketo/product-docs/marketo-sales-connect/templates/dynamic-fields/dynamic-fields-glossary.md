---
unique-page-id: 14352509
description: Glossar "Dynamische Felder"- Marketing-Dokumente - Produktdokumentation
title: Glossar "Dynamische Felder"
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Glossar für dynamische Felder {#dynamic-fields-glossary}

Beim Erstellen einer Vorlage in Sales Connect empfehlen wir immer, dynamische Felder mithilfe der Schaltfläche **MSE Dynamische Felder** zu integrieren.

Dieses Tool wird verwendet, um `auto-personalize your email` und sparen Sie Tonnen Zeit durch `pulling information from the People page`.

| Dynamisches Feld | Beispiel für die E-Mail |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Wenn du nicht noch einmal von mir hören willst, gib mir bitte hier Bescheid |
| `{{my_name}}` | Alan Bradley |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Senior Technical Writer |
| `{{work_website}}` | https://www.marketo.com |

**Folgendes ist zu beachten**:

* Wenn die Informationen eines Kontakts falsch eingegeben wurden oder auf der Seite &quot;Personen&quot;fehlen, werden sie nicht korrekt in Ihre Vorlage übernommen.
* Der Unterschied zwischen `{{company}}` und `{{company_friendly}}` besteht darin, dass `{{company_friendly}}` alle formalen Titel, wie z.B. Inc., LLC. usw., aus dem Namen der Firma Ihres Kontakts entfernen wird.
* Stellen Sie bei Verwendung von `{{company_friendly}}` sicher, dass Sie in den Kontaktdaten die Option &quot;Inc.&quot;oder &quot;Co.&quot;mit einem Komma trennen. So weiß Sales Connect, was entfernt werden muss, wenn der Wert eingezogen wird.

>[!TIP]
>
>Sie können Ihr eigenes dynamisches [benutzerdefiniertes Feld](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) für alles erstellen, was Sie automatisch in Ihre E-Mails eingefügt haben möchten
