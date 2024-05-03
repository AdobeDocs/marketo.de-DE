---
description: Dokumentieren Sie die Einrichtung Ihrer neuen Marketo Engage-Instanz.
title: Best Practices für neue Instanzen - Dokument zur Einrichtung
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c64d25e8-564b-487d-824e-7fcbfbf5d8bb
source-git-commit: 97480487268af59aac90ef64bc1ef35ee81db310
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 3%

---

# Best Practices für neue Instanzen: Dokument zur Einrichtung {#new-instance-best-practices-document-your-setup}

Nachdem Sie nun gelernt haben, die wichtigsten Produktbereiche für eine neue Marketo Engage-Instanz einzurichten, erstellen Sie als Nächstes eine Dokumentation für Ihre Instanzkonfiguration und Ihren technischen Stack. Egal, ob Sie sie über eine Tabellenkalkulation oder eine Anwendung für das Projektmanagement erstellen - Ihre Dokumentation ist eine großartige Ressource, um Fortschritte zu verfolgen und Details aufzuzeichnen sowie Ihre Instanz für zukünftige Marketing-Experten in Ihrem Unternehmen strukturiert und nachhaltig zu halten.

## Daten {#data}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Listenimport</td>
    <td><li>Zusammenstellen einer Liste von Datenquellen, aus denen Datensätze abgerufen werden <a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started-with-marketo/quick-wins/import-a-list-of-people" target="_blank">Import in Marketo Engage</a>.</li>
    <li>Wenn Sie einen Import aus mehreren Datenquellen durchführen, sollten Sie die Verwendung von Master-Listen in Erwägung ziehen oder <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo" target="_blank">Erstellen eines benutzerdefinierten Felds</a> auf dem Datensatz der Person, um die Datenquelle zu kennzeichnen.</li></td>
  </tr>
  <tr>
    <td>Datenbankintegration</td>
    <td><li>Wenn Sie die native Synchronisierung zwischen Marketo Engage und Ihrem CRM nutzen, sollten Sie sorgfältig überlegen, welche Felder zwischen den Systemen synchronisiert werden sollen. Nicht jedes Feld muss synchronisiert werden. Seien Sie also strategisch bei Ihren Datenflüssen.</li></td>
  </tr>
</tbody>
</table>

## Dokumentation {#documentation}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Benutzer</td>
    <td><li>Dokumentieren Sie <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user#add-a-user" target="_blank">aktuelle Benutzer</a> in Ihrer Instanz aus Sicherheitsgründen. Die folgenden Details sollten mindestens enthalten sein (und sind alle sichtbar, indem Sie zu Adobe Admin Console &gt; Benutzer navigieren):</li>
    <ul>
    <li>Name</li>
    <li>E-Mail</li>
    <li>Anmeldung</li>
    <li>Role</li>
    <li>Ablaufdatum des Zugriffs</li>
    <li>Benutzererstelltes Datum</li>
    <li>Letztes Anmeldungsdatum</li></ul>
    <p><img src="assets/note-icon.png" alt="Notizsymbol"> HINWEIS: Sie können dies auch erweitern und eine Dokumentation zu Rollen/Berechtigungen hinzufügen.
    <p>
    <li>Entwickeln Sie als Marketo Engage Product Admin einen internen Prozess, um die Marketo Engage-Benutzerliste regelmäßig zu überprüfen und zu aktualisieren. Um Änderungen an der Benutzerliste in Adobe Admin Console vorzunehmen, beachten Sie <a href="https://helpx.adobe.com/de/enterprise/using/users.html" target="_blank">Massenaktionen</a>, z. B. das Hochladen einer .CSV-Datei, die Verwendung der User Management-REST-API usw.</li></td>
  </tr>
  <tr>
    <td>Organization</td>
    <td><li>Dokumentieren Sie die vereinbarte Ordnerstruktur, die standardmäßigen Benennungskonventionen für Programme, Assets usw. und den Grund für die getroffenen Entscheidungen. <a href="https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/fundamentals/best-practices-to-organize-a-new-instance" target="_blank">Weitere Informationen zu Best Practices finden Sie hier .</a></li></td>
  </tr>
  <tr>
    <td>Changelog</td>
    <td><li>Erstellen Sie ein changelog , in dem Sie dokumentieren können, was sich in Ihrer Instanz ändert und warum die Änderungen vorgenommen wurden. <a href="https://experienceleague.adobe.com/en/docs/marketo-learn/auditing-an-inherited-instance/develop-an-instance-governance-guide" target="_blank">Weitere Informationen zu Best Practices finden Sie hier .</a></li></td>
  </tr>
  <tr>
    <td>Playbooks</td>
    <td><li>Erstellen Sie ein Playbook für Benutzer oder ein Playbook für Administratoren für interne Benutzer, die auf die Instanz einsteigen.</li></td>
  </tr>
  <tr>
    <td>Konversationen mit internen Teams</td>
    <td><li>Beginnen Sie damit, die Erwartungen des internen Marketingteams an die Marketo Engage mit den Marketo Engage-Funktionen abzustimmen.</li>
    <li>Identifizieren Sie die Teams, die Ihre Stakeholder in der Marketo Engage-Instanz sein werden, und dokumentieren Sie ihre Ziele für die Verwendung von Marketo Engage als Technologie.</li></td>
  </tr>
</tbody>
</table>
