---
description: Dynamische Felder - Marketo-Dokumente - Produktdokumentation
title: Dynamische Felder
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 1%

---

# Dynamische Felder {#dynamic-fields}

Wir ermöglichen es Ihnen, Ihre E-Mail-Vorlagen mit vordefinierten Attributen wie `{{first_name}}` oder `{{company}}` zu personalisieren. Mit diesen Feldern können Sie mehrere Kontakte per E-Mail versenden und diese Felder automatisch ausfüllen, ohne sie für jeden Kontakt separat eingeben zu müssen.

>[!TIP]
>
>Die Felder „first_name“ und „company“ sind die einzigen Felder, die sowohl an [!DNL Sales Insight Actions] als auch an [!DNL Salesforce] gerichtet sind. Wenn also in der [Web-Anwendung](https://toutapp.com/login) kein Kontakt vorhanden ist, überprüfen wir [!DNL Salesforce], ob wir einen Kontakt-/Lead-Datensatz mit einer entsprechenden E-Mail-Adresse finden können. Anschließend verwenden wir Informationen aus diesem Datensatz, um das Feld auszufüllen.

## Einfügen eines dynamischen Felds in eine Vorlage {#insert-a-dynamic-field-into-a-template}

1. Suchen **[!UICONTROL unter „Vorlagen und Kampagnen]** die Vorlage, die Sie bearbeiten möchten, und klicken Sie auf **[!UICONTROL Vorlage bearbeiten]**.

1. Klicken Sie **[!UICONTROL Dynamisches Feld einfügen]**.

   >[!NOTE]
   >
   >Beim Senden von E-Mails an Kontakte, die in [!DNL Sales Insight Actions] vorhanden sind, können Sie die grundlegenden dynamischen Felder verwenden. Diese ziehen direkt aus dem Kontakt.

Wenn Sie Kontakte per E-Mail versenden, die bereits in [!DNL Salesforce] vorhanden sind, können Sie die [!DNL Salesforce] dynamischen Felder nutzen. Diese beginnen alle mit „sfdc“. Sofern Sie über eine Verbindung zu [!DNL Salesforce] verfügen, werden diese Felder direkt den Lead/Kontakt aufrufen, [!DNL Salesforce] Informationen in der Vorlage auszufüllen.

## Dynamische Felder in eine Betreffzeile einfügen {#insert-dynamic-fields-in-a-subject-line}

Kopieren Sie sie einfach manuell und fügen Sie sie im Betrefffeld einer E-Mail ein. Achten Sie dabei darauf, dass die korrekte Formatierung gewährleistet ist.

## Standardwerte für dynamische Felder {#dynamic-field-default-values}

Beim Hinzufügen dynamischer Felder zu Ihren E-Mail-Vorlagen können Sie einen Standardwert hinzufügen, den das dynamische Feld auflöst, wenn kein anderer Wert verfügbar ist.

Fügen Sie dazu &quot;|&quot; nach der dynamischen Feldbezeichnung und dann „Standard:“ hinzu (beide ohne Anführungszeichen). Fügen Sie dann den Wert hinzu, zu dem das Feld aufgelöst werden soll (in Anführungszeichen eingeschlossen), wenn kein anderer Wert gefunden werden kann.

**Beispiel:**

`{{first name | default: "loyal customer"}}`

`{{sfdc_contact_account_name | default: "your company"}}`

## Glossar für dynamische Felder {#dynamic-fields-glossary}

Beim Erstellen einer Vorlage in [!DNL Sales Insight Actions] empfehlen wir immer die Integration dynamischer Felder mithilfe der Schaltfläche **[!UICONTROL Dynamisches Feld einfügen]**.

Dieses Tool wird verwendet, um Ihnen `auto-personalize your email` viel Zeit zu `pulling information from the People page` und zu sparen.

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
* Wenn Sie `{{company_friendly}}` verwenden, stellen Sie sicher, dass Sie Inc. oder Co. durch ein Komma in den Kontaktdaten trennen. So weiß [!DNL Sales Insight Actions], was beim Abrufen des Werts entfernt werden soll.
* Wir ermöglichen es Ihnen, Ihre E-Mail-Vorlagen mit vordefinierten Attributen wie `{{my_name}}` oder `{{my_title}}` zu personalisieren. Mit diesen Feldern können Sie schnell auf sich selbst in Ihren E-Mail-Vorlagen verweisen.
* Das System hängt die Signatur des Benutzers automatisch an jede gesendete E-Mail an. Wenn der/die Benutzende eine Vorlage mit dem dynamischen Feld `{{my_signature}}` verwendet, füllt das System die Signatur, in der das dynamische Feld `{{my_signature}}` platziert wurde. Er wird nur hinzugefügt, um Duplizierungen zu vermeiden. Das System handhabt `{{team_unsubscribe}}` auf dieselbe Weise, wenn die globale Einstellung zum Abmelden vom Append aktiviert ist.

>[!TIP]
>
>Wenn Ihre dynamischen Felder nicht ausgefüllt sind, lesen Sie [diesen Artikel](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
