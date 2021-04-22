---
description: Standardmäßige Feldzuordnung für Dynamiken - Marketo Docs - Produktdokumentation
title: Standardmäßige Feldzuordnung für Dynamik
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 47%

---

# Standardmäßige Feldzuordnung für Dynamik {#default-dynamics-field-mapping}

Wenn Sie Ihr Marketo-Konto zunächst mit Microsoft synchronisieren, stellt Marketo automatisch diese Verbindungen zwischen Ihren integrierten Dynamics- und Marketo-Feldern her.  Marketo synchronisiert außerdem Ihre benutzerdefinierten Felder mit Ihren Leads, Konten, Möglichkeiten und Kontakten.

## Lead-Felder {#lead-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Marketo-Feld</th> 
   <th>MS Dynamics Field</th> 
   <th>MS Dynamics API-Name</th> 
  </tr> 
  <tr> 
   <td>Microsoft – Erstellungsdatum</td> 
   <td>Erstellt am</td> 
   <td>createdon</td> 
  </tr> 
  <tr> 
   <td>Anrede</td> 
   <td>Anrede</td> 
   <td>Anrede</td> 
  </tr> 
  <tr> 
   <td>Vorname</td> 
   <td>Vorname</td> 
   <td>firstname</td> 
  </tr> 
  <tr> 
   <td>Zweiter Vorname</td> 
   <td>Zweiter Vorname</td> 
   <td>middlename</td> 
  </tr> 
  <tr> 
   <td>Nachname</td> 
   <td>Nachname</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>E-Mail</td> 
   <td>E-Mail</td> 
   <td>emailaddress1</td> 
  </tr> 
  <tr> 
   <td>Jobtitel</td> 
   <td>Stellenbezeichnung</td> 
   <td>jobtitle</td> 
  </tr> 
  <tr> 
   <td>Telefon</td> 
   <td>Geschäftstelefon</td> 
   <td>telephone1</td> 
  </tr> 
  <tr> 
   <td>Mobil</td> 
   <td>Mobiltelefon</td> 
   <td>mobilephone</td> 
  </tr> 
  <tr> 
   <td>Fax</td> 
   <td>Fax</td> 
   <td>Fax</td> 
  </tr> 
  <tr> 
   <td>Adresse</td> 
   <td>Straße 1</td> 
   <td>address1_line1</td> 
  </tr> 
  <tr> 
   <td>Ort</td> 
   <td>Ort</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>Bundesland</td> 
   <td>Bundesland/Kanton</td> 
   <td>address1_stateorprovinz</td> 
  </tr> 
  <tr> 
   <td>Land</td> 
   <td>Land/Region</td> 
   <td>address1_country</td> 
  </tr> 
  <tr> 
   <td>Postleitzahl</td> 
   <td>PLZ</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>Person – Quelle</td> 
   <td>Lead-Quelle</td> 
   <td>leadsourcecode</td> 
  </tr> 
  <tr> 
   <td>Personen-Status</td> 
   <td>Status</td> 
   <td>statecode</td> 
  </tr> 
  <tr> 
   <td>Statusgrund</td> 
   <td>Statusgrund</td> 
   <td>statuscode</td> 
  </tr> 
  <tr> 
   <td>Personenhinweise</td> 
   <td>Beschreibung</td> 
   <td>Beschreibung</td> 
  </tr> 
  <tr> 
   <td>Nicht aufrufen</td> 
   <td>Telefonanrufe nicht zulassen</td> 
   <td>donotphone</td> 
  </tr> 
  <tr> 
   <td>Abgemeldet</td> 
   <td>Keine Massen-E-Mail</td> 
   <td>donotbulkemail</td> 
  </tr> 
  <tr> 
   <td>Personenbewertung</td> 
   <td>Bewertung</td> 
   <td>Leadqualitycode</td> 
  </tr> 
  <tr> 
   <td>Microsoft – Adresse 2</td> 
   <td>Straße 2</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Microsoft – Adresse 3</td> 
   <td>Straße 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Microsoft – Keine E-Mail senden</td> 
   <td>E-Mails nicht zulassen</td> 
   <td>Donotemail</td> 
  </tr> 
  <tr> 
   <td>Microsoft – Kein Fax senden</td> 
   <td>Faxe nicht zulassen</td> 
   <td>donotfax</td> 
  </tr> 
  <tr> 
   <td>Microsoft – Kein Marketingmaterial senden</td> 
   <td>Marketingmaterial</td> 
   <td>donotsendmm</td> 
  </tr> 
  <tr> 
   <td>Microsoft – Telefon privat</td> 
   <td>Festnetztelefon</td> 
   <td>telephone2</td> 
  </tr> 
  <tr> 
   <td>Bevorzugte Microsoft-Kontaktmethode</td> 
   <td>Bevorzugte Kontaktmethode</td> 
   <td>preferConactmethodcode</td> 
  </tr> 
  <tr> 
   <td>Microsoft – Thema</td> 
   <td>Thema</td> 
   <td>subject</td> 
  </tr> 
 </tbody> 
