---
description: Checkliste für die geerbte Instanzdatenbank - Marketo-Dokumente - Produktdokumentation
title: Checkliste für die geerbte Instanzdatenbank
feature: Getting Started
source-git-commit: 092b66fe4170d571d373291f84971e2beda6d7d7
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 7%

---

# Vererbte Instanz: Datenbank-Checkliste {#inherited-instance-database-checklist}

Verstehen Sie die Gesamtzahl der Personen, vermarktbaren Personen und der Personen, die in Ihrem Abonnement die meisten Personen erwerben. Denken Sie daran, [Checklisten herunterladen](/help/marketo/getting-started/inheriting-a-marketo-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) und verfolgen Sie Ihren Fortschritt.

## Smart Lists für System {#system-smart-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Alle Personen</td> 
   <td><li>Wie viele Personen gibt es in der <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md" target="_blank">Datenbank</a>?</li>
<li>Wenn Ihre Datenbank nahezu vollständig ist, empfiehlt Ihre Unternehmensrichtlinie, die Datenbankgröße zu erweitern oder historische Daten zu bereinigen?</li>
<li>Ist Ihre Datenbank zu mindestens 85 % vermarktbar? 
<br/>     Wenn Ihre Site unter diesen Schwellenwert fällt, sollten Sie sich die anderen System-Smart-Listen (Blockierungsliste, Marketing ausgesetzt, Duplikate, Abmeldung) mit größerer Sorgfalt ansehen.</li></td>
  </tr>
  <tr> 
   <td>Abgemeldete Person</td> 
   <td><li>Nach welchen Kriterien sind Sie für <a href="/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md#marketing-suspended" target="_blank">abgemeldete Personen</a>? Gibt es zu viele abgemeldete Personen?</li>
<li>Stimmen Ihre Abmeldemethoden mit Ihren Datenschutzanforderungen überein?</li>
<li>Ist Ihre Voreinstellung zur Abmeldung aktuell? Wie lange sind Datensätze in Ihrer Datenbank noch nicht vermarktbar?</li></td>
  </tr>
  <tr> 
   <td>Marketing eingestellt</td> 
   <td><li>Nach welchen Kriterien sind Sie für <a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md#marketing-suspended" target="_blank">Marketing ausgesetzt</a>? Gibt es zu viele Personen, die Marketing ausgesetzt haben?</li>
<li>Wie lange sind Datensätze im Status Ausgesetzt des Marketing erhalten geblieben?</li>
<p>Anwendungsbeispiel für Marketing ausgesetzt : Personen erfassen aktiv mit Verkäufen in verspäteten Gelegenheiten, für die Sie Marketing-Nachrichten unterdrücken möchten.</td>
  </tr>
   <tr> 
   <td>Blockierungsliste</td> 
   <td><li>Nach welchen Kriterien sind Sie für <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md" target="_blank">auf die Blockierungsliste setzend Datensätze</a>? Gibt es zu viele auf die Blockierungsliste gesetzt?</li></td>
  </tr>
  <tr> 
   <td>Unzustellbare E-Mail-Adressen</td> 
   <td><li>Hast du viel? <a href="/help/marketo/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.md" target="_blank">Bounce-Personen</a> in Ihrer Datenbank?
   <br/>     Wenn ja, prüfen Sie, warum.</li></td></li></td>
  </tr>
  <tr> 
   <td>Mögliche Duplikate</td> 
   <td><li>Wie viele <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md" target="_blank">potenziell doppelte Datensätze</a> Gibt es sie?
   <br/>     Ziehen Sie das Löschen oder Zusammenführen in Erwägung.</li></td>
  </tr>
   <tr> 
   <td>Kein Akquisitionsprogramm</td> 
   <td><li>Wie viele Menschen haben keine <a href="/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md#acquisition-program" target="_blank">Akquiseprogramm</a>?
   <br/>     Wenn es viel gibt, überlegen Sie, warum.</li></td>
  </tr>
 </tbody> 
</table>

## Smart Lists {#smart-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Smart Lists</td> 
   <td><li>Wie viele <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md" target="_blank">Smart-Listen</a> Gibt es sie? Wie werden sie in dieser Instanz verwendet?</li>
   <p><img src="assets/note-icon.png" alt="Notizsymbol"> HINWEIS: Im Abschnitt "Datenbank"werden Smart-Listen für Gruppen vom Benutzer generiert und intelligente Systemlisten werden von Marketo Engage erstellt.
<li>Sind die Listen in einer zusammenhängenden Ordnerstruktur organisiert? 
<br/>     Wenn Sie verwaiste Listen haben, sollten Sie Ihren Baum so organisieren, dass Assets einfach zu finden sind.</li>
<p><img src="assets/tip-icon.png" alt="Tippsymbol">TIPP: <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md#archive-a-folder" target="_blank">Archivierung</a> Intelligente Listen, die nicht mehr benötigt werden, helfen bei der Organisation und Leistung.</td>
  </tr>
 </tbody> 
</table>

## Statische Listen {#static-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Statische Listen</td> 
   <td><li>Wie viele <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/understanding-static-lists.md" target="_blank">Statische Listen</a> Gibt es sie? Wie werden sie in dieser Instanz verwendet?</li>
   <p><img src="assets/note-icon.png" alt="Notizsymbol"> HINWEIS: Im Abschnitt "Datenbank"sind Gruppenlisten statische Listen.</td>
  </tr>
 </tbody> 
</table>

## Segmentierungen {#segmentations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Segmentierungen</td> 
   <td><li>Welcher <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md" target="_blank">Segmentierungen</a> Gibt es sie? Wie werden sie verwendet?</li>
<li>Sind zu viele Personen in <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md" target="_blank">Standardsegmente</a>?</li>
<li>Gibt es eine Segmentierung für die vermarktbare Zielgruppe? 
<br/>     Ist dies nicht der Fall, können Sie eine erstellen.</li></td>
  </tr>
 </tbody> 
</table>

<br> 

[Audit und geerbte Instanz: Admin](/help/marketo/getting-started/inheriting-a-marketo-instance/admin-section-checklist.md)

[Prüfen einer vererbten Instanz: Marketingaktivitäten ►](/help/marketo/getting-started/inheriting-a-marketo-instance/marketing-activities-checklist.md)
