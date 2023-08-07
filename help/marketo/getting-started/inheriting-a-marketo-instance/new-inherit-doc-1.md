---
description: Vererben von Dokument 1 - Marketo-Dokumente - Produktdokumentation
title: Erben von Doc 1
hide: true
hidefromtoc: true
source-git-commit: 518c6a84dafd0882f1112caa0356f04a772832a1
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 6%

---

# Erben von Doc 1 {#inherit-doc-1}

Die Prüfung einer geerbten Instanz kann wie eine ...

Haben Sie eine vorhandene Marketo Engage-Instanz von einem anderen Administrator übernommen? Wenn ja, ist dieser Artikel für Sie...

Die folgende Checkliste wurde mit Eingaben von Marketo Champions zusammengestellt, um Ihnen dabei zu helfen, schnell in Ihrer geerbten Instanz zu arbeiten...

>[!TIP]
>
>Wenn Sie ein neuer Benutzer des Marketo Engages sind und nicht mit vielen der Begriffe vertraut sind, lesen Sie bitte den Abschnitt [Marketo-Glossar](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## Benutzer und Rollen {#users-and-roles}

<table> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
   <th>Spalte 3</th>
  </tr> 
  <tr> 
   <td>Benutzer</td> 
   <td><li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">Anzahl der Benutzer</a> Gibt es sie?</li>
<li>Gibt es Benutzer, die abgelaufen sein sollten?</li>
<li>Verfügt Ihr Unternehmen über Richtlinien zum Löschen von Benutzern?</li> 
<li>Wie viele Benutzer haben <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">Administratorberechtigungen</a>?</li>
<li>Sollte einer dieser Benutzer in <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">andere Rollen?</a></li> 
<li>Wer sind die API-Benutzer in dieser Instanz?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Rollen</td> 
   <td><li>Wie viele Rollen gibt es?</li>  
<li>Was <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">permissions/access</a> Hat jede Rolle eine Rolle? Sollte eine Anpassung vorgenommen werden?</li>
<li>Wie viele Benutzer gibt es pro Rolle?</li>
<li>Wie oft sind Benutzer <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">Anmelden</a>?</li>
<li>Gibt es für jeden API-Benutzer <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">eigene Benutzerrolle</a>? Falls nicht, sollten Sie dies implementieren, um die Fehlerbehebung zu vereinfachen.</li> 
<li>Stimmen Sie Ihre Benutzerrollen und Berechtigungen mit Ihren Unternehmensdaten überein <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">Datenschutzrichtlinien</a>?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Interne Dokumentation</td> 
   <td><li>Sind Benutzer und Rollen in Ihrer Organisation klar definiert?</li>
<li>Wie wird ein neuer Benutzer/Administrator hinzugefügt?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Sandbox (falls zutreffend)</td> 
   <td><li>Haben Sie eine <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">Sandbox-Instanz</a>? Wenn ja, überprüfen Sie die oben genannten Kategorien für Ihre Sandbox.</li>
<li>Is <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">Programmimport</a> mit Ihrer Sandbox verknüpft ist?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Audit-Trail {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
   <th>Spalte 3</th>
  </tr> 
  <tr> 
   <td>Audit-Trail</td> 
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">Wer arbeitet</a> in der Instanz?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Arbeitsbereiche und Partitionen {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
   <th>Spalte 3</th>
  </tr> 
  <tr> 
   <td>Arbeitsbereiche und Partitionen</td> 
   <td><li>Wie viele <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md" target="_blank">Arbeitsbereiche und/oder Partitionen</a> Hast du etwas?</li>
<li>Welchen Hauptzweck haben die einzelnen Arbeitsbereiche und Partition?</li>
<li>Entweder <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-a-workspace.md" target="_blank">Arbeitsbereiche</a> oder <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-an-existing-person-partition.md" target="_blank">Partitionen</a> müssen geprüft/geändert werden?</li>
<li>Welche Beziehung besteht zwischen Ihren Arbeitsbereichen und Partitionen?</li>
<li>Anzahl der Benutzer <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.md" target="_blank">Zugriff</a> zu jedem Arbeitsbereich?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Interne Dokumentation</td> 
   <td><li>Wie werden Arbeitsbereiche und Partitionen definiert?</li>
<li>Wie verläuft Ihr Prozess, um Ihrer Instanz Arbeitsbereiche hinzuzufügen oder Benutzer zu einem Arbeitsbereich hinzuzufügen?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Intelligente Kampagnen {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
   <th>Spalte 3</th>
  </tr> 
  <tr> 
   <td>Einstellungen für intelligente Kampagne</td> 
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank">Haben Sie Einschränkungen?</a> zur Größe von Smart-Kampagnen?</li>
<li>Ist dies nicht der Fall, können Sie eine hinzufügen. Es wird empfohlen, die für intelligente Kampagnen geltenden Grenzwerte auf 25 % Ihrer Datenbank zu begrenzen, um eine Überkommunikation oder Verarbeitung Ihrer gesamten Datenbank in Workflows zu vermeiden. Dies schützt nicht nur Ihre Marke, sondern schützt auch die Leistung Ihrer Instanz.</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Kommunikationsbeschränkungen {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
   <th>Spalte 3</th>
  </tr> 
  <tr> 
   <td>Kommunikationsbeschränkungen</td> 
   <td><li>Gibt es <a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">Kommunikationsbeschränkungen</a> vorhanden? Verfügt Ihr Unternehmen über Richtlinien, bei denen Kommunikationsbeschränkungen erforderlich sein könnten?</li>
<li>Adobe empfiehlt, Ihre Kommunikation auf 1 pro Tag und 3 pro 7 Tage zu begrenzen, mit <b>non</b>-<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">operativ</a> blockierte E-Mails.</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Tags {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
   <th>Spalte 3</th>
  </tr> 
  <tr> 
   <td>Tags</td> 
   <td><li>Wie viele Tags gibt es? Wie viele Tags werden verwendet? Müssen noch weitere hinzugefügt werden?</li>
<li>Sind Tags in Ihren Programmen erforderlich?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Kanäle</td> 
   <td><li>Wie viele <a href="/help/marketo/product-docs/administration/tags/create-a-program-channel.md" target="_blank">channels</a> Gibt es sie? Wie viele werden verwendet?</li>
<li>sind alle <a href="/help/marketo/product-docs/administration/tags/hide-unhide-a-program-channel.md" target="_blank">Kanalprogrammstatus, angemessen</a>? Zeigen sie Fortschritte im Rahmen des Programms?</li>
<li>Sind Ihre Kanäle mit bestimmten Programmtypen verbunden?</li>
<li>Welche Status werden für jeden Kanal als erfolgreich betrachtet? Stimmen diese mit Ihren Marketing-Zielen überein?</li>
<li>Wird der operationelle Kanal ordnungsgemäß verwendet?</li>
<li>Ist für "Erweiterter Report Builder"(Umsatz-Cycle Explorer\RCE) Ihr Kanalanalyseverhalten so eingestellt, dass es an Ihren Programmpraktiken ausgerichtet ist und die Zeitraumkosten enthält?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Marketing-Kalender (falls zutreffend)</td> 
   <td><li>Wie viele Kalendereintragstypen gibt es? Sind sie alle noch relevant?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Datenbankverwaltung {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
   <th>Spalte 3</th>
  </tr> 
  <tr> 
   <td>Feldverwaltung</td> 
   <td><li>Wie viele Felder gibt es? Klicken Sie auf "Feldnamen exportieren", um eine Liste Ihrer Felder, benutzerdefinierten Felder und deren API-Namen anzuzeigen.</li>
<li>Wie viele benutzerdefinierte Felder gibt es?</li>
<li>Wie viele Felder werden verwendet? Wählen Sie im Dropdown-Menü Feldaktionen die Option "Verwendet von exportieren"aus, um zugehörige Assets eines Felds zu überprüfen.</li>
<li>Wie viele werden zwischen Marketo Engage und Ihrem CRM synchronisiert?</li>
<li>Werden CRM-Felder mit den entsprechenden Objekten synchronisiert?</li>
<li>Gibt es eine benutzerdefinierte Ansicht für Personendetails? Sollte es denn geben?</li>
<li>Verfügen Sie über eine auf der Quelle basierende Namenskonvention für Ihre Felder? Wenn nicht, sollten Sie die Implementierung in Erwägung ziehen.</li>
<li>Sind Felder blockiert? Verstehen Sie unbedingt, warum sie sind.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Eigene Aktivitäten</td> 
   <td><li>Gibt es benutzerdefinierte Aktivitäten?</li>
<li>Wenn ja, durchklicken Sie sie, um zu verstehen, welche Aktivitäten nicht mit einem Marketo-Formular, einer E-Mail oder einer Landingpage verbunden sind.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>benutzerdefinierte -Objekte</td> 
   <td><li>Wie viele benutzerdefinierte Objekte gibt es? Wie werden sie mit Ihrem CRM synchronisiert?</li>
<li>Wie werden diese benutzerdefinierten Objekte von Ihren Programmen und Listenabfragen verwendet?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Integrationen {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
   <th>Spalte 3</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>Mit welchem CRM synchronisieren Sie? Salesforce? MS Dynamics? Veeva?</li>
<li>Ist die benutzerdefinierte Synchronisierung oder bidirektional? (KG: KORREKTUR UND BEDEUTUNG DER PRÜFUNG)</li>
<li>[Nur Salesforce] Ist für Ihre Instanz benutzerdefinierte Synchronisierungsfilter implementiert? Wenden Sie sich an den Marketo-Support, um benutzerdefinierte Synchronisierungsfilter zu ermitteln oder die Implementierung einer benutzerspezifischen Synchronisierungsregel anzufordern.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Landing Pages</td> 
   <td><li>Wie lautet die Domäne?</li>
<li>Wie lautet der Fallback?</li>
<li>Wie ist die Homepage eingestellt?</li>
<li>Ist das Vorausfüllen des Formulars aktiviert?</li>
<li>Sind personalisierte URLs aktiviert?</li>
<li>Gibt es Regeln für Umleitungen?</li>
<li>Haben Sie Domain-Aliase? Verfolgen Sie in der Dokumentation, wie Sie Ihre Domain-Aliase verwenden?</li>
<li>Ist "Sichere Domänen"für Landingpages aktiviert? Bestätigen Sie, ob Ihre Landingpage-Assets eine "http"-URL enthalten.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>Ist Ihr Munchkin-Trackingcode auf Ihrer Website (nicht in Marketo)?</li>
<li>Ist eine Browseranforderung "Nicht verfolgen"aktiviert?</li>
<li>Ist Ihre Munchkin-API konfiguriert? Wenn Ihnen die Dokumentation fehlt, in der sich der Munchkin-Code auf Ihrer Website befindet, beginnen Sie mit einer Schnellansicht. Verwenden Sie dazu den "Web Analytics-Bericht"in "Analytics", um zu verstehen, wo der Munchkin-Code auf Ihrer Website platziert wird.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Web-Services</td> 
   <td><li>Sind IP-Einschränkungen aktiviert? Sollen sie das sein?</li>
<li>Welche Benutzer/Apps führen API-Aufrufe in Ihrer Instanz durch?</li>
<li>Haben Sie Ihr API-Limit erreicht oder stehen Sie kurz davor? Falls ja, sollten Sie sie erhöhen oder Ihre Instanz überprüfen, um diese API-Aufrufe zu reduzieren.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Marketo Sales Insight (falls zutreffend)</td> 
   <td><li>Hat die <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">MSI-Paket installiert</a>?</li>
<li>Habt ihr <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">auf die neueste Version von Sales Insight aktualisiert</a>?</li>
<li>Haben Sie die Konfiguration von Sales Insight abgeschlossen? Enterprise/Unlimited-Benutzer <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">Klicken Sie hier</a>, Professional Users <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">Klicken Sie hier</a>.</li>
<li>Habt ihr <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">Zugriff auf Ihre Benutzer</a> basierend auf der Anzahl der von Ihnen erworbenen Plätze?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Startpunkt (falls zutreffend)</td> 
   <td><li>Welche Dienste haben Sie konfiguriert (Webinar, Werbung usw.)? Sind sie kurz vor ihrem Ablauf?</li>
<li>Wie viele API-Aufrufe verwenden Ihre Integrationen?</li>
<li>Verfügen Sie über die richtigen Integrationen für Ihre Anwendungsfälle?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Webhooks (falls zutreffend)</td> 
   <td><li>Welche Verbindungen haben Sie eingerichtet?</li>
<li>Wird es nicht mehr verwendet?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Mobile Apps (falls zutreffend)</td> 
   <td><li>Welche mobilen Apps haben Sie?</li>
<li>Welche Prüfgeräte wurden hinzugefügt?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Schatzkiste {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
   <th>Spalte 3</th>
  </tr> 
  <tr> 
   <td>Schatzkiste</td> 
   <td><li>Was ist in der Schatzkiste eingeschaltet?</li>
<li>Gibt es Funktionen, die aktiviert oder deaktiviert werden sollten?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Kampagnenprüfung</td> 
   <td><li>Ist der Campaign Inspector aktiviert?</li>
<li>Ist dies nicht der Fall, sollten Sie es aktivieren, um einfach festzustellen, welche Kampagnen aktiv sind, mit Ihrem CRM-System zu synchronisieren und/oder Datensätze zu löschen.</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Verschiedenes {#miscellaneous}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
   <th>Spalte 3</th>
  </tr> 
  <tr> 
   <td>Marketo Engage-Statusaktualisierungen</td> 
   <td><li>Ist Ihre Instanz für Marketo Engage-Statusaktualisierungen angemeldet?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Zugelassene Kontakte</td> 
   <td><li>Haben Sie die entsprechenden autorisierten Kontakte im Support-Portal eingerichtet?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Warnungen</td> 
   <td><li>Gibt es aktive Warnungen, die von Marketo Engage an interne Teams gesendet werden?</li>
<li>Wenn ja, funktionieren diese Ausschreibungen ordnungsgemäß?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Benachrichtigungen</td> 
   <td><li>Haben Sie entsprechende Administratorbenachrichtigungen abonniert?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>
