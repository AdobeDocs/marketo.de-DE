---
description: Vererben Sie Doc 3 - Marketo Docs - Produktdokumentation
title: Erben von Doc 3
hide: true
hidefromtoc: true
source-git-commit: 4f833625421d7977d5aa8f59e13221a1946163f2
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 2%

---

# Erben von Doc 3 {#inherit-doc-3}

Haben Sie eine vorhandene Marketo Engage-Instanz von einem anderen Administrator übernommen? Wenn ja, ist dieser Artikel für Sie.

>[!TIP]
>
>Wenn Sie ein neuer Marketo Engage-Benutzer sind und nicht mit vielen der Begriffe vertraut sind, sehen Sie sich bitte die [Marketo-Glossar](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## Organisation {#organization}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Benennungskonventionen</td> 
   <td><li>Verfügen Ihre Programme über eine einheitliche <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#naming-schemes" target="_blank">Namenskonvention</a>?</li></td>
  </tr>
  <tr> 
   <td>Ordnerstruktur</td> 
   <td><li>Verfügen Sie über eine konsistente und leicht zu navigierende <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#folders" target="_blank">Ordnerstruktur</a>?</li></td>
  </tr>
  <tr> 
   <td>Programme</td> 
   <td><li>Gibt es ein Exzellenzzentrum mit Programmvorlagen? Wenn ja, sind die Programmvorlagen für die Anwendungsfälle der Teams sinnvoll?</li>
<li>Sind ähnliche Programmtypen <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md" target="_blank">einheitlich strukturiert</a>?</li>
<li>sind <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md" target="_blank">Zeitkosten</a> eingeführt?</li>
<li>Sind alle Programme <a href="/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md" target="_blank">mit SFDC-Kampagnen synchronisiert</a> (falls zutreffend)?</li>
<li>Verfügen Sie über Flussschritte, mit denen Sie einem <a href="/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md#acquisition-program" target="_blank">Akquiseprogramm</a> für Menschen?</li></td>
  </tr>
  <tr> 
   <td>Archivieren</td> 
   <td><li>Sind ältere Programme archiviert? Die Best Practice ist, jedes Jahr zu überprüfen.</li>
<li>Wie oft überprüft und archiviert Ihr Unternehmen alte Programme?</li></td>
  </tr>
  <tr> 
   <td>Benachrichtigungen</td> 
   <td><li>Gibt es Kampagnenfehler im Tab Benachrichtigungen oben in Ihrer Instanz?</li>
<li>Haben Sie Benachrichtigungen abonniert, um auf dem Laufenden zu bleiben, welche Fehler in der Zukunft auftreten können?</li></td>
  </tr>
  <tr> 
   <td>Abonnements mit intelligenter Liste 
   <br/>(Registerkarte Marketingaktivitäten/Abonnements )</td> 
   <td><li>Gibt es in Ihrer Instanz fortlaufende Smart-List-Abonnements? Wenn ja, wer wird sie dann tun?</li>
<li>Erwägen Sie die Einrichtung von Smart-List-Abonnements, um einen Teamalias und nicht einen Kontakt aufzurufen. Dies betrifft Sie für den Fall, dass Einzelpersonen im Urlaub oder Urlaub sind.</li></td>
  </tr>
 </tbody> 
</table>

## Assets {#assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Token</td> 
   <td><li>Werden Token in regelmäßig verwendeten Programmtypen verwendet? Wenn nicht, sollten Sie sie zur Effizienzsteigerung in Erwägung ziehen.</li>
<li>Wenn Token implementiert sind, gibt es globale Ordner-Token? Wie werden sie verwendet?</li></td>
  </tr>
  <tr> 
   <td>Engagementprogramme</td> 
   <td><li>Gibt es aktive Pflegeprogramme?</li>
<li>Wie viele Leute sind erschöpft? Wenn es viele erschöpfte Personen gibt, sollten Sie Inhalt hinzufügen.</li>
<li>Sind die Menschen mit den Inhalten der Pflege beschäftigt? Falls nicht, sollten Sie den Inhalt und/oder die A/B-Tests aktualisieren.</li>
<li>Wie viele Personen sind an mehr als einem Interaktionsprogramm beteiligt? Sollen sie mehrere sein?</li></td>
  </tr>
  <tr> 
   <td>Stapelkampagnen</td> 
   <td><li>Wie viele wiederkehrende Batch-Kampagnen gibt es?</li>
<li>Sollen sie deaktiviert/archiviert werden?</li></td>
  </tr>
   <tr> 
   <td>Auslöserkampagnen</td> 
   <td><li>Wie viele Trigger-Kampagnen gibt es?</li>
<li>Sollen sie deaktiviert/archiviert werden?</li>
<li>Sollten Trigger-Kampagnen in Batch-Kampagnen geändert werden, um die Verarbeitungseffizienz zu verbessern?</li></td>
  </tr>
  <tr> 
   <td>Lokaler Forms</td> 
   <td><li>Wie viele Programme haben lokale Formulare? Sollen diese Formulare in globale Formulare umgewandelt werden?</li>
<li>Erfassen sie geeignete Daten für Ihre Marketing- und Verkaufsteams?</li>
<p>Tipp: Begrenzen Sie die Anzahl lokaler Formulare, um die Aktualisierung und Anpassung an Änderungen an den Datenschutz-, Opt-in-/Opt-out-Richtlinien zu vereinfachen. Bei der Erstellung eines Formulars sollten Sie bedenken, welche Fragen gestellt werden müssen, ob sich die erfassten Informationen nicht ändern und sich die erweiterte Formularfunktion nicht ändert. Nehmen Sie als Beispiel ein globales Formular anstelle eines lokalen Formulars.</td>
  </tr>
  <tr> 
   <td>Globale Formulare</td> 
   <td><li>Wo werden globale Formulare verwendet? (Marketo-Landingpages im Vergleich zu Nicht-Marketo-Landingpages)</li>
<li>Wie weisen Ihre globalen Formulare Benutzer auf eine Dankeseite zu? (über ausgeblendetes Formularfeld oder in der CMS-Seitenvorlage)</li>
<li>Gibt es Formularfelder, die Sie hinzufügen oder entfernen sollten?</li>
<li>Gibt es Picklist-Werte, die Sie ändern sollten?</li>
<li>Müssen Sie progressives Profiling in Erwägung ziehen?</li>
<li>Sind all Ihre erforderlichen Felder für die CRM-Synchronisierung und die Marketing-Anforderungen enthalten?</li>
<li>Berücksichtigen Ihre globalen Formulare Ihre Datenschutz- und gesetzlichen Anforderungen für die Opt-in-Strategie und -Verwaltung?</li></td>
  </tr>
 </tbody> 
</table>

## Operationelle Programme {#operational-programs}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Personenbewertung</td> 
   <td><li>Haben Sie ein zentralisiertes Personenbewertungsprogramm?</li>
<li>Erhöht oder verringert Ihre Personenermittlung die Punktzahl?</li></td>
  </tr>
  <tr> 
   <td>Personen-Quelle</td> 
   <td><li>Verfügen Sie über ein zentralisiertes Programm, das den Feldern der Personenquelle Werte zuordnet?</li>
<p>Hinweis: Marketo Engage erfasst automatisch Daten in einem Quellfeld, unabhängig von den operationellen Programmen</td>
  </tr>
  <tr> 
   <td>Datenstandardisierung</td> 
   <td><li>Verfügen Sie über ein zentralisiertes Programm zur Standardisierung der eingehenden Daten?</li></td>
  </tr>
  <tr> 
   <td>Bounce Management</td> 
   <td><li>Haben Sie ein zentralisiertes Programm, um mit Bounce-Leuten umzugehen?</li></td>
  </tr>
  <tr> 
   <td>Datenschutz und Compliance</td> 
   <td><li>Verfügen Sie über Programme, um sicherzustellen, dass Sie die Datenschutzgesetze und Spam-Gesetze einhalten? Betrachten Sie DSGVO, CASL, CAN-SPAM, CCPA usw.</li>
<p>Tipp: Denken Sie daran, sich immer an Ihr Rechtsabteilung zu diesen Fragen zu wenden. Fragen Sie Ihr Team nach früheren Initiativen, um die Einhaltung zu gewährleisten, bevor Sie Änderungen vornehmen.</td>
  </tr>
  <tr> 
   <td>Lebensdauer</td> 
   <td><li>Haben Sie ein Programm, um Menschen durch Ihren Lebenszyklus zu bewegen?</li>
<li>Welche Werte sind für den Status der Person verfügbar?</li></td>
  </tr>
  <tr> 
   <td>E-Mail-Zustellbarkeit</td> 
   <td><li>Rufen Sie einen E-Mail-Leistungsbericht für Sendungen ab, die in den letzten Monaten gesendet wurden. Wie sieht die Zustellbarkeit von E-Mails aus?</li>
<li>Wenn die E-Mail-Zustellbarkeit schlecht ist, sollten Sie Best Practices für die Zustellbarkeit von E-Mails wie SPF und DKIM untersuchen und implementieren.</li>
<li>Stehen Sie in Kontakt mit Ihrem kompletten marktfähigen Publikum?</li></td>
  </tr>
  <tr> 
   <td>Abonnement-/Voreinstellungszentrum</td> 
   <td><li>Haben Sie ein An-/Abmeldezentrum eingerichtet? Funktioniert es so, wie es sollte?</li></td>
  </tr>
  <tr> 
   <td>Interessante Momente (falls zutreffend)</td> 
   <td><li>Haben Sie ein Programm oder Fluss-Schritte in Programmen, um interessante Momente passend an Salesforce zu senden?</li></td>
  </tr>
 </tbody> 
</table>
