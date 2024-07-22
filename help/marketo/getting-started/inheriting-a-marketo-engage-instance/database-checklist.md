---
description: Checkliste für die geerbte Instanzdatenbank - Marketo-Dokumente - Produktdokumentation
title: Checkliste für die geerbte Instanzdatenbank
feature: Getting Started
exl-id: 278a6a2f-7b68-4003-8727-129e0dc96c12
source-git-commit: 2c74c71c9311312f7e0991ed5598ccb09a9b1f15
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 7%

---

# Vererbte Instanz: Datenbank-Checkliste {#inherited-instance-database-checklist}

Verstehen Sie die Gesamtzahl der Personen, vermarktbaren Personen und der Personen, die in Ihrem Abonnement die meisten Personen erwerben. Denken Sie daran, [die Checklisten herunterzuladen](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) und Ihren Fortschritt zu verfolgen.

## Intelligente Listen für System {#system-smart-lists}

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
   <td>Abbestellte Personen</td> 
   <td><li>Nach welchen Kriterien richten Sie <a href="/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md#marketing-suspended" target="_blank">Abonnenten abmelden</a>? Gibt es zu viele abgemeldete Personen?</li>
<li>Stimmen Ihre Abmeldemethoden mit Ihren Datenschutzanforderungen überein?</li>
<li>Ist Ihre Voreinstellung zur Abmeldung aktuell? Wie lange sind Datensätze in Ihrer Datenbank noch nicht vermarktbar?</li></td>
  </tr>
  <tr> 
   <td>Marketing eingestellt</td> 
   <td><li>Welche Kriterien erfüllen Sie für <a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md#marketing-suspended" target="_blank">ausgesetztes Marketing</a>? Gibt es zu viele Personen, die Marketing ausgesetzt haben?</li>
<li>Wie lange sind Datensätze im Status Ausgesetzt des Marketing erhalten geblieben?</li>
<p>Anwendungsbeispiel für Marketing ausgesetzt : Personen erfassen aktiv mit Verkäufen in verspäteten Gelegenheiten, für die Sie Marketing-Nachrichten unterdrücken möchten.</td>
  </tr>
   <tr> 
   <td>Sperrliste</td> 
   <td><li>Nach welchen Kriterien werden Datensätze <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md" target="_blank">auf die Blockierungsliste gesetzt</a>? Gibt es zu viele auf die Blockierungsliste gesetzt?</li></td>
  </tr>
  <tr> 
   <td>Adressen für aufgrund von Bounce-Ereignissen unzustellbare E-Mails</td> 
   <td><li>Haben Sie viele <a href="/help/marketo/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.md" target="_blank">Personen, die in Ihrer Datenbank nicht mit </a> angemeldet sind?
   <br/>     Wenn ja, prüfen Sie, warum.</li></td></li></td>
  </tr>
  <tr> 
   <td>Mögliche Duplikate</td> 
   <td><li>Wie viele <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md" target="_blank">potenziell doppelte Datensätze</a> gibt es?
   <br/>     Ziehen Sie das Löschen oder Zusammenführen in Erwägung.</li></td>
  </tr>
   <tr> 
   <td>Kein Akquisitionsprogramm</td> 
   <td><li>Wie viele Personen haben kein <a href="/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md#acquisition-program" target="_blank">Akquiseprogramm</a>?
   <br/>     Wenn es viel gibt, überlegen Sie, warum.</li></td>
  </tr>
 </tbody> 
</table>

## Intelligente Listen {#smart-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Intelligente Listen</td> 
   <td><li>Wie viele <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md" target="_blank">Smart-Listen</a> gibt es? Wie werden sie in dieser Instanz verwendet?</li>
   <p><img src="assets/note-icon.png" alt="Notizsymbol"> HINWEIS: Im Abschnitt "Datenbank"werden Smart-Listen für Gruppen vom Benutzer generiert und intelligente Systemlisten werden von Marketo Engage erstellt.
<li>Sind die Listen in einer zusammenhängenden Ordnerstruktur organisiert? 
<br/>     Wenn Sie verwaiste Listen haben, sollten Sie Ihren Baum so organisieren, dass Assets einfach zu finden sind.</li>
<p><img src="assets/tip-icon.png" alt="Tippsymbol">TIPP: <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md#archive-a-folder" target="_blank">Die Archivierung</a> intelligenter Listen, die nicht mehr benötigt werden, hilft bei der Organisation und Leistung.</td>
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
   <td><li>Wie viele statische <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/understanding-static-lists.md" target="_blank">Listen</a> gibt es? Wie werden sie in dieser Instanz verwendet?</li>
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
   <td><li>Welche <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md" target="_blank">Segmentationen</a> gibt es? Wie werden sie verwendet?</li>
<li>Sind zu viele Personen in <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md" target="_blank">Standardsegmenten</a>?</li>
<li>Gibt es eine Segmentierung für die vermarktbare Zielgruppe? 
<br/>     Ist dies nicht der Fall, können Sie eine erstellen.</li></td>
  </tr>
 </tbody> 
</table>
