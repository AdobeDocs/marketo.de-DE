---
unique-page-id: 4719314
description: Standardmäßige Salesforce-Feldzuordnung - Marketo-Dokumente - Produktdokumentation
title: Standardmäßige Zuordnung von Salesforce-Feldern
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 57%

---

# Standardmäßige Zuordnung von Salesforce-Feldern {#default-salesforce-field-mapping}

Wenn Sie Ihr Marketo-Konto zum ersten Mal mit Salesforce synchronisieren, führt Marketo diese Verknüpfungen automatisch zwischen Ihren integrierten Salesforce- und Marketo-Feldern durch. Marketo synchronisiert auch Ihre benutzerdefinierten Felder mit Ihren Leads, Konten, Chancen und Kontakten.

## Lead-Felder {#lead-fields}

| SFDC-Feld | Marketo-Feld |
|---|---|
| Jahresumsatz | Jahresumsatz |
| Ort | Ort |
| Unternehmen | Untern.-name |
| Konvertiertes Datum | SFDC – Konvertiertes Datum |
| Land | Land |
| Erstellungsdatum | SFDC-Erstellungsdatum |
| Beschreibung | Personenhinweise |
| E-Mail | E-Mail-Adresse |
| Fax | Faxnummer |
| Vorname | Vorname |
| E-Mail-Abmeldung | Hat abbestellt |
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
| Bundesland/Kanton | Bundesland |
| Status | Status |
| Straße | Adresse |
| Titel | Jobtitel |
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
| E-Mail-Abmeldung | Hat abbestellt |
| Gelöscht | SFDC wurde gelöscht |
| Nachname | Nachname |
| Lead-Quelle | Quelle |
| Lead-Bewertung | Bewertung |
| MailingCity | Ort |
| MailingCountry | Land |
| MailingPostalCode | Postleitzahl |
| MailingState | Bundesland |
| MailingStreet | Adresse |
| Mobiltelefon | Mobiltelefonnummer |
| Geschäftstelefon | Telefonnummer |
| Anrede | Anrede |
| Titel | Jobtitel |

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
| Kontoname | Untern.-name |
| Mitarbeiter | Anzahl Mitarbeiter |
| Konto-Telefon | Haupttelefonnummer |
| SIC-Code | SIC-Code |
| Kontoseite | Seite |
| Kontotyp | SFDC-Typ |
| Webseite | Webseite |

## Salesforce-bezogene Systemfelder in Marketo (schreibgeschützt) {#salesforce-related-system-fields-in-marketo-read-only}

Diese Felder werden in Marketo erstellt, können jedoch nicht von den Kunden angepasst werden.

| Feld | Beschreibung |
|---|---|
| SFDC-ID | Die Salesforce-ID mit 18 Zeichen |
| SFDC-Typ | Lead oder Kontakt. Wenn leer, ist der Lead nur als Person in Marketo vorhanden |
| SFDC-Erstellungsdatum | Datum, das in SFDC erstellt wurde (kann sich von dem in Marketo erstellten unterscheiden) |
| SFDC wird gelöscht | Person, die früher Teil des SFDC war, aber gelöscht wurde und jetzt nur noch in Marketo lebt |