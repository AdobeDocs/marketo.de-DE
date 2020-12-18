---
unique-page-id: 14352509
description: Glossar "Dynamische Felder"- Marketing-Dokumente - Produktdokumentation
title: Glossar "Dynamische Felder"
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '173'
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
| `{{personal_email}}` | [[E-Mail-geschützt]](http://docs.marketo.com/cdn-cgi/l/email-protection) |
| `{{title}}` | Senior Technical Writer |
| `{{work_website}}` | https://www.marketo.com |

**Folgendes ist zu beachten**:

* Wenn ein Kontakt `information is entered incorrectly` oder auf der Seite &quot;Personen&quot;fehlt, wird `will not pull over correctly` in Ihre Vorlage eingefügt.

* Der Unterschied zwischen `{{company}}` und `{{company_friendly}}` besteht darin, dass `{{company_friendly}}` `remove any formal title` &lt;a3/>, z. B. Inc., LLC. usw., aus dem Namen der Firma Ihres Kontakts wird.
* Stellen Sie bei Verwendung von `{{company_friendly}}` sicher, dass Sie in den Kontaktdaten die Option &quot;Inc.&quot;oder &quot;Co.&quot;mit einem Komma trennen. So weiß Sales Connect, was entfernt werden muss, wenn der Wert eingezogen wird.

>[!TIP]
>
>Sie können Ihr eigenes dynamisches [benutzerdefiniertes Feld](http://docs.marketo.com/x/fADb) für alles erstellen, was Sie automatisch in Ihre E-Mails eingefügt haben möchten

