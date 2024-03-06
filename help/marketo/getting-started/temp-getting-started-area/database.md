---
description: Einrichten des Datenbankabschnitts für eine neue Marketo Engage-Instanz.
title: DATENBANK FÜR NEUE GEBIETE
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 3cb7e5ddef8ec05a7cf8d65dd9f3bafa5dcb7da1
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 13%

---

# NEUER BEREICH: Datenbank-Checkliste {#new-area-database-checklist}

Erfahren Sie, wie Sie die erforderlichen Schritte für den Abschnitt Datenbank in Ihrer neuen Marketo Engage-Instanz implementieren. Befolgen Sie die Anleitungen zum Implementieren einer neuen Instanz und verfolgen Sie die laufenden Aufgaben, um Sie bei der Einrichtung Ihrer Instanz für eine langfristige Effizienz zu unterstützen.

## Smart Lists für System {#system-smart-lists}

<table>
<thead>
  <tr>
    <th>Bereich</th>
    <th>Aktionselemente</th>
    <th>Priorität</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Alle Personen</td>
    <td><li>Bestimmen Sie die Implementierung einer 1:1-Synchronisation mit CRM oder die Anwendung von Filtern, um zu begrenzen, wer von System zu System wechselt und wann.</li> 
    <li>Überprüfen Sie die Gesamtzahl der Personen und vermarktbaren Personen in Ihrem <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html" target="_blank" rel="noopener noreferrer">Datenbank</a>.</li></td>
    <td>Text</td>
  </tr>
  <tr>
    <td>Blockierungsliste</td>
    <td><li>Definieren Sie die Kriterien für die Blockierungsliste. Erwägen Sie das Hinzufügen der Domänen von Konkurrenten zu <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html" target="_blank" rel="noopener noreferrer">Blockierungsliste</a> um zu verhindern, dass sie Marketing- und operative E-Mails erhalten.</li></td>
    <td>Text</td>
  </tr>
  <tr>
    <td>Marketing eingestellt</td>
    <td><li>Definieren <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html#marketing-suspended" target="_blank" rel="noopener noreferrer">Marketing ausgesetzt</a> Kriterien.</li></td>
    <td>Text</td>
  </tr>
  <tr>
    <td>Unzustellbare E-Mail-Adressen </td>
    <td><li>Definieren Sie Ihre Kriterien für Bounce-E-Mail-Adressen.</li>
    <li>Überprüfen Sie die Personen in der Kategorie "E-Mail ungültig"und ob ihre E-Mails erforderlich sind. <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html" target="_blank" rel="noopener noreferrer">Manuelles Zurücksetzen</a>.</li></td>
    <td>Text</td>
  </tr>
  <tr>
    <td>Mögliche Duplikate</td>
    <td><li>Überprüfen Sie Personen in der Liste Mögliche Duplikate .</li> 
    <li>Definieren Sie Ihre Strategie zur Duplikatverwaltung, um <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html" target="_blank" rel="noopener noreferrer">Manuelles Zusammenführen von Personen</a> oder nicht.</li>  
    <li>Wenn Sie über eine CRM-Integration verfügen, sollten Sie einen Prozess und ein Konto für <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html#effect-in-salesforce" target="_blank" rel="noopener noreferrer">Auswirkungen der Zusammenführung von Leads im CRM</a>.</li></td>
    <td>Text</td>
  </tr>
  <tr>
    <td>Kein Akquisitionsprogramm</td>
    <td><li>Richten Sie Kampagnen in Ihren Programmvorlagen ein, die das Akquiseprogramm festlegen, insbesondere bei Verwendung globaler Formulare.</li></td>
    <td>Text</td>
  </tr>
  <tr>
    <td>Abgemeldete Person</td>
    <td><li>Überprüfen Sie Ihre Kriterien für <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html" target="_blank" rel="noopener noreferrer">Personen abmelden</a>.</li></td>
    <td>Text</td>
  </tr>
</tbody>
</table>

## Smart Lists für Gruppen {#group-smart-lists}

<table>
<thead>
  <tr>
    <th>Bereich</th>
    <th>Aktionselemente</th>
    <th>Priorität</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Smart Lists für Gruppen</td>
    <td><li>Achten Sie darauf, Smart-Listen für Gruppen zu erstellen, damit keine doppelten Listen vorhanden sind.</li>
    <li>Führen Sie hier in der Datenbank eine Übersicht über die Master-Listen.</li></td>
    <td>Text</td>
  </tr>
</tbody>
</table>

## Segmentierung {#segmentation}

<table>
<thead>
  <tr>
    <th>Bereich</th>
    <th>Aktionselemente</th>
    <th>Priorität</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Segmentierung</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html" target="_blank" rel="noopener noreferrer">Erstellen von Segmenten</a> auf Grundlage Ihrer Geschäftsanforderungen. Jedes Abonnement ist auf 20 Segmentierungen und 100 Segmente innerhalb jeder Segmentierung beschränkt.</li></td>
    <td>Text</td>
  </tr>
</tbody>
</table>
