---
unique-page-id: 4719314
description: Standardmäßige Salesforce-Feldzuordnung - Marketing-Dokumente - Produktdokumentation
title: Standardmäßige Zuweisung von Salesforce-Feldern
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# Standardmäßige Salesforce-Feldzuordnung {#default-salesforce-field-mapping}

Wenn Sie Ihr Marketo-Konto zum ersten Mal mit Salesforce synchronisieren, erstellt Marketo automatisch diese Verknüpfungen zwischen Ihren integrierten Salesforce- und Marketo-Feldern. Marketo synchronisiert auch Ihre benutzerdefinierten Felder auf Ihren Leads, Konten, Chancen und Kontakten.

## Interessentenfelder {#lead-fields}

| SFDC-Feld | Feld &quot;Marke&quot; |
|---|---|
| Jahresumsatz | Jahresumsatz |
| Ort | Ort |
| Firma | Name der Firma |
| Konvertierungsdatum | Konvertierungsdatum des SFDC |
| Land | Land |
| Erstellungsdatum | Erstellungsdatum des SFDC |
| Beschreibung | Personenknoten |
| Email | Email-Adresse |
| Fax | Faxnummer |
| Vorname | Vorname |
| Opt-out | Nicht abonniert |
| Branche | Branche |
| Konvertiert | SFDC wird konvertiert |
| Gelöscht | SFDC wird gelöscht |
| Nachname | Nachname |
| Interessentenquelle | Quelle |
| Interessentenbewertung | Ergebnis |
| Mobiltelefon | Mobiltelefonnummer |
| ArbeitnehmerInnen | Anzahl Arbeitnehmer |
| Telefon | Telefonnummer |
| PLZ/Postleitzahl | Postleitzahl |
| Beurteilung | Beurteilung |
| Anrede | Anrede |
| Bundesland/-staat | state |
| Status | Status |
| Straße | Adresse |
| Titel | Auftragstitel |
| Webseite | Webseite |

## Kontaktfelder {#contact-fields}

| SFDC-Feld | Feld &quot;Marke&quot; |
|---|---|
| Geburtsdatum | Geburtsdatum |
| Erstellungsdatum | Erstellungsdatum des SFDC |
| Kontaktbeschreibung | Personenknoten |
| Email | Email-Adresse |
| Business Fax | Faxnummer |
| Vorname | Vorname |
| Opt-out | Nicht abonniert |
| Gelöscht | SFDC wird gelöscht |
| Nachname | Nachname |
| Interessentenquelle | Quelle |
| Interessentenbewertung | Ergebnis |
| MailingCity | Ort |
| MailingCountry | Land |
| MailingPostalCode | Postleitzahl |
| MailingState | state |
| MailingStreet | Adresse |
| Mobiltelefon | Mobiltelefonnummer |
| Business Phone | Telefonnummer |
| Anrede | Anrede |
| Titel | Auftragstitel |

## Kontofelder {#account-fields}

| SFDC-Feld | Feld &quot;Marke&quot; |
|---|---|
| Jahresumsatz | Jahresumsatz |
| Rechnungsstadt | Rechnungsstadt |
| Rechnungsland | Rechnungsland |
| Rechnungsstellung Postleitzahl | Postleitzahl der Rechnungsstellung |
| Rechnungsland/-staat | Rechnungsstaat |
| Billing Street | Rechnungsadresse |
| Kontobeschreibung | Hinweise zur Firma |
| Branche | Branche |
| Gelöscht | SFDC wird gelöscht |
| Kontoname | Name der Firma |
| ArbeitnehmerInnen | Anzahl Arbeitnehmer |
| Konto Telefon | Hauptfach |
| SIC-Code | SIC-Code |
| Kontosite | Site |
| Kontotyp | SFDC-Typ |
| Webseite | Webseite |

## Salesforce-verwandte Systemfelder in Marketo (schreibgeschützt) {#salesforce-related-system-fields-in-marketo-read-only}

Diese Felder werden in Marketo erstellt, können aber nicht von Kunden angepasst werden.

| Feld | Beschreibung |
|---|---|
| SFDC-ID | Die Salesforce-ID mit 18 Zeichen |
| SFDC-Typ | Interessent oder Kontakt. Wenn leer, existiert der Interessent nur als Person in Marketo |
| Erstellungsdatum des SFDC | In SFDC erstelltes Datum (kann sich von Erstellungsdatum in Marketing unterscheiden) |
| SFDC wird gelöscht | Person war früher im SFDC, wurde aber gelöscht und lebt jetzt nur in Marketo |
