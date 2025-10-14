---
description: Checkliste für die geerbte Instanzdatenbank - Marketo-Dokumente - Produktdokumentation
title: Checkliste für geerbte Instanzdatenbank
feature: Getting Started
exl-id: 278a6a2f-7b68-4003-8727-129e0dc96c12
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 8%

---

# Vererbte Instanz: Checkliste für Datenbank {#inherited-instance-database-checklist}

Erfahren Sie, wie viele Personen, vermarktbare Personen und die wichtigsten Personen-Akquise-Quellen in Ihrem Abonnement vorhanden sind. Denken Sie daran[&#x200B; die Checklisten herunterzuladen &#x200B;](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) Ihren Fortschritt zu verfolgen.

## Intelligente Listen für System {#system-smart-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr>
  <tr>
   <td>Alle Personen</td>
   <td><li>Wie viele Personen gibt es in der <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md" target="_blank">Datenbank</a>?</li>
<li>Wenn Ihre Datenbank fast vollständig ist, empfiehlt Ihre Unternehmensrichtlinie, Ihre Datenbankgröße zu erweitern oder historische Daten zu bereinigen?</li>
<li>Ist Ihre Datenbank insgesamt zu mindestens 85 % marktfähig?
<br/>     Wenn Ihr Abonnement unter diesen Schwellenwert fällt, sollten Sie die anderen Smart Lists des Systems (Blockierungsliste, Marketing ausgesetzt, Duplikate, Abo beenden) genauer unter die Lupe nehmen.</li></td>
  </tr>
  <tr>
   <td>Abbestellte Personen</td>
   <td><li>Nach welchen Kriterien <a href="/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md#marketing-suspended" target="_blank"> abgemeldete Personen </a>? Gibt es zu viele Abgemeldete?</li>
<li>Stimmen Ihre Abmeldemethoden mit Ihren Datenschutzanforderungen überein?</li>
<li>Ist Ihre Abmeldevoreinstellung auf dem neuesten Stand? Wie lange sind Datensätze in Ihrer Datenbank als nicht marktfähig verblieben?</li></td>
  </tr>
  <tr>
   <td>Marketing eingestellt</td>
   <td><li>Welche Kriterien gelten für <a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md#marketing-suspended" target="_blank">Marketing ausgesetzt</a>? Gibt es zu viele Personen, die das Marketing aussetzen?</li>
<li>Wie lange sind Datensätze im Status „Marketing ausgesetzt“ geblieben?</li>
<p>Anwendungsbeispiel für ausgesetztes Marketing: Personen zeichnen auf, die aktiv am Verkauf von Opportunities in der Spätphase beteiligt sind, für die Sie Marketing-Nachrichten unterdrücken möchten.</td>
  </tr>
   <tr>
   <td>Sperrliste</td>
   <td><li>Auf die Blockierungsliste setzen Nach welchen Kriterien werden <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md" target="_blank">Datensätze </a>? Gibt es zu viele Menschen, die auf die Blockierungsliste gesetzt sind?</li></td>
  </tr>
  <tr>
   <td>Adressen für aufgrund von Bounce-Ereignissen unzustellbare E-Mails</td>
   <td><li>Haben Sie viele <a href="/help/marketo/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.md" target="_blank">Personen, die gebounct haben</a> in Ihrer Datenbank?
   <br/>     Wenn ja, sollten Sie die Gründe dafür untersuchen.</li></td></li></td>
  </tr>
  <tr>
   <td>Mögliche Duplikate</td>
   <td><li>Wie viele <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md" target="_blank">potenziell doppelte Datensätze</a> gibt es?
   <br/>     Sie sollten gelöscht oder zusammengeführt werden.</li></td>
  </tr>
   <tr>
   <td>Kein Akquisitionsprogramm</td>
   <td><li>Wie viele Leute haben kein <a href="/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md#acquisition-program" target="_blank">Akquisitionsprogramm</a>?
   <br/>     Wenn es viele gibt, sollten Sie sich überlegen, warum das so ist.</li></td>
  </tr>
 </tbody>
</table>

## Intelligente Listen {#smart-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr>
  <tr>
   <td>Intelligente Listen</td>
   <td><li>Wie viele <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md" target="_blank">Smart Lists</a> gibt es? Wie werden sie in diesem Fall verwendet?</li>
   <p><img src="assets/note-icon.png" alt="Notizensymbol"> HINWEIS: Im Abschnitt „Datenbank“ werden Smart-Listen für Gruppen von Benutzern generiert, und Smart-Listen für Systeme werden standardmäßig von Marketo Engage erstellt.
<li>Sind die Listen in einer zusammenhängenden Ordnerstruktur organisiert?
<br/>     Wenn Sie verwaiste Listen haben, sollten Sie Ihren Baum so organisieren, dass Assets leicht zu finden sind.</li>
<p><img src="assets/tip-icon.png" alt="Tipp-Symbol">TIPP: <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md#archive-a-folder" target="_blank">Archivierung</a> Nicht mehr benötigte Smart Lists helfen bei Organisation und Leistung.</td>
  </tr>
 </tbody>
</table>

## Statische Listen {#static-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr>
  <tr>
   <td>Statische Listen</td>
   <td><li>Wie viele <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/understanding-static-lists.md" target="_blank">Statische Listen</a> gibt es? Wie werden sie in diesem Fall verwendet?</li>
   <p><img src="assets/note-icon.png" alt="Notizensymbol"> HINWEIS: Im Abschnitt Datenbank sind Gruppenlisten statische Listen.</td>
  </tr>
 </tbody>
</table>

## Segmentierungen {#segmentations}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr>
  <tr>
   <td>Segmentierungen</td>
   <td><li>Welche <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md" target="_blank">Segmentierungen</a> gibt es? Wie werden sie verwendet?</li>
<li>Sind zu viele Personen in <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md" target="_blank">Standardsegmenten</a>?</li>
<li>Gibt es eine Segmentierung für die vermarktbare Zielgruppe?
<br/>     Wenn nicht, sollten Sie eine erstellen.</li></td>
  </tr>
 </tbody>
</table>