</table>

## Kontaktfelder {#contact-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Marketo-Feld</th> 
   <th>MS Dynamics Field</th> 
   <th>MS Dynamics API-Name</th> 
  </tr> 
  <tr> 
   <td>Microsoft – Erstellungsdatum</td> 
   <td>Erstellt am</td> 
   <td>createdon</td> 
  </tr> 
  <tr> 
   <td>Anrede</td> 
   <td>Anrede</td> 
   <td>Anrede</td> 
  </tr> 
  <tr> 
   <td>Vorname</td> 
   <td>Vorname</td> 
   <td>firstname</td> 
  </tr> 
  <tr> 
   <td>Zweiter Vorname</td> 
   <td>Zweiter Vorname</td> 
   <td>middlename</td> 
  </tr> 
  <tr> 
   <td>Nachname</td> 
   <td>Nachname</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>E-Mail</td> 
   <td>E-Mail</td> 
   <td>emailaddress1</td> 
  </tr> 
  <tr> 
   <td>Jobtitel</td> 
   <td>Jobtitel</td> 
   <td>jobtitle</td> 
  </tr> 
  <tr> 
   <td>Telefon</td> 
   <td>Geschäftstelefon</td> 
   <td>telephone1</td> 
  </tr> 
  <tr> 
   <td>Mobil</td> 
   <td>Mobiltelefon</td> 
   <td>mobilephone</td> 
  </tr> 
  <tr> 
   <td>Adresse</td> 
   <td>Adresse 1: Straße 1</td> 
   <td>address1_line1</td> 
   <tr> 
   <td>Ort</td> 
   <td>Adresse 1: Ort</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>Bundesland</td> 
   <td>Adresse 1: Bundesland/Kanton</td> 
   <td>address1_stateorprovinz</td> 
  </tr> 
  <tr> 
   <td>Land</td> 
   <td>Adresse 1: Land/Region</td> 
   <td>address1_country</td> 
   <tr> 
   <td>Postleitzahl</td> 
   <td>Adresse 1: PLZ/Postleitzahl</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>Personen-Status</td> 
   <td>Status</td> 
   <td>statecode</td> 
  </tr> 
  <tr> 
   <td>Statusgrund</td> 
   <td>Statusgrund</td> 
   <td>statuscode</td> 
  </tr> 
   <tr> 
   <td>Nicht aufrufen</td> 
   <td>Telefonanrufe nicht zulassen</td> 
   <td>donotphone</td> 
  </tr> 
  <tr> 
   <td>Abgemeldet</td> 
   <td>Keine Massen-E-Mail</td> 
   <td>donotbulkemail</td> 
  </tr> 
  <tr> 
   <td>Microsoft – Adresse 2</td> 
   <td>Adresse 1: Straße 2</td> 
   <td>address1_line2</td> 
  </tr> 
   <tr> 
   <td>Microsoft – Adresse 3</td> 
   <td>Adresse 1: Straße 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Microsoft – Keine E-Mail senden</td> 
   <td>E-Mails nicht zulassen</td> 
   <td>Donotemail</td> 
  </tr> 
  <tr> 
   <td>Microsoft – Telefon privat</td> 
   <td>Festnetztelefon</td> 
   <td>telephone2</td> 
  </tr> 
  <tr> 
   <td>Bevorzugte Microsoft-Kontaktmethode</td> 
   <td>Bevorzugte Kontaktmethode</td> 
   <td>preferConactmethodcode</td> 
  </tr> 
 </tbody> 
