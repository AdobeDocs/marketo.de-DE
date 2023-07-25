---
description: Dynamische Felder - Marketo-Dokumente - Produktdokumentation
title: Dynamische Felder
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 1%

---

# Dynamische Felder {#dynamic-fields}

Wir ermöglichen es Ihnen, Ihre E-Mail-Vorlagen mit vordefinierten Attributen wie `{{first_name}}` oder `{{company}}`. Mithilfe dieser Felder können Sie mehrere Kontakte per E-Mail versenden und diese Felder automatisch ausfüllen lassen, ohne sie für jeden Kontakt einzeln eingeben zu müssen.

>[!TIP]
>
>Die Felder &quot;first_name&quot;und &quot;company&quot;sind die einzigen Felder, die sowohl für Sales Insight-Aktionen als auch für Salesforce gelten. Das bedeutet, wenn ein Kontakt im [Webanwendung](https://toutapp.com/login), sehen wir uns in Salesforce an, ob wir einen Kontakt-/Lead-Datensatz mit einer entsprechenden E-Mail-Adresse finden können. Dann verwenden wir Informationen aus diesem Datensatz, um das Feld zu füllen.

## Dynamisches Feld in eine Vorlage einfügen {#insert-a-dynamic-field-into-a-template}

1. In **Vorlagen und Kampagnen**, suchen Sie die Vorlage, die Sie bearbeiten möchten, und klicken Sie auf **Vorlage bearbeiten**.

1. Klicken **Dynamisches Feld einfügen**.

   >[!NOTE]
   >
   >Wenn Sie Kontakte per E-Mail senden, die in Sales Insight-Aktionen vorhanden sind, können Sie die grundlegenden dynamischen Felder verwenden. Diese werden direkt vom Kontakt abgerufen.

Wenn Sie Kontakte per E-Mail versenden, die in Salesforce vorhanden sind, können Sie die dynamischen Felder von Salesforce nutzen. Diese beginnen alle mit &quot;sfdc&quot;. Solange Sie eine Verbindung zu Salesforce haben, rufen diese Felder direkt an den Lead/Kontakt in Salesforce auf, um Informationen in der Vorlage auszufüllen.

## Dynamische Felder in eine Betreffzeile einfügen {#insert-dynamic-fields-in-a-subject-line}

Kopieren Sie sie einfach manuell und fügen Sie sie in das Betrefffeld einer E-Mail ein. Achten Sie dabei darauf, dass Sie über die richtige Formatierung verfügen.

## Standardwerte für dynamische Felder {#dynamic-field-default-values}

Wenn Sie Ihren E-Mail-Vorlagen dynamische Felder hinzufügen, können Sie einen Standardwert hinzufügen, zu dem das dynamische Feld aufgelöst wird, wenn kein anderer Wert verfügbar ist.

Fügen Sie dazu &quot;|&quot;hinter der dynamischen Feldbeschriftung hinzu und fügen Sie dann &quot;default:&quot;hinzu (beides ohne Anführungszeichen). Fügen Sie dann den Wert hinzu, den das Feld auflösen soll (in Anführungszeichen gesetzt), wenn kein anderer Wert gefunden werden kann.

**Beispiel:**

`{{first name | default: "loyal customer"}}`

`{{sfdc_contact_account_name | default: "your company"}}`

## Glossar zu dynamischen Feldern {#dynamic-fields-glossary}

Wenn Sie eine Vorlage in Sales Insight-Aktionen erstellen, empfehlen wir immer, dynamische Felder mithilfe der Variablen **Dynamisches Feld einfügen** Schaltfläche.

Dieses Tool wird verwendet, um `auto-personalize your email` und sparen Ihnen unzählige Zeit `pulling information from the People page`.

| Dynamisches Feld | Anwendungsbeispiel für E-Mails |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Wenn du nicht noch einmal von mir hören willst, gib mir bitte hier Bescheid |
| `{{my_name}}` | Alan Bradley |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Senior Technical Writer |
| `{{work_website}}` | https://www.marketo.com |

**Was zu beachten ist**:

* Wenn die Informationen eines Kontakts falsch eingegeben wurden oder auf der Seite &quot;Personen&quot;fehlen, werden sie nicht korrekt in Ihre Vorlage übernommen.
* Der Unterschied zwischen `{{company}}` und `{{company_friendly}}` dass `{{company_friendly}}` wird jeden formalen Titel, wie z.B. Inc., LLC. etc., aus dem Namen Ihres Kontakts entfernen.
* Bei Verwendung von `{{company_friendly}}`, stellen Sie sicher, dass Sie Inc. oder Co. mit einem Komma in den Kontaktdaten trennen. So wissen Sales Insight-Aktionen, was beim Einziehen des Werts entfernt werden muss.
* Wir ermöglichen es Ihnen, Ihre E-Mail-Vorlagen mit vordefinierten Attributen wie `{{my_name}}` oder `{{my_title}}`. Diese Felder ermöglichen es Ihnen, sich schnell in Ihren E-Mail-Vorlagen zu referenzieren.

>[!TIP]
>
>Wenn Ihre dynamischen Felder nicht ausgefüllt werden, überprüfen Sie [diesem Artikel](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
