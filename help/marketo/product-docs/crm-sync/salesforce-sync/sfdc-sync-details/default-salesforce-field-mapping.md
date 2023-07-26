---
unique-page-id: 4719314
description: Standardmäßige Salesforce-Feldzuordnung - Marketo-Dokumente - Produktdokumentation
title: Standardmäßige Zuordnung von Salesforce-Feldern
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 58%

---

# Standardmäßige Zuordnung von Salesforce-Feldern {#default-salesforce-field-mapping}

Wenn Sie Ihr Marketo-Konto zum ersten Mal mit Salesforce synchronisieren, führt Marketo diese Verknüpfungen automatisch zwischen Ihren integrierten Salesforce- und Marketo-Feldern durch. Marketo synchronisiert auch Ihre benutzerdefinierten Felder mit Ihren Leads, Konten, Chancen und Kontakten.

## Lead-Felder {#lead-fields}

| SFDC-Feld | Marketo-Feld |
|---|---|
| Jahresumsatz | Jahresumsatz |
| Ort | Ort |
| Unternehmen | Firmenname |
| Konvertiertes Datum | SFDC – Konvertiertes Datum |
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
| Lead-Quelle | Quelle |
| Lead-Bewertung | Bewertung |
| Mobiltelefon | Mobiltelefonnummer |
| Mitarbeiter | Anzahl Mitarbeiter |
| Telefon | Telefonnummer |
| PLZ | Postleitzahl |
| Bewertung | Bewertung |
| Anrede | Anrede |
| Bundesland/Kanton | Status |
| Status | Status |
| Straße | Adresse |
| Titel | Job-Titel |
| Website | Website |

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
| Lead-Quelle | Quelle |
| Lead-Bewertung | Bewertung |
| MailingCity | Ort |
| MailingCountry | Land |
| Postleitzahl | Postleitzahl |
| MailingState | Status |
| MailingStreet | Adresse |
| Mobiltelefon | Mobiltelefonnummer |
| Geschäftstelefon | Telefonnummer |
| Anrede | Anrede |
| Titel | Job-Titel |

## Kontofelder {#account-fields}

| SFDC-Feld | Marketo-Feld |
|---|---|
| Jahresumsatz | Jahresumsatz |
| Rechnungsort | Rechnungsort |
| Rechnungsland | Rechnungsland |
| Postleitzahl der Abrechnung | Postleitzahl für Rechnung |
| Abrechnungsstaat/Provinz | Bundesland für Rechnung |
| Billing Street | Rechnungsadresse |
| Kontobeschreibung | Unternehmenshinweise |
| Branche | Branche |
| Gelöscht | SFDC wurde gelöscht |
| Kontoname | Firmenname |
| Mitarbeiter | Anzahl Mitarbeiter |
| Konto-Telefon | Haupttelefonnummer |
| SIC-Code | SIC-Code |
| Kontoseite | Seite |
| Kontotyp | SFDC-Typ |
| Website | Website |

## Salesforce-bezogene Systemfelder in Marketo (schreibgeschützt) {#salesforce-related-system-fields-in-marketo-read-only}

Diese Felder werden in Marketo erstellt, können jedoch nicht von den Kunden angepasst werden.

| Feld | Beschreibung |
|---|---|
| SFDC-ID | Die Salesforce-ID mit 18 Zeichen |
| SFDC-Typ | Lead oder Kontakt. Wenn leer, ist der Lead nur als Person in Marketo vorhanden |
| SFDC-Erstellungsdatum | In SFDC erstelltes Datum (kann sich von dem in Marketo erstellten unterscheiden) |
| SFDC wird gelöscht | Person, die früher Teil des SFDC war, aber gelöscht wurde und jetzt nur noch in Marketo lebt |
