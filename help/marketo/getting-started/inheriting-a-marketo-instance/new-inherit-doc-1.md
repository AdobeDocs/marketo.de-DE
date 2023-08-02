---
description: Vererben von Dokument 1 - Marketo-Dokumente - Produktdokumentation
title: Erben von Doc 1
hide: true
hidefromtoc: true
source-git-commit: b6628cee17799801815f5b84c424399538eaf5ee
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 10%

---

# Erben von Doc 1 {#inherit-doc-1}

Die Prüfung einer geerbten Instanz kann wie eine

Haben Sie eine vorhandene Marketo Engage-Instanz von einem anderen Administrator übernommen? Wenn ja, ist dieser Artikel für Sie.

>[!TIP]
>
>Wenn Sie ein neuer Benutzer des Marketo Engages sind und nicht mit vielen der Begriffe vertraut sind, lesen Sie bitte den Abschnitt [Marketo-Glossar](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## Benutzer und Rollen {#users-and-roles}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
   <th>Spalte 3</th>
  </tr> 
  <tr> 
   <td>Benutzer</td> 
   <td><li>Wie viele Benutzer gibt es?</li>
<li>Gibt es Benutzer, die abgelaufen sein sollten?</li>
<li>Verfügt Ihr Unternehmen über Richtlinien zum Löschen von Benutzern?</li> 
<li>Wie viele Benutzer haben Administratorberechtigungen?</li>
<li>Sollte einer dieser Benutzer in andere Rollen geändert werden?</li> 
<li>Wer sind die API-Benutzer in dieser Instanz?</li></td>
   <td>3,1</td>
  </tr>
  <tr> 
   <td>Rollen</td> 
   <td><li>Wie viele Rollen gibt es?</li>  
<li>Welche Berechtigungen/Zugriffsberechtigungen hat jede Rolle? Sollte eine Anpassung vorgenommen werden?</li>
<li>Wie viele Benutzer gibt es pro Rolle?</li>
<li>Wie oft melden sich Benutzer an?</li>
<li>Verfügt jeder API-Benutzer über eine eigene Benutzerrolle? Falls nicht, sollten Sie dies implementieren, um die Fehlerbehebung zu vereinfachen.</li> 
<li>Stimmen Ihre Benutzerrollen und Berechtigungen mit Ihren Datenschutzrichtlinien für Unternehmensdaten überein?</li></td>
   <td>3,2</td>
  </tr>
  <tr> 
   <td>Interne Dokumentation</td> 
   <td><li>Sind Benutzer und Rollen in Ihrer Organisation klar definiert?</li>
<li>Wie wird ein neuer Benutzer/Administrator hinzugefügt?</li></td>
   <td>3.3</td>
  </tr>
  <tr> 
   <td>Sandbox (falls zutreffend)</td> 
   <td><li>Haben Sie eine Sandbox-Instanz? Wenn ja, überprüfen Sie die oben genannten Kategorien für Ihre Sandbox.</li>
<li>Ist der Programm-Import mit Ihrer Sandbox verknüpft?</li></td>
   <td>3,4</td>
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
   <td><li>Wer arbeitet in der Instanz?</li></td>
   <td>3.1</td>
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
   <td><li>Wie viele Arbeitsbereiche und/oder Partitionen haben Sie?</li>
<li>Welchen Hauptzweck haben die einzelnen Arbeitsbereiche und Partition?</li>
<li>Müssen sie überprüft oder geändert werden?</li>
<li>Welche Beziehung besteht zwischen Ihren Arbeitsbereichen und Partitionen?</li>
<li>Wie viele Benutzer haben Zugriff auf die einzelnen Arbeitsbereiche?</li></td>
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
   <td><li>Haben Sie eine Einschränkung der Größe von Smart-Kampagnen?</li>
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
   <td><li>Gibt es Beschränkungen? Verfügt Ihr Unternehmen über Richtlinien, bei denen Kommunikationsbeschränkungen erforderlich sein könnten?</li>
<li>Adobe empfiehlt, Ihre Kommunikation auf 1 pro Tag und 3 pro 7 Tage zu begrenzen, wobei nicht operative E-Mails blockiert werden.</li></td>
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
   <td><li>Wie viele Kanäle gibt es? Wie viele werden verwendet?</li>
<li>Sind alle Status des Kanalprogramms angemessen? Zeigen sie Fortschritte im Rahmen des Programms?</li>
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
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Marketo Sales Insight (falls zutreffend)</td> 
   <td><li>Wurde das MSI-Paket installiert?</li>
<li>Haben Sie auf die neueste Version von Sales Insight aktualisiert?</li>
<li>Haben Sie die Konfiguration von Sales Insight abgeschlossen?</li>
<li>Haben Sie Ihren Benutzern Zugriff auf die von Ihnen erworbenen Plätze gewährt?</li></td>
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
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
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
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
 </tbody> 
</table>
