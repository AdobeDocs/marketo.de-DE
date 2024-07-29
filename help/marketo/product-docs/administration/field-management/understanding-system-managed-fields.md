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

Möglicherweise haben Sie bemerkt, dass die [Personen-Detailseite](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} eine Reihe von nicht bearbeitbaren Feldern enthält, die von Marketo erstellt wurden. Diese Daten stammen aus verschiedenen Quellen, und es gibt unzählige Werte, die angezeigt werden können.

## Feldtypen {#field-types}

<table><thead>
  <tr>
    <th>Feldname</th>
    <th>Definition</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ursprünglicher Quellentyp</td>
    <td>Der Ort, an dem eine Person oder ein Website-Besucher zuerst entdeckt wurde (Beispiel: Listenimport, Webseitenbesuch)</td>
  </tr>
  <tr>
    <td>Ursprüngliche Quelleninfo</td>
    <td>Details zu dieser Position (Beispiel: Name der Liste, URL der Webseite)</td>
  </tr>
  <tr>
    <td>Ursprüngliche Such-Engine</td>
    <td>Gegebenenfalls die Suchmaschine, die die Person an die ursprüngliche Einstiegsquelle verwiesen hat</td>
  </tr>
  <tr>
    <td>Ursprünglicher Suchausdruck</td>
    <td>Falls zutreffend, der verwendete Suchbegriff, der die Person an die ursprüngliche Quelle der Einsendung verwiesen hat</td>
  </tr>
  <tr>
    <td>Ursprünglicher Verweis</td>
    <td>URL, die die ursprüngliche Einstiegsquelle hostet</td>
  </tr>
  <tr>
    <td>Registrierungsquellentyp</td>
    <td>Der Ort, an dem eine Aktivität zuerst zu einer Person wurde (Beispiel: Listenimport, Webseitenbesuch)</td>
  </tr>
  <tr>
    <td>Registrierungsquelleninfo</td>
    <td>Details zu dieser Position (Beispiel: Name der Liste, URL der Webseite)</td>
  </tr>
  <tr>
    <td>Anonyme IP</td>
    <td>Gibt die IP-Adresse einer Person an</td>
  </tr>
  <tr>
    <td>Abgeleitetes Unternehmen</td>
    <td>Die beste Schätzung von Marketo (basierend auf IP) für das Unternehmen der Person</td>
  </tr>
  <tr>
    <td>Abgeleiteter Ort</td>
    <td>Die beste Schätzung von Marketo (basierend auf IP) für die Stadt der Person</td>
  </tr>
  <tr>
    <td>Abgeleitetes Bundesland/abgeleitete Region</td>
    <td>Die beste Schätzung von Marketo (basierend auf IP) des Bundesstaates oder der Region der Person</td>
  </tr>
  <tr>
    <td>Abgeleitete Postleitzahl</td>
    <td>Die beste Schätzung von Marketo (basierend auf IP) für die Postleitzahl der Person</td>
  </tr>
  <tr>
    <td>Abgeleitetes Land</td>
    <td>Die beste Schätzung von Marketo (basierend auf IP) für das Land der Person</td>
  </tr>
  <tr>
    <td>Abgeleiteter Stadtbereich</td>
    <td>Die beste Schätzung (basierend auf IP) der Metropolregion der Person durch Marketo</td>
  </tr>
  <tr>
    <td>Abgleitete Vorwahl</td>
    <td>Die beste Schätzung von Marketo (basierend auf IP) des Gebietscodes der Person</td>
  </tr>
</tbody></table>

## Mögliche Werte für den Source-Typ Original und Registrierung {#possible-values-for-original-and-registration-source-type}

Im Folgenden finden Sie einige mögliche Werte und deren Bedeutung.

<table><thead>
  <tr>
    <th>Ursprünglicher Quellentyp</th>
    <th>Definition</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Salesforce.com</td>
    <td>Person wurde bei der Salesforce-Synchronisation entdeckt</td>
  </tr>
  <tr>
    <td>Webseitenbesuche</td>
    <td>Person wurde auf einer Webseite entdeckt</td>
  </tr>
  <tr>
    <td>Webformularausfüllung</td>
    <td>Person wurde nach dem Ausfüllen eines Formulars entdeckt</td>
  </tr>
  <tr>
    <td>Listenimport</td>
    <td>Person wurde beim Listenimport entdeckt</td>
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
    <td>Sales Email</td>
    <td>Person wurde über das Sales Insight E-Mail-Add-In eine E-Mail gesendet</td>
  </tr>
  <tr>
    <td>Person</td>
    <td>Person wurde von Salesforce als Person synchronisiert</td>
  </tr>
  <tr>
    <td>Kontakt</td>
    <td>Person wurde über Webhook als Kontakt synchronisiert</td>
  </tr>
  <tr>
    <td>Munchkin-API</td>
    <td>Person wurde von der Marketo Engage Munchkin-API entdeckt</td>
  </tr>
  <tr>
    <td>Social App</td>
    <td>Person wurde von einem Social-Widget entdeckt</td>
  </tr>
  <tr>
    <td>Webdienst-API</td>
    <td>Person wurde von einer Web-Service-API entdeckt</td>
  </tr>
  <tr>
    <td>Veranstaltungspartner</td>
    <td>Person wurde über einen synchronisierten Webinardienst entdeckt</td>
  </tr>
  <tr>
    <td>Lead verknüpfen</td>
    <td>Person, die über den API-Aufruf "Associate Lead"zusammengeführt wurde</td>
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
    <td>Person durch Listenimport werden</td>
  </tr>
  <tr>
    <td>Salesforce.com</td>
    <td>Person durch Salesforce-Synchronisation werden</td>
  </tr>
  <tr>
    <td>Webformularausfüllung</td>
    <td>Person werden, nachdem ein Formular ausgefüllt wurde</td>
  </tr>
  <tr>
    <td>Sales Email</td>
    <td>Person wurde über das Sales Insight E-Mail-Add-In eine E-Mail gesendet</td>
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
    <td>Werden Sie durch die Marketo Munchkin-API zu einer Person</td>
  </tr>
  <tr>
    <td>Social App</td>
    <td>Person über ein Social Widget werden</td>
  </tr>
  <tr>
    <td>Veranstaltungspartner</td>
    <td>Person über einen verknüpften Webinar-Dienst werden</td>
  </tr>
</tbody>
</table>
