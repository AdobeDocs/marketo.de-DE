---
description: Standard-Veeva-Feldzuordnung - Marketo-Dokumente - Produktdokumentation
title: Standard-Veeva-Feldzuordnung
exl-id: 3bf36d50-daea-431f-9537-b3007ad75945
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 44%

---

# Standard-Veeva-Feldzuordnung {#default-veeva-field-mapping}

Wenn Sie Ihr Marketo Engage-Konto zum ersten Mal mit Veeva synchronisieren, führt Marketo diese Verknüpfungen automatisch zwischen Ihren integrierten Veeva- und Marketo-Feldern durch. Marketo synchronisiert auch Ihre benutzerdefinierten Felder in Ihren Konten und Kontakten.

## Kontaktfelder {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>SFDC-Feld</th>
      <th>Marketo-Feld</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Geburtsdatum</td>
      <td>Geburtsdatum</td>
    </tr>
    <tr>
      <td>Erstellungsdatum</td>
      <td>SFDC Created Date</td>
    </tr>
    <tr>
      <td>Kontaktbeschreibung</td>
      <td>Personenhinweise</td>
    </tr>
    <tr>
      <td>E-Mail</td>
      <td>E-Mail-Adresse</td>
    </tr>
    <tr>
      <td>Fax (geschäftlich)</td>
      <td>Faxnummer</td>
    </tr>
    <tr>
      <td>Vorname</td>
      <td>Vorname</td>
    </tr>
    <tr>
      <td>E-Mail-Abmeldung</td>
      <td>Abbestellt</td>
    </tr>
    <tr>
      <td>Gelöscht</td>
      <td>SFDC wurde gelöscht</td>
    </tr>
    <tr>
      <td>Nachname</td>
      <td>Nachname</td>
    </tr>
    <tr>
      <td>Lead-Quelle</td>
      <td>Quelle</td>
    </tr>
    <tr>
      <td>Lead-Bewertung</td>
      <td>Ergebnis</td>
    </tr>
    <tr>
      <td>MailingCity</td>
      <td>Stadt</td>
    </tr>
    <tr>
      <td>MailingCountry</td>
      <td>Land</td>
    </tr>
    <tr>
      <td>MailingPostalCode</td>
      <td>Postleitzahl</td>
    </tr>
    <tr>
      <td>MailingState</td>
      <td>Land</td>
    </tr>
    <tr>
      <td>MailingStreet</td>
      <td>Adresse</td>
    </tr>
    <tr>
      <td>Mobiltelefon</td>
      <td>Mobiltelefonnummer</td>
    </tr>
    <tr>
      <td>Geschäftstelefon</td>
      <td>Telefonnummer</td>
    </tr>
    <tr>
      <td>Anrede</td>
      <td>Anrede</td>
    </tr>
    <tr>
      <td>Titel</td>
      <td>Jobtitel</td>
    </tr>
  </tbody>
</table>

## Kontofelder {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>SFDC-Feld</th>
      <th>Marketo-Feld</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Jahresumsatz</td>
      <td>Jahresumsatz</td>
    </tr>
    <tr>
      <td>Abrechnungsort</td>
      <td>Abrechnungsort</td>
    </tr>
    <tr>
      <td>Abrechnungsland</td>
      <td>Abrechnungsland</td>
    </tr>
    <tr>
      <td>Postleitzahl für die Rechnungsstellung</td>
      <td>Postleitzahl für Abrechnung</td>
    </tr>
    <tr>
      <td>Fakturastaat/Provinz</td>
      <td>Bundesland für Abrechnung</td>
    </tr>
    <tr>
      <td>Abrechnungsstraße</td>
      <td>Rechnungsadresse</td>
    </tr>
    <tr>
      <td>Kontobeschreibung</td>
      <td>Unternehmenshinweise</td>
    </tr>
    <tr>
      <td>Branche</td>
      <td>Branche</td>
    </tr>
    <tr>
      <td>Gelöscht</td>
      <td>SFDC wurde gelöscht</td>
    </tr>
    <tr>
      <td>Kontoname</td>
      <td>Firmenname</td>
    </tr>
    <tr>
      <td>Mitarbeiter</td>
      <td>Anzahl Mitarbeiter</td>
    </tr>
    <tr>
      <td>Telefonnummer des Kontos</td>
      <td>Haupttelefonnummer</td>
    </tr>
    <tr>
      <td>SIC-Code</td>
      <td>SIC-Code</td>
    </tr>
    <tr>
      <td>Konto-Website</td>
      <td>Seite</td>
    </tr>
    <tr>
      <td>Kontotyp</td>
      <td>SFDC-Typ</td>
    </tr>
    <tr>
      <td>Website</td>
      <td>Website</td>
    </tr>
  </tbody>
</table>

## Veeva-bezogene Systemfelder in Marketo (schreibgeschützt) {#veeva-related-system-fields-in-marketo}

Diese Felder werden in Marketo erstellt, können von Kunden jedoch nicht angepasst werden.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>Feld</th>
      <th>Beschreibung</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Veeva ID</td>
      <td>Die 18-stellige Salesforce ID</td>
    </tr>
    <tr>
      <td>Veeva-Typ</td>
      <td>Kontakt. Wenn leer, ist der Lead nur als Person in Marketo vorhanden</td>
    </tr>
    <tr>
      <td>Veeva Created Date</td>
      <td>Erstellungsdatum in SFDC (kann sich von dem in Marketo unterscheiden)</td>
    </tr>
    <tr>
      <td>Veeva wird gelöscht</td>
      <td>Person war früher in SFDC, wurde jedoch gelöscht und lebt jetzt nur noch in Marketo</td>
    </tr>
  </tbody>
</table>
