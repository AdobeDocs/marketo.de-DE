---
description: Einrichten des Datenbankabschnitts für eine neue Marketo Engage-Instanz.
title: DATENBANK FÜR NEUE GEBIETE
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: 1966bc6f-9384-4c51-b3aa-57d5e52781f1
source-git-commit: 8473c4d59210bb18c3968a56883034febf00c320
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 10%

---

# NEUER BEREICH: Datenbank-Checkliste {#new-area-database-checklist}

Erfahren Sie, wie Sie die erforderlichen Schritte für den Abschnitt Datenbank in Ihrer neuen Marketo Engage-Instanz implementieren. Befolgen Sie die Anleitungen zum Implementieren einer neuen Instanz und verfolgen Sie die laufenden Aufgaben, um Sie bei der Einrichtung Ihrer Instanz für eine langfristige Effizienz zu unterstützen.

## Intelligente Listen für System {#system-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Alle Personen</td>
    <td><li>Bestimmen Sie die Implementierung einer 1:1-Synchronisation mit Ihrem CRM-System oder die Anwendung von Filtern, um zu begrenzen, wer von System zu System wechselt und wann.</li> 
    <li>Überprüfen Sie die Gesamtzahl der Personen und vermarktbaren Personen in Ihrem <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html" target="_blank">Marketo Engage-Datenbank</a>.</li></td>
  </tr>
  <tr>
    <td>Sperrliste</td>
    <td><li>Definieren Sie die Kriterien für die Blockierungsliste. Erwägen Sie, die Domänen des Konkurrenten zum <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html" target="_blank">Blockierungsliste</a> um zu verhindern, dass sie Ihre E-Mails erhalten.</li></td>
  </tr>
  <tr>
    <td>Marketing eingestellt</td>
    <td><li>Definieren <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html#marketing-suspended" target="_blank">Marketing ausgesetzt</a> Kriterien.</li></td>
  </tr>
  <tr>
    <td>Adressen für aufgrund von Bounce-Ereignissen unzustellbare E-Mails </td>
    <td><li>Definieren Sie Ihre Kriterien für nicht zugestellte E-Mail-Adressen.</li>
    <li>Überprüfen Sie die Personen in der Kategorie "E-Mail ungültig"und ob ihre E-Mails erforderlich sind. <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html" target="_blank">manuell zurücksetzen</a>.</li></td>
  </tr>
  <tr>
    <td>Mögliche Duplikate</td>
    <td><li>Überprüfen Sie Personen in der Liste Mögliche Duplikate .</li> 
    <li>Definieren Sie Ihre Strategie zur Duplikatverwaltung, um festzustellen, ob Sie <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html" target="_blank">Personen manuell zusammenführen</a>.</li>  
    <li>Wenn Sie über eine CRM-Integration verfügen, definieren Sie einen Prozess und ein Konto für <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html#effect-in-salesforce" target="_blank">Auswirkungen der Zusammenführung von Leads in Ihrem CRM</a>.</li></td>
  </tr>
  <tr>
    <td>Kein Akquisitionsprogramm</td>
    <td><li>Richten Sie Kampagnen in Ihren Programmvorlagen ein, die ein Akquiseprogramm einrichten, insbesondere bei der Verwendung globaler Formulare.</li></td>
  </tr>
  <tr>
    <td>Abbestellte Personen</td>
    <td><li>Überprüfen Sie Ihre Kriterien für <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html" target="_blank">Personen abmelden</a>.</li></td>
  </tr>
</tbody>
</table>

## Intelligente Gruppenlisten {#group-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Intelligente Gruppenlisten</td>
    <td><li>Achten Sie darauf, Smart-Listen für Gruppen zu erstellen, damit keine doppelten Listen vorhanden sind.</li>
    <li>Überwachen Sie die Master-Listen in der Datenbank.</li></td>
  </tr>
</tbody>
</table>

## Segmentierung {#segmentation}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Segmentierung</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html" target="_blank">Erstellen von Segmenten</a> auf Grundlage Ihrer Geschäftsanforderungen. Jedes Abonnement ist auf 20 Segmentierungen und 100 Segmente innerhalb jeder Segmentierung beschränkt.</li></td>
  </tr>
</tbody>
</table>