</table>

## Kontofelder {#account-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Marketo-Feld</th> 
   <th>MS Dynamics Field</th> 
   <th>MS Dynamics API-Name</th> 
  </tr> 
  <tr> 
   <td>Konto (a)</td> 
   <td>Konto</td> 
   <td>accountid</td> 
  </tr> 
  <tr> 
   <td>Rechnungsadresse</td> 
   <td>Adresse 1: Straße 1</td> 
   <td>address1_line1</td> 
  </tr> 
  <tr> 
   <td>Abrechnungsort</td> 
   <td>Adresse 1: Ort</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>Abrechnungsland</td> 
   <td>Adresse 1: Land/Region</td> 
   <td>address1_country</td> 
  </tr> 
  <tr> 
   <td>Postleitzahl für Abrechnung</td> 
   <td>Adresse 1: PLZ/Postleitzahl</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>Microsoft – Rechnungsadresse 2</td> 
   <td>Adresse 1: Straße 2</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Microsoft – Rechnungsadresse 3</td> 
   <td>Adresse 1: Straße 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Haupttelefonnummer</td> 
   <td>Haupttelefonnummer</td> 
   <td>telephone1</td> 
  </tr> 
  <tr> 
   <td>Unternehmenstyp</td> 
   <td>Unternehmenstyp</td> 
   <td>businessStypecode</td> 
  </tr> 
  <tr> 
   <td>Microsoft-Kontonummer</td> 
   <td>Kontonummer</td> 
   <td>accountNumber</td> 
  </tr> 
  <tr> 
   <td>Microsoft – Unternehmensstatus</td> 
   <td>Status</td> 
   <td>statecode</td> 
  </tr> 
  <tr> 
   <td>Jahresumsatz</td> 
   <td>Jahresumsatz</td> 
   <td>umsatz</td> 
  </tr> 
  <tr> 
   <td>Unternehmenshinweise</td> 
   <td>Beschreibung</td> 
   <td>Beschreibung</td> 
  </tr> 
  <tr> 
   <td>Branche</td> 
   <td>Branche</td> 
   <td>industrycode</td> 
  </tr> 
  <tr> 
   <td>SIC-Code</td> 
   <td>SIC-Code</td> 
   <td>sic</td> 
  </tr> 
  <tr> 
   <td>Website</td> 
   <td>Webseite</td> 
   <td>website</td> 
  </tr> 
 </tbody> 
</table>

## Microsoft-bezogene Systemfelder in Marketo (schreibgeschützt) {#microsoft-related-system-fields-in-marketo}

Diese Felder werden in Marketo erstellt, können jedoch nicht von Kunden angepasst werden.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Marketo-Feld</th> 
   <th>Beschreibung</th> 
  </tr> 
  <tr> 
   <td>Microsoft – Typ</td> 
   <td>Interessent oder Kontakt. Wenn leer, existiert der Interessent nur als Person in Marketo</td> 
  </tr> 
  <tr> 
   <td>Microsoft – Erstellungsdatum</td> 
   <td>In MS Dynamics erstelltes Datum (kann sich von Erstellt in Marketo unterscheiden)</td> 
  </tr> 
  <tr> 
   <td>Microsoft wird gelöscht</td> 
   <td>Er war früher bei Microsoft, wurde aber gelöscht und lebt jetzt nur noch in Marketo</td> 
  </tr> 
 </tbody> 
</table>
