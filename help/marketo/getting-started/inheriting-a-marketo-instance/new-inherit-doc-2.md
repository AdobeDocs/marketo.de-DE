---
description: Vererben von Dokument 2 - Marketo-Dokumente - Produktdokumentation
title: Erben von Doc 2
hide: true
hidefromtoc: true
source-git-commit: 4b726947bfaf9f8e4dcf48076e1148124fb46d25
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 9%

---

# Erben von Doc 2 {#inherit-doc-2}

Haben Sie eine vorhandene Marketo Engage-Instanz von einem anderen Administrator übernommen? Wenn ja, ist dieser Artikel für Sie.

>[!TIP]
>
>Wenn Sie ein neuer Marketo Engage-Benutzer sind und nicht mit vielen der Begriffe vertraut sind, sehen Sie sich bitte die [Marketo-Glossar](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## Smart Lists für System {#system-smart-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Alle Personen</td> 
   <td><li>Wie viele Personen gibt es in der <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md" target="_blank">Datenbank</a>?</li>
<li>Wenn Ihre Datenbank nahezu vollständig ist, empfiehlt Ihre Unternehmensrichtlinie, die Datenbankgröße zu erweitern oder historische Daten zu bereinigen?</li>
<li>Ist Ihre Datenbank zu mindestens 85 % vermarktbar? 
<br/>Wenn Ihre Site unter diesen Schwellenwert fällt, sollten Sie sich die anderen System-Smart-Listen (Blockierungsliste, Marketing ausgesetzt, Duplikate, Abmeldung) mit größerer Sorgfalt ansehen.</li></td>
  </tr>
  <tr> 
   <td>Abgemeldete Person</td> 
   <td><li>Nach welchen Kriterien sind Sie für <a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md" target="_blank">abgemeldete Personen</a>? Gibt es zu viele abgemeldete Personen?</li>
<li>Stimmen Ihre Abmeldemethoden mit Ihren Datenschutzanforderungen überein?</li>
<li>Ist Ihre Voreinstellung zur Abmeldung aktuell? Wie lange sind Datensätze in Ihrer Datenbank noch nicht vermarktbar?</li></td>
  </tr>
  <tr> 
   <td>Marketing eingestellt</td> 
   <td><li>Nach welchen Kriterien sind Sie für <a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md#marketing-suspended" target="_blank">Marketing ausgesetzt</a>? Gibt es zu viele Personen, die Marketing ausgesetzt haben?</li>
<li>Wie lange sind Datensätze im Status Ausgesetzt des Marketing erhalten geblieben?</li>
<p>Anwendungsbeispiel für Marketing ausgesetzt: Datensätze, die aktiv am Vertrieb beteiligt sind, in verspäteten Gelegenheiten, für die Sie Marketing-Kommunikation unterdrücken möchten.</td>
  </tr>
   <tr> 
   <td>Blockierungsliste</td> 
   <td><li>Nach welchen Kriterien sind Sie für <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md" target="_blank">auf die Blockierungsliste setzend Datensätze</a>? Gibt es zu viele auf die Blockierungsliste gesetzt?</li></td>
  </tr>
  <tr> 
   <td>Unzustellbare E-Mail-Adressen</td> 
   <td><li>Text</li></td>
  </tr>
  <tr> 
   <td>Mögliche Duplikate</td> 
   <td><li>Wie viele <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md" target="_blank">potenziell doppelte Datensätze</a> Gibt es sie?
   <br/>Ziehen Sie das Löschen oder Zusammenführen in Erwägung.</li></td>
  </tr>
   <tr> 
   <td>Kein Akquisitionsprogramm</td> 
   <td><li>Wie viele Menschen haben keine <a href="/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md#acquisition-program" target="_blank">Akquiseprogramm</a>?
   <br/>Wenn es viel gibt, überlegen Sie, warum.</li></td>
  </tr>
 </tbody> 
</table>

## Smart Lists für Gruppen {#group-smart-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Smart Lists für Gruppen</td> 
   <td><li>Welche Smart-Listen gibt es? Wie werden sie in dieser Instanz verwendet?</li>
<li>Sind die Listen in einer zusammenhängenden Ordnerstruktur organisiert? <br/>Wenn Sie verwaiste Listen haben, sollten Sie Ihren Baum so organisieren, dass Assets einfach zu finden sind.</li>
<p>Tipp: <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md#archive-a-folder" target="_blank">Archivieren</a> Smart-Listen gruppieren, die nicht mehr zum Abfragen, Reporting oder Verweisen benötigt werden, um die Organisation und Leistung zu unterstützen.</td>
  </tr>
 </tbody> 
</table>

## Gruppenlisten {#group-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Gruppenlisten</td> 
   <td><li>Welche Gruppenlisten gibt es?</li>
<li>Wie werden sie in dieser Instanz verwendet?</li></td>
  </tr>
 </tbody> 
</table>

## Segmentierungen {#segmentations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Segmentierungen</td> 
   <td><li>Welcher <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md" target="_blank">Segmentierungen</a> Gibt es sie? Wie werden sie verwendet?</li>
<li>Sind zu viele Personen in <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md" target="_blank">Standardsegmente</a>?</li>
<li>Gibt es eine Segmentierung für die vermarktbare Zielgruppe? 
<br/>Ist dies nicht der Fall, können Sie eine erstellen.</li></td>
  </tr>
 </tbody> 
</table>
