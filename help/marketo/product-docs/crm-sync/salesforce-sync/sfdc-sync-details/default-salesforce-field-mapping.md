---
unique-page-id: 4719314
description: Standardmäßige Salesforce-Feldzuordnung - Marketo-Dokumente - Produktdokumentation
title: Standardmäßige Salesforce-Feldzuordnung
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 59%

---

# Standardmäßige Salesforce-Feldzuordnung {#default-salesforce-field-mapping}

Wenn Sie Ihr Marketo Engage-Konto zum ersten Mal mit Salesforce synchronisieren, führt Marketo diese Verknüpfungen zwischen Ihren integrierten Salesforce- und Marketo-Feldern automatisch durch. Marketo synchronisiert auch Ihre benutzerdefinierten Felder für Leads, Konten, Chancen und Kontakte.

## Lead-Felder {#lead-fields}

| SFDC-Feld | Marketo-Feld |
|---|---|
| Jahresumsatz | Jahresumsatz |
| Stadt | Stadt |
| Unternehmen | Firmenname |
| Konvertiertes Datum | SFDC – Konvertiertes Datum |
| Land | Land |
| Erstellungsdatum | SFDC-Erstellungsdatum |
| Beschreibung | Personenhinweise |
| E-Mail | E-Mail-Adresse |
| Fax | Faxnummer |
| Vorname | Vorname |
| E-Mail-Abmeldung | Abbestellt |
| Branche | Branche |
| Konvertiert | SFDC wird konvertiert |
| Gelöscht | SFDC wurde gelöscht |
| Nachname | Nachname |
| Lead-Quelle | Quelle |
| Lead-Bewertung | Ergebnis |
| Mobiltelefon | Mobiltelefonnummer |
| Mitarbeiter | Anzahl Mitarbeiter |
| Telefon | Telefonnummer |
| PLZ | Postleitzahl |
| Rating | Rating |
| Anrede | Anrede |
| Bundesland/Provinz | Land |
| Status | Status |
| Straße | Adresse |
| Titel | Jobtitel |
| Website | Website |

## Kontaktfelder {#contact-fields}

| SFDC-Feld | Marketo-Feld |
|---|---|
| Geburtsdatum | Geburtsdatum |
| Erstellungsdatum | SFDC Created Date |
| Kontaktbeschreibung | Personenhinweise |
| E-Mail | E-Mail-Adresse |
| Fax (geschäftlich) | Faxnummer |
| Vorname | Vorname |
| E-Mail-Abmeldung | Abbestellt |
| Gelöscht | SFDC wurde gelöscht |
| Nachname | Nachname |
| Lead-Quelle | Quelle |
| Lead-Bewertung | Ergebnis |
| MailingCity | Stadt |
| MailingCountry | Land |
| MailingPostalCode | Postleitzahl |
| MailingState | Land |
| MailingStreet | Adresse |
| Mobiltelefon | Mobiltelefonnummer |
| Geschäftstelefon | Telefonnummer |
| Anrede | Anrede |
| Titel | Jobtitel |

## Kontofelder {#account-fields}

| SFDC-Feld | Marketo-Feld |
|---|---|
| Jahresumsatz | Jahresumsatz |
| Abrechnungsort | Abrechnungsort |
| Abrechnungsland | Abrechnungsland |
| Postleitzahl für die Rechnungsstellung | Postleitzahl für Abrechnung |
| Fakturastaat/Provinz | Bundesland für Abrechnung |
| Abrechnungsstraße | Rechnungsadresse |
| Kontobeschreibung | Unternehmenshinweise |
| Branche | Branche |
| Gelöscht | SFDC wurde gelöscht |
| Kontoname | Firmenname |
| Mitarbeiter | Anzahl Mitarbeiter |
| Telefonnummer des Kontos | Haupttelefonnummer |
| SIC-Code | SIC-Code |
| Konto-Website | Seite |
| Kontotyp | SFDC-Typ |
| Website | Website |

## Salesforce-bezogene Systemfelder in Marketo (schreibgeschützt) {#salesforce-related-system-fields-in-marketo-read-only}

Diese Felder werden in Marketo erstellt, können von Kunden jedoch nicht angepasst werden.

| Feld | Beschreibung |
|---|---|
| SFDC-ID | Die 18-stellige Salesforce ID |
| SFDC-Typ | Lead oder Kontakt. Wenn leer, ist der Lead nur als Person in Marketo vorhanden |
| SFDC Created Date | Erstellungsdatum in SFDC (kann sich von dem in Marketo unterscheiden) |
| SFDC wird gelöscht | Person war früher in SFDC, wurde jedoch gelöscht und lebt jetzt nur noch in Marketo |
