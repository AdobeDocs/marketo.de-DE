---
description: Standardmäßige Feldzuordnung für Dynamiken - Marketing-Dokumente - Produktdokumentation
title: Standardmäßige Feldzuordnung für Dynamik
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 1%

---


# Standardmäßige Feldzuordnung für Dynamik {#default-dynamics-field-mapping}

Wenn Sie Ihr Marketo-Konto zunächst mit Microsoft synchronisieren, stellt Marketo automatisch diese Verbindungen zwischen Ihren integrierten Dynamics- und Marketo-Feldern her.  Marketo synchronisiert auch Ihre benutzerdefinierten Felder auf Ihren Leads, Konten, Chancen und Kontakten.

## Interessentenfelder {#lead-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Markierungsfeld</th> 
   <th>MS Dynamics Field</th> 
   <th>MS Dynamics API-Name</th> 
  </tr> 
  <tr> 
   <td>Microsoft Created Date</td> 
   <td>Erstellt am</td> 
   <td>createdon</td> 
  </tr> 
  <tr> 
   <td>Anrede</td> 
   <td>Anrede</td> 
   <td>Anrede</td> 
  </tr> 
  <tr> 
   <td>Erster</td> 
   <td>Vorname</td> 
   <td>firstname</td> 
  </tr> 
  <tr> 
   <td>Mittel</td> 
   <td>Mittlerer Name</td> 
   <td>middlename</td> 
  </tr> 
  <tr> 
   <td>Letzte</td> 
   <td>Nachname</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>Email</td> 
   <td>Email</td> 
   <td>emailaddress1</td> 
  </tr> 
  <tr> 
   <td>Auftragstitel</td> 
   <td>Titel</td> 
   <td>jobtitle</td> 
  </tr> 
  <tr> 
   <td>Telefon</td> 
   <td>Business Phone</td> 
   <td>telephone1</td> 
  </tr> 
  <tr> 
   <td>Mobilnummer</td> 
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
   <td>state</td> 
   <td>Bundesland/-staat</td> 
   <td>address1_stateorprovinz</td> 
  </tr> 
  <tr> 
   <td>Land</td> 
   <td>Land/Region</td> 
   <td>address1_country</td> 
  </tr> 
  <tr> 
   <td>Postleitzahl</td> 
   <td>PLZ/Postleitzahl</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>Personalquelle</td> 
   <td>Interessentenquelle</td> 
   <td>leadsourcecode</td> 
  </tr> 
  <tr> 
   <td>Personenstand</td> 
   <td>Status</td> 
   <td>statecode</td> 
  </tr> 
  <tr> 
   <td>Statusgrund</td> 
   <td>Statusgrund</td> 
   <td>statuscode</td> 
  </tr> 
  <tr> 
   <td>Personenknoten</td> 
   <td>Beschreibung</td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td>Nicht aufrufen</td> 
   <td>Telefonanrufe nicht zulassen</td> 
   <td>donotphone</td> 
  </tr> 
  <tr> 
   <td>Nicht abonniert</td> 
   <td>Keine Massen-E-Mail</td> 
   <td>donotbulkemail</td> 
  </tr> 
  <tr> 
   <td>Personenbewertung</td> 
   <td>Beurteilung</td> 
   <td>Leadqualitycode</td> 
  </tr> 
  <tr> 
   <td>Microsoft-Adresse 2</td> 
   <td>Straße 2</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Microsoft-Adresse 3</td> 
   <td>Straße 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Microsoft nicht per E-Mail senden</td> 
   <td>E-Mails nicht zulassen</td> 
   <td>Donotemail</td> 
  </tr> 
  <tr> 
   <td>Microsoft Do Not Fax</td> 
   <td>Faxe nicht zulassen</td> 
   <td>donotfax</td> 
  </tr> 
  <tr> 
   <td>Microsoft sendet kein Marketingmaterial</td> 
   <td>Marketingmaterial</td> 
   <td>donotsendmm</td> 
  </tr> 
  <tr> 
   <td>Microsoft Home Phone</td> 
   <td>Home Phone</td> 
   <td>telephone2</td> 
  </tr> 
  <tr> 
   <td>Bevorzugte Microsoft-Kontaktmethode</td> 
   <td>Bevorzugte Kontaktmethode</td> 
   <td>preferConactmethodcode</td> 
  </tr> 
  <tr> 
   <td>Microsoft-Thema</td> 
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
   <th>Markierungsfeld</th> 
   <th>MS Dynamics Field</th> 
   <th>MS Dynamics API-Name</th> 
  </tr> 
  <tr> 
   <td>Microsoft Created Date</td> 
   <td>Erstellt am</td> 
   <td>createdon</td> 
  </tr> 
  <tr> 
   <td>Anrede</td> 
   <td>Anrede</td> 
   <td>Anrede</td> 
  </tr> 
  <tr> 
   <td>Erster</td> 
   <td>Vorname</td> 
   <td>firstname</td> 
  </tr> 
  <tr> 
   <td>Mittel</td> 
   <td>Mittlerer Name</td> 
   <td>middlename</td> 
  </tr> 
  <tr> 
   <td>Letzte</td> 
   <td>Nachname</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>Email</td> 
   <td>Email</td> 
   <td>emailaddress1</td> 
  </tr> 
  <tr> 
   <td>Auftragstitel</td> 
   <td>Auftragstitel</td> 
   <td>jobtitle</td> 
  </tr> 
  <tr> 
   <td>Telefon</td> 
   <td>Business Phone</td> 
   <td>telephone1</td> 
  </tr> 
  <tr> 
   <td>Mobilnummer</td> 
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
   <td>state</td> 
   <td>Adresse 1: Bundesland/-staat</td> 
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
   <td>Personenstand</td> 
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
   <td>Nicht abonniert</td> 
   <td>Keine Massen-E-Mail</td> 
   <td>donotbulkemail</td> 
  </tr> 
  <tr> 
   <td>Microsoft-Adresse 2</td> 
   <td>Adresse 1: Straße 2</td> 
   <td>address1_line2</td> 
  </tr> 
   <tr> 
   <td>Microsoft-Adresse 3</td> 
   <td>Adresse 1: Straße 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Microsoft nicht per E-Mail senden</td> 
   <td>E-Mails nicht zulassen</td> 
   <td>Donotemail</td> 
  </tr> 
  <tr> 
   <td>Microsoft Home Phone</td> 
   <td>Home Phone</td> 
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
   <th>Markierungsfeld</th> 
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
   <td>Rechnungsstadt</td> 
   <td>Adresse 1: Ort</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>Rechnungsland</td> 
   <td>Adresse 1: Land/Region</td> 
   <td>address1_country</td> 
  </tr> 
  <tr> 
   <td>Postleitzahl der Rechnungsstellung</td> 
   <td>Adresse 1: PLZ/Postleitzahl</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>Microsoft-Rechnungsadresse 2</td> 
   <td>Adresse 1: Straße 2</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Microsoft-Rechnungsadresse 3</td> 
   <td>Adresse 1: Straße 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Hauptfach</td> 
   <td>Hauptfach</td> 
   <td>telephone1</td> 
  </tr> 
  <tr> 
   <td>Geschäftstyp</td> 
   <td>Geschäftstyp</td> 
   <td>businessStypecode</td> 
  </tr> 
  <tr> 
   <td>Microsoft-Kontonummer</td> 
   <td>Kontonummer</td> 
   <td>accountNumber</td> 
  </tr> 
  <tr> 
   <td>Microsoft Firma-Status</td> 
   <td>Status</td> 
   <td>statecode</td> 
  </tr> 
  <tr> 
   <td>Jahresumsatz</td> 
   <td>Jahresumsatz</td> 
   <td>Umsatz</td> 
  </tr> 
  <tr> 
   <td>Hinweise zur Firma</td> 
   <td>Beschreibung</td> 
   <td>description</td> 
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
   <td>Webseite</td> 
   <td>Webseite</td> 
   <td>website</td> 
  </tr> 
 </tbody> 
</table>

## Microsoft-bezogene Systemfelder in Marketo (schreibgeschützt) {#microsoft-related-system-fields-in-marketo}

Diese Felder werden in Marketo erstellt, können aber nicht von Kunden angepasst werden.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Markierungsfeld</th> 
   <th>Beschreibung</th> 
  </tr> 
  <tr> 
   <td>Microsoft-Typ</td> 
   <td>Interessent oder Kontakt. Wenn leer, existiert der Interessent nur als Person in Marketo</td> 
  </tr> 
  <tr> 
   <td>Microsoft Created Date</td> 
   <td>In MS Dynamics erstelltes Datum (kann sich von Erstellt in Marketo unterscheiden)</td> 
  </tr> 
  <tr> 
   <td>Microsoft wird gelöscht</td> 
   <td>Person war früher bei Microsoft, wurde aber gelöscht und lebt jetzt nur in Marketo</td> 
  </tr> 
 </tbody> 
</table>
