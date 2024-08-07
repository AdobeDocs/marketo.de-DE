---
description: Standardmäßige Dynamics-Feldzuordnung - Marketo-Dokumente - Produktdokumentation
title: Standardmäßige Dynamics-Feldzuordnung
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 45%

---

# Standardmäßige Dynamics-Feldzuordnung {#default-dynamics-field-mapping}

Wenn Sie Ihr Marketo Engage-Konto zum ersten Mal mit Microsoft synchronisieren, führt Marketo diese Verknüpfungen automatisch zwischen Ihren integrierten Dynamics- und Marketo-Feldern durch.  Marketo synchronisiert auch Ihre benutzerdefinierten Felder mit Ihren Leads, Konten, Chancen und Kontakten.

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
      <td>createdon</td>
    </tr>
    <tr>
      <td>Anrede</td>
      <td>Anrede</td>
      <td>salutation</td>
    </tr>
    <tr>
      <td>Zuerst</td>
      <td>Vorname</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>Zweiter Vorname</td>
      <td>Zweiter Vorname</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>Zuletzt</td>
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
      <td>fax</td>
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
      <td>Telefonaufrufe nicht zulassen</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>Abbestellt</td>
      <td>Massen-E-Mail nicht</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>Personenbewertung</td>
      <td>Bewertung</td>
      <td>Leadqualitätscode</td>
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
      <td>Marketing-Material</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>Microsoft – Telefon privat</td>
      <td>Telefonnummer (privat)</td>
      <td>telephone2</td>
    </tr>
    <tr>
      <td>Von Microsoft bevorzugte Kontaktmethode</td>
      <td>Bevorzugte Kontaktmethode</td>
      <td>preferredContextMethodencode</td>
    </tr>
    <tr>
      <td>Microsoft – Thema</td>
      <td>Thema</td>
      <td>subject</td>
    </tr>
    <tr>
      <td>Letztes interessantes Datum</td>
      <td>Letztes interessantes Datum</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>Letzter interessanter Moment desc</td>
      <td>Letzter interessanter Moment desc</td>
      <td>mkt_lastinterestingmomentdesc</td>
    </tr>
    <tr>
      <td>Letzte interessante Moment-Quelle</td>
      <td>Letzte interessante Moment-Quelle</td>
      <td>mkt_leadinterestingmomentsource</td>
    </tr>
    <tr>
      <td>Letzter interessanter Moment</td>
      <td>Letzter interessanter Moment</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>Unternehmen</td>
      <td>Unternehmensname</td>
      <td>companyname</td>
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
      <td>mkt_frequency</td>
    </tr>
    <tr>
      <td>Betreff</td>
      <td>Thema</td>
      <td>subject</td>
    </tr>
    <tr>
      <td>Jahresumsatz</td>
      <td>Jahresumsatz</td>
      <td>umsatz</td>
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
      <td>ownerid</td>
    </tr>
    <tr>
      <td>created on</td>
      <td>createdon</td>
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
      <td>createdon</td>
    </tr>
    <tr>
      <td>Anrede</td>
      <td>Anrede</td>
      <td>salutation</td>
    </tr>
    <tr>
      <td>Zuerst</td>
      <td>Vorname</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>Zweiter Vorname</td>
      <td>Zweiter Vorname</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>Zuletzt</td>
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
    </tr>
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
    </tr>
    <tr>
      <td>Postleitzahl</td>
      <td>Adresse 1: Postleitzahl</td>
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
      <td>Telefonaufrufe nicht zulassen</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>Abbestellt</td>
      <td>Massen-E-Mail nicht</td>
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
      <td>Telefonnummer (privat)</td>
      <td>telephone2</td>
    </tr>
    <tr>
      <td>Von Microsoft bevorzugte Kontaktmethode</td>
      <td>bevorzugte Kontaktmethode</td>
      <td>preferredContextMethodencode</td>
    </tr>
    <tr>
      <td>Letztes interessantes Datum</td>
      <td>Letztes interessantes Datum</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>Letzter interessanter Moment</td>
      <td>Letzter interessanter Moment</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>Letzte interessante Moment-Quelle</td>
      <td>Letzte interessante Moment-Quelle</td>
      <td>mkt_leadinterestingmomentsource</td>
    </tr>
    <tr>
      <td>Letzter interessanter Moment desc</td>
      <td>Letzter interessanter Moment desc</td>
      <td>mkt_lastinterestingmomentdesc</td>
    </tr>
    <tr>
      <td>Microsoft – Kein Marketingmaterial senden</td>
      <td>Marketing-Material</td>
      <td>donotsendmm</td>
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
      <td>mkt_frequency</td>
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
      <td>ownerid</td>
    </tr>
    <tr>
      <td>created on</td>
      <td>createdon</td>
    </tr>
    <tr>
      <td>parentcustomerid</td>
      <td>Unternehmensname</td>
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
      <td>Kontonummer</td>
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
      <td>Website</td>
      <td>website</td>
    </tr>
    <tr>
      <td>Anzahl Mitarbeiter</td>
      <td>Anzahl der Mitarbeiter</td>
      <td>Anzahl der Beschäftigten</td>
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
      <td>Anzahl der Beschäftigten</td>
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
      <td>ownerid</td>
    </tr>
    <tr>
      <td>created on</td>
      <td>createdon</td>
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
      <td>nächste Wahrscheinlichkeit</td>
    </tr>
    <tr>
      <td>Phase</td>
      <td>Status</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>Tatsächliches Abschlussdatum</td>
      <td>Tatsächliches Abschlussdatum</td>
      <td>actualclosedate</td>
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
      <td>ownerid</td>
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

Die folgenden Felder werden in Marketo erstellt, können jedoch nicht von Benutzern angepasst werden.

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
      <td>In MS Dynamics erstelltes Datum (kann sich von dem in Marketo erstellten unterscheiden)</td>
    </tr>
    <tr>
      <td>Microsoft wird gelöscht</td>
      <td>Person, die früher in Microsoft war, aber gelöscht wurde und jetzt nur noch in Marketo lebt</td>
    </tr>
  </tbody>
</table>
