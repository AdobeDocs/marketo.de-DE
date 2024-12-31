---
unique-page-id: 5472615
description: Grundlegendes zu systemverwalteten Feldern - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zu systemverwalteten Feldern
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: fc25a088005ee1d552f6e61e2fa7b953e2fde862
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 16%

---

# Grundlegendes zu systemverwalteten Feldern {#understanding-system-managed-fields}

Möglicherweise haben Sie bemerkt, dass die [Personendetailseite](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} eine Reihe von nicht bearbeitbaren Feldern enthält, die von Marketo erstellt wurden. Diese Daten stammen aus verschiedenen Quellen und es gibt unzählige Werte, die angezeigt werden könnten.

## Feldtypen {#field-types}

<table><thead>
  <tr>
    <th>Feldname</th>
    <th>Definition</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ursprünglicher Quellentyp</td>
    <td>Der Ort, an dem eine Person oder ein Website-Besucher zum ersten Mal erkannt wurde (Beispiel: Listen-Import, Web-Seitenbesuch)</td>
  </tr>
  <tr>
    <td>Ursprüngliche Quelleninfo</td>
    <td>Besonderheiten in Bezug auf diesen Speicherort (Beispiel: Name der Liste, URL der Web-Seite)</td>
  </tr>
  <tr>
    <td>Ursprüngliche Such-Engine</td>
    <td>Gegebenenfalls die Suchmaschine, die die Person an die ursprüngliche Einreisequelle verwiesen hat</td>
  </tr>
  <tr>
    <td>Ursprünglicher Suchausdruck</td>
    <td>Falls zutreffend, der verwendete Suchbegriff, der die Person auf die ursprüngliche Einstiegsquelle verwies</td>
  </tr>
  <tr>
    <td>Ursprünglicher Verweis</td>
    <td>URL, die die ursprüngliche Eintragsquelle gehostet hat</td>
  </tr>
  <tr>
    <td>Registrierungsquellentyp</td>
    <td>Der Ort, an dem eine Aktivität erstmals eine Person wurde (Beispiel: Listen-Import, Web-Seitenbesuch)</td>
  </tr>
  <tr>
    <td>Registrierungsquelleninfo</td>
    <td>Besonderheiten in Bezug auf diesen Speicherort (Beispiel: Name der Liste, URL der Web-Seite)</td>
  </tr>
  <tr>
    <td>Anonyme IP</td>
    <td>Gibt die IP-Adresse einer Person an</td>
  </tr>
  <tr>
    <td>Abgeleitetes Unternehmen</td>
    <td>Marketos beste Schätzung (basierend auf IP) des Unternehmens der Person</td>
  </tr>
  <tr>
    <td>Abgeleiteter Ort</td>
    <td>Marketos beste Schätzung (basierend auf IP) der Stadt der Person</td>
  </tr>
  <tr>
    <td>Abgeleitetes Bundesland/abgeleitete Region</td>
    <td>Marketos beste Schätzung (basierend auf IP) des Bundesstaats oder der Region der Person</td>
  </tr>
  <tr>
    <td>Abgeleitete Postleitzahl</td>
    <td>Marketos beste Schätzung (basierend auf IP) der Postleitzahl der Person</td>
  </tr>
  <tr>
    <td>Abgeleitetes Land</td>
    <td>Marketos beste Schätzung (basierend auf IP) des Landes der Person</td>
  </tr>
  <tr>
    <td>Abgeleiteter Stadtbereich</td>
    <td>Marketos beste Schätzung (basierend auf IP) des Ballungsraums der Person</td>
  </tr>
  <tr>
    <td>Abgleitete Vorwahl</td>
    <td>Marketos beste Schätzung (basierend auf IP) des Gebietscodes der Person</td>
  </tr>
</tbody></table>

## Mögliche Werte für den Source-Typ „Original“ und „Registrierung“ {#possible-values-for-original-and-registration-source-type}

Im Folgenden finden Sie einige mögliche Werte und ihre Bedeutung.

<table><thead>
  <tr>
    <th>Ursprünglicher Quellentyp</th>
    <th>Definition</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Salesforce.com</td>
    <td>Person wurde bei der Salesforce-Synchronisierung erkannt</td>
  </tr>
  <tr>
    <td>Web-Seitenbesuche</td>
    <td>Person wurde von einer Webseite entdeckt</td>
  </tr>
  <tr>
    <td>Web-Formular-Filllout</td>
    <td>Person wurde nach dem Ausfüllen eines Formulars erkannt</td>
  </tr>
  <tr>
    <td>Listenimport</td>
    <td>Person wurde von einem Listenimport entdeckt</td>
  </tr>
  <tr>
    <td>Neue Person</td>
    <td>Person wurde manuell in die Datenbank eingegeben</td>
  </tr>
  <tr>
    <td>Weblink-Klick</td>
    <td>Person wurde nach dem Klicken auf einen Link erkannt</td>
  </tr>
  <tr>
    <td>Verkaufs-E-Mail</td>
    <td>Person wurde eine E-Mail über Sales Insight Email Add-In gesendet</td>
  </tr>
  <tr>
    <td>Person</td>
    <td>Person wurde von Salesforce als Person synchronisiert</td>
  </tr>
  <tr>
    <td>Kontakt</td>
    <td>Person wurde von Webhook als Kontakt synchronisiert</td>
  </tr>
  <tr>
    <td>Munchkin-API</td>
    <td>Person wurde von der Marketo Engage Munchkin-API erkannt</td>
  </tr>
  <tr>
    <td>Social App</td>
    <td>Person wurde von einem Social-Widget entdeckt</td>
  </tr>
  <tr>
    <td>Webdienst-API</td>
    <td>Person wurde von einer Webservice-API erkannt</td>
  </tr>
  <tr>
    <td>Veranstaltungspartner</td>
    <td>Person wurde durch einen synchronisierten Webinar-Service erkannt</td>
  </tr>
  <tr>
    <td>Lead verknüpfen</td>
    <td>Person, die über den Aufruf der Associate Lead-API zusammengeführt wurde</td>
  </tr>
</tbody></table>

<table><thead>
  <tr>
    <th>Registrierungsquellentyp</th>
    <th>Definition</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Listenimport</td>
    <td>Durch einen Listenimport zu einer Person geworden</td>
  </tr>
  <tr>
    <td>Salesforce.com</td>
    <td>Durch Salesforce-Synchronisierung zu einer Person wurde</td>
  </tr>
  <tr>
    <td>Web-Formular-Filllout</td>
    <td>Person wurde, nachdem ein Formular ausgefüllt wurde</td>
  </tr>
  <tr>
    <td>Verkaufs-E-Mail</td>
    <td>Person wurde eine E-Mail über Sales Insight Email Add-In gesendet</td>
  </tr>
  <tr>
    <td>Webdienst-API</td>
    <td>Person wurde über die SOAP/REST-API erstellt</td>
  </tr>
  <tr>
    <td>Neue Person</td>
    <td>Person wurde manuell in die Datenbank eingegeben</td>
  </tr>
  <tr>
    <td>Munchkin-API</td>
    <td>Person über die Munchkin-API von Marketo</td>
  </tr>
  <tr>
    <td>Social App</td>
    <td>Über ein soziales Widget zu einer Person geworden</td>
  </tr>
  <tr>
    <td>Veranstaltungspartner</td>
    <td>Person durch einen verknüpften Webinar-Service geworden</td>
  </tr>
</tbody>
</table>
