---
description: Dokumentieren Sie die Einrichtung Ihrer neuen Marketo Engage-Instanz.
title: Best Practices für neue Instanzen - Dokumentieren der Einrichtung
feature: Getting Started
exl-id: c64d25e8-564b-487d-824e-7fcbfbf5d8bb
source-git-commit: 14583b7fa148aa2b03c8cf6316b9a106c11717b7
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 3%

---

# Best Practices für neue Instanzen: Dokumentieren Sie Ihre Einrichtung {#new-instance-best-practices-document-your-setup}

Nachdem Sie nun die wichtigsten Produktbereiche kennen, die für eine neue Marketo Engage-Instanz eingerichtet werden müssen, erstellen Sie als nächsten Schritt eine Dokumentation für Ihre Instanzkonfiguration und Ihren Tech-Stack. Egal, ob Sie sie über eine Tabelle oder eine Projektmanagement-Anwendung erstellen, Ihre Dokumentation ist eine großartige Ressource, um den Fortschritt zu verfolgen und Details aufzuzeichnen sowie Ihre Instanz für zukünftige Marketing-Fachleute in Ihrem Unternehmen strukturiert und nachhaltig zu halten.

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
    <td><li>Erfassen Sie eine Liste der Datenquellen, aus denen Datensätze abgerufen werden (<a href="https://experienceleague.adobe.com/de/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people" target="_blank"> in Marketo Engage importieren</a>.</li>
    <li>Wenn Sie Daten aus mehreren Datenquellen importieren, sollten Sie Master-Listen verwenden oder <a href="https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo" target="_blank">ein benutzerdefiniertes Feld erstellen</a> im Personendatensatz verwenden, um die Datenquelle zu kennzeichnen.</li></td>
  </tr>
  <tr>
    <td>Datenbankintegration</td>
    <td><li>Wenn Sie die native Synchronisierung zwischen Marketo Engage und Ihrem CRM nutzen, überlegen Sie sorgfältig, welche Felder Sie zwischen den Systemen synchronisieren möchten. Nicht jedes Feld muss synchronisiert werden. Gehen Sie daher bei Ihren Datenflüssen strategisch vor.</li></td>
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
    <td><li>Dokumentieren Sie aus <a href="https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user#add-a-user" target="_blank"> die </a> Benutzer in Ihrer Instanz. Die folgenden Details sollten mindestens enthalten sein (und alle sind sichtbar, wenn Sie zu Admin &gt; Benutzer und Rollen gehen):</li>
    <ul>
    <li>Name</li>
    <li>E-Mail</li>
    <li>Anmeldung</li>
    <li>Role</li>
    <li>Ablaufdatum des Zugriffs</li>
    <li>Erstellungsdatum des Benutzers</li>
    <li>Datum der letzten Anmeldung</li></ul>
    <p><img src="assets/note-icon.png" alt="Notizensymbol"> HINWEIS: Sie können dies auch erweitern, um Dokumentationen zu Rollen/Berechtigungen einzuschließen.
    <p>
    <li>Entwickeln Sie als Marketo Engage-Produktadministrator einen internen Prozess, um die Marketo Engage-Benutzerliste regelmäßig zu überprüfen und zu aktualisieren. Wenn Sie Änderungen an der Benutzerliste in Adobe Admin Console vornehmen möchten, sollten Sie Massenaktionen <a href="https://helpx.adobe.com/de/enterprise/using/users.html" target="_blank">, </a>. B. das Hochladen einer CSV-Datei, die Verwendung der User Management-REST-API usw.</li></td>
  </tr>
  <tr>
    <td>Organisation</td>
    <td><li>Dokumentieren Sie die vereinbarte Ordnerstruktur, die standardmäßigen Benennungskonventionen für Programme, Assets usw. und die Gründe für die getroffenen Entscheidungen. <a href="https://experienceleague.adobe.com/de/docs/marketo-learn/tutorials/fundamentals/best-practices-to-organize-a-new-instance" target="_blank">Weitere Informationen zu den Best Practices finden Sie hier.</a></li></td>
  </tr>
  <tr>
    <td>Änderungsprotokoll</td>
    <td><li>Erstellen Sie ein Änderungsprotokoll, in dem Sie die Änderungen in Ihrer Instanz und die Gründe für die Änderungen dokumentieren können. <a href="https://experienceleague.adobe.com/de/docs/marketo-learn/auditing-an-inherited-instance/develop-an-instance-governance-guide" target="_blank">Weitere Informationen zu den Best Practices finden Sie hier.</a></li></td>
  </tr>
  <tr>
    <td>Playbooks</td>
    <td><li>Erstellen Sie ein Benutzer- oder Admin-Playbook für interne Benutzer, die in die Instanz einsteigen.</li></td>
  </tr>
  <tr>
    <td>Gespräche mit internen Teams</td>
    <td><li>Stimmen Sie die Erwartungen des internen Marketing-Teams an das Marketo Engage mit den Funktionen der Marketo Engage ab.</li>
    <li>Identifizieren Sie die Teams, die Ihre Stakeholder in der Marketo Engage-Instanz sein werden, und dokumentieren Sie ihre Ziele für die Verwendung von Marketo Engage als Technologie.</li></td>
  </tr>
  <tr>
    <td>Arbeitsbereiche und Partitionen (falls zutreffend)</td>
    <td><li>Dokumentieren Sie, wie Arbeitsbereiche definiert werden und wie sich dies auf Datenbankpartitionen bezieht (z. B. ein globaler Arbeitsbereich, der alle im Vergleich zu Geschäftssektoren zeigt).</li>
    <li>Importieren Sie neue Einträge in die entsprechende Partition.</li>
    <li>Definieren Sie den Wert in Ihrem CRM, der Benutzer in der entsprechenden Partition platziert.</li></td>
  </tr>
</tbody>
</table>
