---
description: Standardmäßige Dynamics-Feldzuordnung - Marketo-Dokumente - Produktdokumentation
title: Dynamische Standardfeldzuordnung
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 46%

---

# Dynamische Standardfeldzuordnung {#default-dynamics-field-mapping}

Wenn Sie Ihr Marketo Engage-Konto zum ersten Mal mit Microsoft synchronisieren, führt Marketo diese Verknüpfungen zwischen Ihren integrierten Dynamics- und Marketo-Feldern automatisch durch.  Marketo synchronisiert auch Ihre benutzerdefinierten Felder für Leads, Konten, Chancen und Kontakte.

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
      <th>MS Dynamics-Feld</th>
      <th>MS Dynamics API-Name</th>
    </tr>
    <tr>
      <td>Microsoft – Erstellungsdatum</td>
      <td>Erstellt am</td>
      <td>createdOn</td>
    </tr>
    <tr>
      <td>Anrede</td>
      <td>Anrede</td>
      <td>Begrüßung</td>
    </tr>
    <tr>
      <td>Zuerst</td>
      <td>Vorname</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>Zweiter Vorname</td>
      <td>Zweiter Vorname</td>
      <td>MiddleName</td>
    </tr>
    <tr>
      <td>Zuletzt</td>
      <td>Nachname</td>
      <td>lastname</td>
    </tr>
    <tr>
      <td>E-Mail</td>
      <td>E-Mail</td>
      <td>emailAddress1</td>
    </tr>
    <tr>
      <td>Jobtitel</td>
      <td>Stellenbezeichnung</td>
      <td>Stellenbezeichnung</td>
    </tr>
    <tr>
      <td>Telefon</td>
      <td>Geschäftstelefon</td>
      <td>Telefon 1</td>
    </tr>
    <tr>
      <td>Mobile</td>
      <td>Mobiltelefon</td>
      <td>Mobiltelefon</td>
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
      <td>Stadt</td>
      <td>Stadt</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>Land</td>
      <td>Bundesland/Provinz</td>
      <td>address1_stateorProvince</td>
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
      <td>Lead-Quellcode</td>
    </tr>
    <tr>
      <td>Personen-Status</td>
      <td>Status</td>
      <td>Zustandscode</td>
    </tr>
    <tr>
      <td>Status – Grund</td>
      <td>Status – Grund</td>
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
      <td>Donotphone</td>
    </tr>
    <tr>
      <td>Abbestellt</td>
      <td>Keine Massen-E-Mails senden</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>Personenbewertung</td>
      <td>Rating</td>
      <td>LeadQualityCode</td>
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
      <td>donotemail</td>
    </tr>
    <tr>
      <td>Microsoft – Kein Fax senden</td>
      <td>Faxe nicht zulassen</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>Microsoft – Kein Marketingmaterial senden</td>
      <td>Marketingmaterial</td>
      <td>donotsendm</td>
    </tr>
    <tr>
      <td>Microsoft – Telefon privat</td>
      <td>Privates Telefon</td>
      <td>Telefon2</td>
    </tr>
    <tr>
      <td>Bevorzugte Kontaktmethode von Microsoft</td>
      <td>Bevorzugte Kontaktmethode</td>
      <td>PreferredContactMethodCode</td>
    </tr>
    <tr>
      <td>Microsoft – Thema</td>
      <td>Thema</td>
      <td>Subjekt</td>
    </tr>
    <tr>
      <td>Datum des letzten interessanten Moments</td>
      <td>Datum des letzten interessanten Moments</td>
      <td>mkt_lastInterestingMomentDate</td>
    </tr>
    <tr>
      <td>Beschreibung des letzten interessanten Moments</td>
      <td>Beschreibung des letzten interessanten Moments</td>
      <td>mkt_lastInterestedMomentdesc</td>
    </tr>
    <tr>
      <td>Quelle des letzten interessanten Moments</td>
      <td>Quelle des letzten interessanten Moments</td>
      <td>mkt_leadInterestedMomentsource</td>
    </tr>
    <tr>
      <td>Typ des letzten interessanten Moments</td>
      <td>Typ des letzten interessanten Moments</td>
      <td>mkt_lastInterestingMomentType</td>
    </tr>
    <tr>
      <td>Unternehmen</td>
      <td>Firmenname</td>
      <td>companyName</td>
    </tr>
    <tr>
      <td>Relative Bewertung</td>
      <td>Relative Bewertung</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>Priorität</td>
      <td>Priorität</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Relative Dringlichkeit</td>
      <td>Dringlichkeit</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Betreff</td>
      <td>Thema</td>
      <td>Subjekt</td>
    </tr>
    <tr>
      <td>Jahresumsatz</td>
      <td>Jahresumsatz</td>
      <td>Umsatz</td>
    </tr>
  </tbody>
</table>

