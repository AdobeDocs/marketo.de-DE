---
description: Standardmäßige Dynamics-Feldzuordnung - Marketo-Dokumente - Produktdokumentation
title: Dynamische Standardfeldzuordnung
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '1036'
ht-degree: 2%

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
      <td>[!UICONTROL Microsoft Erstellungsdatum]</td>
      <td>[!UICONTROL erstellt am]</td>
      <td>createdOn</td>
    </tr>
    <tr>
      <td>[!UICONTROL Anrede]</td>
      <td>[!UICONTROL Anrede]</td>
      <td>Begrüßung</td>
    </tr>
    <tr>
      <td>[!UICONTROL First]</td>
      <td>[!UICONTROL Vorname]</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>[!UICONTROL Middle]</td>
      <td>[!UICONTROL zweiter Vorname]</td>
      <td>MiddleName</td>
    </tr>
    <tr>
      <td>[!UICONTROL Letzte]</td>
      <td>[!UICONTROL Nachname]</td>
      <td>lastname</td>
    </tr>
    <tr>
      <td>[!UICONTROL E-Mail]</td>
      <td>[!UICONTROL E-Mail]</td>
      <td>emailAddress1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Auftragstitel]</td>
      <td>[!UICONTROL Auftragstitel]</td>
      <td>Stellenbezeichnung</td>
    </tr>
    <tr>
      <td>[!UICONTROL Phone]</td>
      <td>[!UICONTROL Business Phone]</td>
      <td>Telefon 1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Mobile]</td>
      <td>[!UICONTROL Mobiltelefon]</td>
      <td>Mobiltelefon</td>
    </tr>
    <tr>
      <td>[!UICONTROL Fax]</td>
      <td>[!UICONTROL Fax]</td>
      <td>Fax</td>
    </tr>
    <tr>
      <td>[!UICONTROL-Adresse]</td>
      <td>[!UICONTROL Straße 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Stadt]</td>
      <td>[!UICONTROL Stadt]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL-Status]</td>
      <td>[!UICONTROL Bundesland/Provinz]</td>
      <td>address1_stateorProvince</td>
    </tr>
    <tr>
      <td>[!UICONTROL Land]</td>
      <td>[!UICONTROL Land/Region]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL Postleitzahl]</td>
      <td>[!UICONTROL Postleitzahl]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Person Source]</td>
      <td>[!UICONTROL Lead Source]</td>
      <td>Lead-Quellcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Personenstatus]</td>
      <td>[!UICONTROL Status]</td>
      <td>Zustandscode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Status Reason]</td>
      <td>[!UICONTROL Status Reason]</td>
      <td>statuscode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Personennotizen]</td>
      <td>[!UICONTROL Beschreibung]</td>
      <td>Beschreibung</td>
    </tr>
    <tr>
      <td>[!UICONTROL Do not call]</td>
      <td>[!UICONTROL Telefonanrufe nicht zulassen]</td>
      <td>Donotphone</td>
    </tr>
    <tr>
      <td>[!UICONTROL abgemeldet]</td>
      <td>[!UICONTROL Nicht als Massennachricht senden]</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Personenbewertung]</td>
      <td>[!UICONTROL Bewertung]</td>
      <td>LeadQualityCode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft-Adresse 2]</td>
      <td>[!UICONTROL Straße 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft-Adresse 3]</td>
      <td>[!UICONTROL Straße 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Nicht E-Mail senden]</td>
      <td>[!UICONTROL E-Mails nicht zulassen]</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft kein Fax]</td>
      <td>[!UICONTROL lässt keine Faxe zu]</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft sendet kein Marketingmaterial]</td>
      <td>[!UICONTROL Marketingmaterial]</td>
      <td>donotsendm</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Home Phone]</td>
      <td>[!UICONTROL Telefon privat]</td>
      <td>Telefon2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Bevorzugte Kontaktmethode von Microsoft]</td>
      <td>[!UICONTROL Bevorzugte Kontaktmethode]</td>
      <td>PreferredContactMethodCode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft-Thema]</td>
      <td>[!UICONTROL Topic]</td>
      <td>Subjekt</td>
    </tr>
    <tr>
      <td>[!UICONTROL Datum des letzten interessanten Moments]</td>
      <td>[!UICONTROL Datum des letzten interessanten Moments]</td>
      <td>mkt_lastInterestingMomentDate</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last Interesting Moment desc]</td>
      <td>[!UICONTROL Last Interesting Moment desc]</td>
      <td>mkt_lastInterestedMomentdesc</td>
    </tr>
    <tr>
      <td>[!UICONTROL Quelle des letzten interessanten Moments]</td>
      <td>[!UICONTROL Quelle des letzten interessanten Moments]</td>
      <td>mkt_leadInterestedMomentsource</td>
    </tr>
    <tr>
      <td>[!UICONTROL Typ des letzten interessanten Moments]</td>
      <td>[!UICONTROL Typ des letzten interessanten Moments]</td>
      <td>mkt_lastInterestingMomentType</td>
    </tr>
    <tr>
      <td>[!UICONTROL Firma]</td>
      <td>[!UICONTROL Firmenname]</td>
      <td>companyName</td>
    </tr>
    <tr>
      <td>[!UICONTROL relative Bewertung]</td>
      <td>[!UICONTROL relative Bewertung]</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>[!UICONTROL-Priorität]</td>
      <td>[!UICONTROL-Priorität]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL Relative Dringlichkeit]</td>
      <td>[!UICONTROL-Dringlichkeit]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL Betreff]</td>
      <td>[!UICONTROL Topic]</td>
      <td>Subjekt</td>
    </tr>
    <tr>
      <td>[!UICONTROL Jahresumsatz]</td>
      <td>[!UICONTROL Jahresumsatz]</td>
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
      <td>[!UICONTROL Inhaber] </td>
      <td>ownerID</td>
    </tr>
    <tr>
      <td>[!UICONTROL erstellt am]</td>
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
      <td>[!UICONTROL Microsoft Erstellungsdatum]</td>
      <td>[!UICONTROL erstellt am]</td>
      <td>createdOn</td>
    </tr>
    <tr>
      <td>[!UICONTROL Anrede]</td>
      <td>[!UICONTROL Anrede]</td>
      <td>Begrüßung</td>
    </tr>
    <tr>
      <td>[!UICONTROL First]</td>
      <td>[!UICONTROL Vorname]</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>[!UICONTROL Middle]</td>
      <td>[!UICONTROL zweiter Vorname]</td>
      <td>MiddleName</td>
    </tr>
    <tr>
      <td>[!UICONTROL Letzte]</td>
      <td>[!UICONTROL Nachname]</td>
      <td>lastname</td>
    </tr>
    <tr>
      <td>[!UICONTROL E-Mail]</td>
      <td>[!UICONTROL E-Mail]</td>
      <td>emailAddress1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Auftragstitel]</td>
      <td>[!UICONTROL Auftragstitel]</td>
      <td>Stellenbezeichnung</td>
    </tr>
    <tr>
      <td>[!UICONTROL Phone]</td>
      <td>[!UICONTROL Business Phone]</td>
      <td>Telefon 1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Mobile]</td>
      <td>[!UICONTROL Mobiltelefon]</td>
      <td>Mobiltelefon</td>
    </tr>
    <tr>
      <td>[!UICONTROL-Adresse]</td>
      <td>[!UICONTROL Adresse 1: Straße 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Stadt]</td>
      <td>[!UICONTROL Adresse 1: Stadt]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL-Status]</td>
      <td>[!UICONTROL Adresse 1: Bundesland/Region]</td>
      <td>address1_stateorProvince</td>
    </tr>
    <tr>
      <td>[!UICONTROL Land]</td>
      <td>[!UICONTROL Adresse 1: Land/Region]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL Postleitzahl]</td>
      <td>[!UICONTROL Adresse 1: Postleitzahl]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Personenstatus]</td>
      <td>[!UICONTROL Status]</td>
      <td>Zustandscode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Status Reason]</td>
      <td>[!UICONTROL Status Reason]</td>
      <td>statuscode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Do not call]</td>
      <td>[!UICONTROL Telefonanrufe nicht zulassen]</td>
      <td>Donotphone</td>
    </tr>
    <tr>
      <td>[!UICONTROL abgemeldet]</td>
      <td>[!UICONTROL Nicht als Massennachricht senden]</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft-Adresse 2]</td>
      <td>[!UICONTROL Adresse 1: Straße 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft-Adresse 3]</td>
      <td>[!UICONTROL Adresse 1: Straße 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Nicht E-Mail senden]</td>
      <td>[!UICONTROL E-Mails nicht zulassen]</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Home Phone]</td>
      <td>[!UICONTROL Telefon privat]</td>
      <td>Telefon2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Bevorzugte Kontaktmethode von Microsoft]</td>
      <td>[!UICONTROL Bevorzugte Kontaktmethode]</td>
      <td>PreferredContactMethodCode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Datum des letzten interessanten Moments]</td>
      <td>[!UICONTROL Datum des letzten interessanten Moments]</td>
      <td>mkt_lastInterestingMomentDate</td>
    </tr>
    <tr>
      <td>[!UICONTROL Typ des letzten interessanten Moments]</td>
      <td>[!UICONTROL Typ des letzten interessanten Moments]</td>
      <td>mkt_lastInterestingMomentType</td>
    </tr>
    <tr>
      <td>[!UICONTROL Quelle des letzten interessanten Moments]</td>
      <td>[!UICONTROL Quelle des letzten interessanten Moments]</td>
      <td>mkt_leadInterestedMomentsource</td>
    </tr>
    <tr>
      <td>[!UICONTROL Last Interesting Moment desc]</td>
      <td>[!UICONTROL Last Interesting Moment desc]</td>
      <td>mkt_lastInterestedMomentdesc</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft sendet kein Marketingmaterial]</td>
      <td>[!UICONTROL Marketingmaterial]</td>
      <td>donotsendm</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft kein Fax]</td>
      <td>[!UICONTROL Microsoft kein Fax]</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>[!UICONTROL-Priorität]</td>
      <td>[!UICONTROL-Priorität]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL Relative Dringlichkeit]</td>
      <td>[!UICONTROL-Dringlichkeit]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL relative Bewertung]</td>
      <td>[!UICONTROL relative Bewertung]</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>[!UICONTROL Personennotizen]</td>
      <td>[!UICONTROL Beschreibung]</td>
      <td>Beschreibung </td>
    </tr>
    <tr>
      <td>[!UICONTROL Personenbewertung]</td>
      <td>[!UICONTROL Lead-Bewertung]</td>
      <td>mkt_leadscore</td>
    </tr>
    <tr>
      <td>[!UICONTROL Personennotizen]</td>
      <td>[!UICONTROL Beschreibung]</td>
      <td>Beschreibung </td>
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
      <td>[!UICONTROL Inhaber] </td>
      <td>ownerID</td>
    </tr>
    <tr>
      <td>[!UICONTROL erstellt am]</td>
      <td>createdOn</td>
    </tr>
    <tr>
      <td>[!UICONTROL Firmenname]</td>
      <td>parentCustomerID</td>
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
      <td>[!UICONTROL-Konto (a)]</td>
      <td>[!UICONTROL-Konto]</td>
      <td>accountid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Rechnungsadresse]</td>
      <td>[!UICONTROL Adresse 1: Straße 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Abrechnungsstadt]</td>
      <td>[!UICONTROL Adresse 1: Stadt]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL Rechnungsland]</td>
      <td>[!UICONTROL Adresse 1: Land/Region]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL Postleitzahl für Rechnungsstellung]</td>
      <td>[!UICONTROL Adresse 1: Postleitzahl]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Rechnungsadresse 2]</td>
      <td>[!UICONTROL Adresse 1: Straße 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Rechnungsadresse 3]</td>
      <td>[!UICONTROL Adresse 1: Straße 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Haupttelefon]</td>
      <td>[!UICONTROL Haupttelefon]</td>
      <td>Telefon 1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Geschäftstyp]</td>
      <td>[!UICONTROL Geschäftstyp]</td>
      <td>BusinessTypeCode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft-Kontonummer]</td>
      <td>[!UICONTROL Kontonummer]</td>
      <td>Kontonummer</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Unternehmensstatus]</td>
      <td>[!UICONTROL Status]</td>
      <td>Zustandscode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Jahresumsatz]</td>
      <td>[!UICONTROL Jahresumsatz]</td>
      <td>Umsatz</td>
    </tr>
    <tr>
      <td>[!UICONTROL Firmennotizen]</td>
      <td>[!UICONTROL Beschreibung]</td>
      <td>Beschreibung</td>
    </tr>
    <tr>
      <td>[!UICONTROL Industry]</td>
      <td>[!UICONTROL Industry]</td>
      <td>Branchencode</td>
    </tr>
    <tr>
      <td>[!UICONTROL SIC-Code]</td>
      <td>[!UICONTROL SIC-Code]</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>[!UICONTROL-Website]</td>
      <td>[!UICONTROL-Website]</td>
      <td>Website</td>
    </tr>
    <tr>
      <td>[!UICONTROL Anzahl Mitarbeiter]</td>
      <td>[!UICONTROL Anzahl der Mitarbeiter]</td>
      <td>Anzahl der Mitarbeiter</td>
    </tr>
    <tr>
      <td>[!UICONTROL SIC-Code]</td>
      <td>[!UICONTROL SIC-Code]</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>[!UICONTROL Firma]</td>
      <td>[!UICONTROL Kontoname]</td>
      <td>name</td>
    </tr>
    <tr>
      <td>[!UICONTROL Anzahl Mitarbeiter]</td>
      <td>[!UICONTROL Anzahl der Mitarbeiter]</td>
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
      <td>[!UICONTROL Inhaber] </td>
      <td>ownerID</td>
    </tr>
    <tr>
      <td>[!UICONTROL erstellt am]</td>
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
      <td>[!UICONTROL Abschlusswahrscheinlichkeit]</td>
      <td>[!UICONTROL-Wahrscheinlichkeit]</td>
      <td>Nahwahrscheinlichkeit</td>
    </tr>
    <tr>
      <td>[!UICONTROL-Phase]</td>
      <td>[!UICONTROL Status]</td>
      <td>Zustandscode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Tatsächliches Abschlussdatum]</td>
      <td>[!UICONTROL Tatsächliches Abschlussdatum]</td>
      <td>actualCloseDate</td>
    </tr>
    <tr>
      <td>[!UICONTROL Name]</td>
      <td>[!UICONTROL Topic]</td>
      <td>name</td>
    </tr>
    <tr>
      <td>[!UICONTROL Geschätzter Wert]</td>
      <td>[!UICONTROL Test. Umsatz]</td>
      <td>estimatedValue</td>
    </tr>
    <tr>
      <td>[!UICONTROL Beschreibung]</td>
      <td>[!UICONTROL Beschreibung]</td>
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
      <td>[!UICONTROL Inhaber] </td>
      <td>ownerID</td>
    </tr>
    <tr>
      <td>[!UICONTROL Opportunity]</td>
      <td>OpportunityId</td>
    </tr>
    <tr>
      <td>[!UICONTROL Potenzieller Kunde]</td>
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
      <td>[!UICONTROL Microsoft-Typ]</td>
      <td>Lead oder Kontakt. Wenn leer, ist der Lead nur als Person in Marketo vorhanden</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Erstellungsdatum]</td>
      <td>Erstellungsdatum in [!DNL MS Dynamics] (kann sich von dem in Marketo unterscheiden)</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft wird gelöscht]</td>
      <td>Person war früher in Microsoft, wurde jedoch gelöscht und lebt jetzt nur noch in Marketo</td>
    </tr>
  </tbody>
</table>
