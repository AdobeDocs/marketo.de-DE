---
description: Richten Sie den Abschnitt Datenbank für Ihre neue Marketo Engage-Instanz ein.
title: Best Practices für neue Instanzen - Datenbank-Checkliste
feature: Getting Started
exl-id: 996ea2db-a00c-48e5-97a8-00f869c261b1
TQID: https://experienceleague.adobe.com/yHZP1MXkAnmnz3zeucu2Bdm6FrCVtmnX9opKWiIJTAA
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 451
ht-degree: 7%

---

# Best Practices für neue Instanzen: Checkliste für Datenbank {#new-instance-best-practices-database-checklist}

Im Abschnitt Datenbank finden Sie die wichtigsten Attribute der Personen in Ihrer Instanz. Erfahren Sie mehr über die erforderlichen Schritte zum Navigieren durch verschiedene Listen und Segmentierungen in Ihrer Datenbank sowie zum Verwalten von Personendatensätzen.

Denken Sie daran[&#x200B; die Checklisten herunterzuladen &#x200B;](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) Ihren Fortschritt zu verfolgen.

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
    <td><li>Bestimmen Sie die Implementierung einer 1:1-Synchronisierung mit Ihrem CRM oder wenden Sie Filter an, um zu begrenzen, wer wann von System zu System wechselt.</li>
    <li>Überprüfen Sie die Gesamtzahl der Personen und vermarktbaren Personen in Ihrer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html?lang=de" target="_blank">Marketo Engage-</a>.</li></td>
  </tr>
  <tr>
    <td>Sperrliste</td>
    <td><li>Definieren Sie die Kriterien für die Blockierungsliste. Erwägen Sie, Ihrer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html?lang=de" target="_blank">Blockierungsliste Domänen von Mitbewerbern hinzuzufügen, </a> sie keine Ihrer E-Mails erhalten können.</li></td>
  </tr>
  <tr>
    <td>Marketing eingestellt</td>
    <td><li>Definieren Sie <a href="https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe#marketing-suspended" target="_blank">Marketing ausgesetzt</a>-Kriterien.</li></td>
  </tr>
  <tr>
    <td>Adressen für aufgrund von Bounce-Ereignissen unzustellbare E-Mails </td>
    <td><li>Definieren Sie Ihre Kriterien für unzustellbare E-Mail-Adressen.</li>
    <li>Überprüfen Sie die Personen in der Kategorie „E-Mail ungültig“ und stellen Sie fest, ob ihre E<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html?lang=de" target="_blank">Mails manuell zurückgesetzt werden </a>.</li></td>
  </tr>
  <tr>
    <td>Mögliche Duplikate</td>
    <td><li>Personen in der Liste der möglichen Duplikate überprüfen.</li>
    <li>Definieren Sie Ihre Strategie zur Duplikatverwaltung, um zu bestimmen, ob Sie <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html?lang=de" target="_blank">Personen manuell zusammenführen</a>.</li>
    <li>Wenn Sie über eine CRM-Integration verfügen, definieren Sie einen Prozess und ein Konto für <a href="https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people#effect-in-salesforce" target="_blank">die Auswirkung der Zusammenführung von Leads in Ihrem CRM</a>.</li></td>
  </tr>
  <tr>
    <td>Kein Akquisitionsprogramm</td>
    <td><li>Legen Sie in Ihren Programmvorlagen Kampagnen fest, die ein Akquise-Programm festlegen, insbesondere wenn Sie globale Formulare verwenden.</li></td>
  </tr>
  <tr>
    <td>Abbestellte Personen</td>
    <td><li>Überprüfen Sie Ihre Kriterien für <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html?lang=de" target="_blank">Abgemeldete Personen</a>.</li></td>
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
    <td><li>Achten Sie darauf, dass Sie Smart-Listen für Gruppen erstellen, damit es keine doppelten Listen gibt.</li>
    <li>Verfolgen Sie die Master-Listen in der Datenbank.</li></td>
  </tr>
</tbody>
</table>

## Segmentierung {#segmentation}

<table>
<thead>
  <tr>
    <th style="width:21%">Bereich</th>
    <th style="width:79%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Segmentierung</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html?lang=de" target="_blank">Erstellen Sie </a> Ihren Geschäftsanforderungen entsprechende Segmentierungen. Jedes Abonnement ist auf 20 Segmentierungen und 100 Segmente innerhalb jeder Segmentierung beschränkt.</li></td>
  </tr>
</tbody>
</table>