Die folgenden Lead-Felder werden für die interne Verwendung synchronisiert.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics-Feld</th>
      <th>MS Dynamics API-Name</th>
    </tr>
    <tr>
      <td>Eigentümer</td>
      <td>ownerID</td>
    </tr>
    <tr>
      <td>Erstellt am</td>
      <td>createdOn</td>
    </tr>
  </tbody>
</table>

## Kontaktfelder {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo-Feld</th>
      <th>MS Dynamics-Feld</th>
      <th>MS Dynamics API-Name</th>
    </tr>
    <tr>
      <td>Microsoft – Erstellungsdatum</td>
      <td>Erstellt am</td>
      <td>createdOn</td>
    </tr>
    <tr>
      <td>Anrede</td>
      <td>Anrede</td>
      <td>Begrüßung</td>
    </tr>
    <tr>
      <td>Zuerst</td>
      <td>Vorname</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>Zweiter Vorname</td>
      <td>Zweiter Vorname</td>
      <td>MiddleName</td>
    </tr>
    <tr>
      <td>Zuletzt</td>
      <td>Nachname</td>
      <td>lastname</td>
    </tr>
    <tr>
      <td>E-Mail</td>
      <td>E-Mail</td>
      <td>emailAddress1</td>
    </tr>
    <tr>
      <td>Jobtitel</td>
      <td>Jobtitel</td>
      <td>Stellenbezeichnung</td>
    </tr>
    <tr>
      <td>Telefon</td>
      <td>Geschäftstelefon</td>
      <td>Telefon 1</td>
    </tr>
    <tr>
      <td>Mobile</td>
      <td>Mobiltelefon</td>
      <td>Mobiltelefon</td>
    </tr>
    <tr>
      <td>Adresse</td>
      <td>Adresse 1: Straße 1</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>Stadt</td>
      <td>Adresse 1: Ort</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>Land</td>
      <td>Adresse 1: Bundesland/Kanton</td>
      <td>address1_stateorProvince</td>
    </tr>
    <tr>
      <td>Land</td>
      <td>Adresse 1: Land/Region</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>Postleitzahl</td>
      <td>Adresse 1: Postleitzahl</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>Personen-Status</td>
      <td>Status</td>
      <td>Zustandscode</td>
    </tr>
    <tr>
      <td>Status – Grund</td>
      <td>Status – Grund</td>
      <td>statuscode</td>
    </tr>
    <tr>
      <td>Nicht aufrufen</td>
      <td>Telefonanrufe nicht zulassen</td>
      <td>Donotphone</td>
    </tr>
    <tr>
      <td>Abbestellt</td>
      <td>Keine Massen-E-Mails senden</td>
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
      <td>donotemail</td>
    </tr>
    <tr>
      <td>Microsoft – Telefon privat</td>
      <td>Privates Telefon</td>
      <td>Telefon2</td>
    </tr>
    <tr>
      <td>Bevorzugte Kontaktmethode von Microsoft</td>
      <td>Bevorzugte Kontaktmethode</td>
      <td>PreferredContactMethodCode</td>
    </tr>
    <tr>
      <td>Datum des letzten interessanten Moments</td>
      <td>Datum des letzten interessanten Moments</td>
      <td>mkt_lastInterestingMomentDate</td>
    </tr>
    <tr>
      <td>Typ des letzten interessanten Moments</td>
      <td>Typ des letzten interessanten Moments</td>
      <td>mkt_lastInterestingMomentType</td>
    </tr>
    <tr>
      <td>Quelle des letzten interessanten Moments</td>
      <td>Quelle des letzten interessanten Moments</td>
      <td>mkt_leadInterestedMomentsource</td>
    </tr>
    <tr>
      <td>Beschreibung des letzten interessanten Moments</td>
      <td>Beschreibung des letzten interessanten Moments</td>
      <td>mkt_lastInterestedMomentdesc</td>
    </tr>
    <tr>
      <td>Microsoft – Kein Marketingmaterial senden</td>
      <td>Marketingmaterial</td>
      <td>donotsendm</td>
    </tr>
    <tr>
      <td>Microsoft – Kein Fax senden</td>
      <td>Microsoft – Kein Fax senden</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>Priorität</td>
      <td>Priorität</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Relative Dringlichkeit</td>
      <td>Dringlichkeit</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Relative Bewertung</td>
      <td>Relative Bewertung</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>Personenhinweise</td>
      <td>Beschreibung</td>
      <td>Beschreibung</td>
    </tr>
    <tr>
      <td>Personen-Punktzahl</td>
      <td>Lead-Bewertung</td>
      <td>mkt_leadscore</td>
    </tr>
    <tr>
      <td>Personenhinweise</td>
      <td>Beschreibung</td>
      <td>Beschreibung</td>
    </tr>
  </tbody>
</table>

Die folgenden Kontaktfelder werden für die interne Verwendung synchronisiert.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics-Feld</th>
      <th>MS Dynamics API-Name</th>
    </tr>
    <tr>
      <td>Eigentümer</td>
      <td>ownerID</td>
    </tr>
    <tr>
      <td>Erstellt am</td>
      <td>createdOn</td>
    </tr>
    <tr>
      <td>parentCustomerID</td>
      <td>Firmenname</td>
    </tr>
  </tbody>
