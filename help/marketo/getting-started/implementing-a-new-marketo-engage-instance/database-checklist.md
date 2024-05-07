---
description: Richten Sie den Abschnitt Datenbank für Ihre neue Marketo Engage-Instanz ein.
title: Best Practices für neue Instanzen - Checkliste für Datenbanken
feature: Getting Started
exl-id: 996ea2db-a00c-48e5-97a8-00f869c261b1
source-git-commit: 14583b7fa148aa2b03c8cf6316b9a106c11717b7
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 9%

---

# Best Practices für neue Instanzen: Datenbank-Checkliste {#new-instance-best-practices-database-checklist}

Im Abschnitt Datenbank finden Sie die Schlüsselattribute der Personen in Ihrer Instanz. Erfahren Sie mehr über die erforderlichen Schritte, um durch verschiedene Listen und Segmentierungen in Ihrer Datenbank zu navigieren und Benutzerdatensätze zu verwalten.

Denken Sie daran, [Checklisten herunterladen](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) und verfolgen Sie Ihren Fortschritt.

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
    <td><li>Definieren Sie die Kriterien für die Blockierungsliste. Ziehen Sie in Erwägung, den Domänen von Konkurrenten zu Ihren <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html" target="_blank">Blockierungsliste</a> um zu verhindern, dass sie Ihre E-Mails erhalten.</li></td>
  </tr>
  <tr>
    <td>Marketing eingestellt</td>
    <td><li>Definieren <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe#marketing-suspended" target="_blank">Marketing ausgesetzt</a> Kriterien.</li></td>
  </tr>
  <tr>
    <td>Adressen für aufgrund von Bounce-Ereignissen unzustellbare E-Mails </td>
    <td><li>Definieren Sie Ihre Kriterien für nicht zugestellte E-Mail-Adressen.</li>
    <li>Überprüfen Sie die Personen in der Kategorie "E-Mail ungültig"und stellen Sie fest, ob ihre E-Mails benötigt werden. <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html" target="_blank">manuell zurücksetzen</a>.</li></td>
  </tr>
  <tr>
    <td>Mögliche Duplikate</td>
    <td><li>Überprüfen Sie Personen in der Liste Mögliche Duplikate .</li> 
    <li>Definieren Sie Ihre Strategie zur Duplikatverwaltung, um festzustellen, ob Sie <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html" target="_blank">Personen manuell zusammenführen</a>.</li>  
    <li>Wenn Sie über eine CRM-Integration verfügen, definieren Sie einen Prozess und ein Konto für <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people#effect-in-salesforce" target="_blank">Auswirkungen der Zusammenführung von Leads in Ihrem CRM</a>.</li></td>
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
