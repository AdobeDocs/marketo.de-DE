---
unique-page-id: 4719314
description: Standardmäßige Salesforce-Feldzuordnung - Marketo Docs - Produktdokumentation
title: Standardmäßige Zuweisung von Salesforce-Feldern
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 57%

---

# Standardmäßige Salesforce-Feldzuordnung {#default-salesforce-field-mapping}

Wenn Sie Ihr Marketo-Konto zum ersten Mal mit Salesforce synchronisieren, stellt Marketo diese Verbindungen automatisch zwischen Ihren integrierten Salesforce- und Marketo-Feldern her. Marketo synchronisiert außerdem Ihre benutzerdefinierten Felder mit Ihren Leads, Konten, Möglichkeiten und Kontakten.

## Lead-Felder {#lead-fields}

| SFDC-Feld | Marketo-Feld |
|---|---|
| Jahresumsatz | Jahresumsatz |
| Ort | Ort |
| Unternehmen | Unternehmensname |
| Konvertierungsdatum | SFDC – Konvertiertes Datum |
| Land | Land |
| Erstellungsdatum | SFDC-Erstellungsdatum |
| Beschreibung | Personenhinweise |
| E-Mail | E-Mail-Adresse |
| Fax | Faxnummer |
| Vorname | Vorname |
| E-Mail-Abmeldung | Abgemeldet |
| Branche | Branche |
| Konvertiert | SFDC wird konvertiert |
| Gelöscht | SFDC wurde gelöscht |
| Nachname | Nachname |
| Lead Quelle | Quelle |
| Lead-Bewertung | Bewertung |
| Mobiltelefon | Mobiltelefonnummer |
| Mitarbeiter | Anzahl Mitarbeiter |
| Telefon | Telefonnummer |
| PLZ | Postleitzahl |
| Bewertung | Bewertung |
| Anrede | Anrede |
| Bundesland/Kanton | Bundesland |
| Status | Status |
| Straße | Adresse |
| Stellenbezeichnung | Jobtitel |
| Website | Webseite |

## Kontaktfelder {#contact-fields}

| SFDC-Feld | Marketo-Feld |
|---|---|
| Geburtsdatum | Geburtsdatum |
| Erstellungsdatum | SFDC-Erstellungsdatum |
| Kontaktbeschreibung | Personenhinweise |
| E-Mail | E-Mail-Adresse |
| Business Fax | Faxnummer |
| Vorname | Vorname |
| E-Mail-Abmeldung | Abgemeldet |
| Gelöscht | SFDC wurde gelöscht |
| Nachname | Nachname |
| Interessent Quelle | Quelle |
| Lead-Bewertung | Bewertung |
| MailingCity | Ort |
| MailingCountry | Land |
| MailingPostalCode | Postleitzahl |
| MailingState | Bundesland |
| MailingStreet | Adresse |
| Mobiltelefon | Mobiltelefonnummer |
| Geschäftstelefon | Telefonnummer |
| Anrede | Anrede |
| Stellenbezeichnung | Jobtitel |

## Kontofelder {#account-fields}

| SFDC-Feld | Marketo-Feld |
|---|---|
| Jahresumsatz | Jahresumsatz |
| Abrechnungsort | Abrechnungsort |
| Abrechnungsland | Abrechnungsland |
| Rechnungsstellung Postleitzahl | Postleitzahl für Abrechnung |
| Rechnungsland/-staat | Bundesland für Abrechnung |
| Billing Street | Rechnungsadresse |
| Kontobeschreibung | Unternehmenshinweise |
| Branche | Branche |
| Gelöscht | SFDC wurde gelöscht |
| Kontoname | Unternehmensname |
| Mitarbeiter | Anzahl Mitarbeiter |
| Konto Telefon | Haupttelefonnummer |
| SIC-Code | SIC-Code |
| Kontosite | Seite |
| Kontotyp | SFDC-Typ |
| Webseite | Webseite |

## Salesforce-bezogene Systemfelder in Marketo (schreibgeschützt) {#salesforce-related-system-fields-in-marketo-read-only}

Diese Felder werden in Marketo erstellt, können jedoch nicht von Kunden angepasst werden.

| Feld | Beschreibung |
|---|---|
| SFDC-ID | Die Salesforce-ID mit 18 Zeichen |
| SFDC-Typ | Interessent oder Kontakt. Wenn leer, existiert der Interessent nur als Person in Marketo |
| SFDC-Erstellungsdatum | In SFDC erstelltes Datum (kann sich von Erstellungsdatum in Marketo unterscheiden) |
| SFDC wird gelöscht | Personen, die früher im SFDC waren, aber gelöscht wurden und jetzt nur noch in Marketo leben |