</table>

## Kontofelder {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo-Feld</th>
      <th>MS Dynamics-Feld</th>
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
      <td>Adresse 1: Postleitzahl</td>
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
      <td>Telefon 1</td>
    </tr>
    <tr>
      <td>Unternehmenstyp</td>
      <td>Unternehmenstyp</td>
      <td>BusinessTypeCode</td>
    </tr>
    <tr>
      <td>Microsoft-Kontonummer</td>
      <td>Kontonummer</td>
      <td>Kontonummer</td>
    </tr>
    <tr>
      <td>Microsoft – Unternehmensstatus</td>
      <td>Status</td>
      <td>Zustandscode</td>
    </tr>
    <tr>
      <td>Jahresumsatz</td>
      <td>Jahresumsatz</td>
      <td>Umsatz</td>
    </tr>
    <tr>
      <td>Unternehmenshinweise</td>
      <td>Beschreibung</td>
      <td>Beschreibung</td>
    </tr>
    <tr>
      <td>Branche</td>
      <td>Branche</td>
      <td>Branchencode</td>
    </tr>
    <tr>
      <td>SIC-Code</td>
      <td>SIC-Code</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>Website</td>
      <td>Website</td>
      <td>Website</td>
    </tr>
    <tr>
      <td>Anzahl Mitarbeiter</td>
      <td>Anzahl der Mitarbeiter</td>
      <td>Anzahl der Mitarbeiter</td>
    </tr>
    <tr>
      <td>SIC-Code</td>
      <td>SIC-Code</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>Unternehmen</td>
      <td>Kontoname</td>
      <td>name</td>
    </tr>
    <tr>
      <td>Anzahl Mitarbeiter</td>
      <td>Anzahl der Mitarbeiter</td>
      <td>Anzahl der Mitarbeiter</td>
    </tr>
  </tbody>
</table>

Die folgenden Kontofelder werden für die interne Verwendung synchronisiert.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics-Feld</th>
      <th>MS Dynamics API-Name</th>
    </tr>
    <tr>
      <td>Eigentümer</td>
      <td>ownerID</td>
    </tr>
    <tr>
      <td>Erstellt am</td>
      <td>createdOn</td>
    </tr>
  </tbody>
</table>

## Opportunity-Felder {#opportunity-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo-Feld</th>
      <th>MS Dynamics-Feld</th>
      <th>MS Dynamics API-Name</th>
    </tr>
    <tr>
      <td>Abschlusswahrscheinlichkeit</td>
      <td>Wahrscheinlichkeit</td>
      <td>Nahwahrscheinlichkeit</td>
    </tr>
    <tr>
      <td>Phase</td>
      <td>status</td>
      <td>Zustandscode</td>
    </tr>
    <tr>
      <td>Tatsächliches Abschlussdatum</td>
      <td>Tatsächliches Abschlussdatum</td>
      <td>actualCloseDate</td>
    </tr>
    <tr>
      <td>Name</td>
      <td>Thema</td>
      <td>name</td>
    </tr>
    <tr>
      <td>Geschätzter Wert</td>
      <td>Gesch. Umsatz</td>
      <td>estimatedValue</td>
    </tr>
    <tr>
      <td>Beschreibung</td>
      <td>Beschreibung</td>
      <td>Beschreibung</td>
    </tr>
  </tbody>
</table>

Die folgenden Kontofelder werden für die interne Verwendung synchronisiert.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics-Feld</th>
      <th>MS Dynamics API-Name</th>
    </tr>
    <tr>
      <td>Eigentümer</td>
      <td>ownerID</td>
    </tr>
    <tr>
      <td>Opportunity</td>
      <td>OpportunityId</td>
    </tr>
    <tr>
      <td>Potenzieller Kunde</td>
      <td>customerId</td>
    </tr>
  </tbody>
</table>

## Microsoft-bezogene Systemfelder in Marketo (schreibgeschützt) {#microsoft-related-system-fields}

Die folgenden Felder werden in Marketo erstellt, können jedoch von Benutzenden nicht angepasst werden.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo-Feld</th>
      <th>Beschreibung</th>
    </tr>
    <tr>
      <td>Microsoft – Typ</td>
      <td>Lead oder Kontakt. Wenn leer, ist der Lead nur als Person in Marketo vorhanden</td>
    </tr>
    <tr>
      <td>Microsoft – Erstellungsdatum</td>
      <td>Erstellungsdatum in MS Dynamics (kann sich von dem in Marketo unterscheiden)</td>
    </tr>
    <tr>
      <td>Microsoft wird gelöscht</td>
      <td>Person war früher in Microsoft, wurde jedoch gelöscht und lebt jetzt nur noch in Marketo</td>
    </tr>
  </tbody>
</table>
