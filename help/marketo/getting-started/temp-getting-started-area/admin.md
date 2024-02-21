---
description: NEUER BEREICH - Marketo-Dokumente - Produktdokumentation
title: NEUER BEREICH
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 7d8cdb2da42769ee0326a3d585ad32a3405dfac1
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 8%

---

# NEU: Admin-Checkliste {#new-area-admin-checklist}

Text einfügen.

## Rollen {#roles}

<table>
<thead>
  <tr>
    <th>Bereich </th>
    <th>Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Rollen </td>
    <td><li>Überprüfen Sie die vordefinierten Rollen und bestätigen Sie, welche Berechtigungen/Zugriffsberechtigungen die einzelnen Rollen haben.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role">Neue Rolle erstellen</a> oder <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role">Rollen bearbeiten</a> basierend auf den Anforderungen Ihrer Organisation und wie oft sich Benutzer anmelden.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#assign-roles-to-a-user">Weisen Sie den entsprechenden Rollen Benutzer zu</a>.</li>
    <li>Nachdem Sie die Rollen für Benutzer zugewiesen haben, überprüfen Sie die Anzahl der Benutzer pro Rolle.</li>  <li>Implementieren Sie für jeden API-Benutzer eine eindeutige Rolle für die einfache Fehlerbehebung.</li></td>
  </tr>
  <tr>
    <td>Dokumentation </td>
    <td>Definieren Sie Benutzer und Rollen für Ihre Organisation. <br>Definieren Sie Ihren Prozess zum Hinzufügen eines neuen Benutzers/Administrators. </td>
  </tr>
  <tr>
    <td>Sandbox (falls zutreffend) </td>
    <td>Überprüfen Sie die oben genannten Kategorien für Ihre Sandbox, falls Sie eine haben. </td>
  </tr>
</tbody>
</table>

## Arbeitsbereiche und Partitionen {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th>Bereich</th>
    <th>Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Arbeitsbereiche und Partitionen </td>
    <td><li>Bestimmen Sie die Anzahl der<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html"> Arbeitsbereiche</a> und/oder Partitionen, die Ihre Organisation benötigen und <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html">wie viele Benutzer Zugriff auf die einzelnen Arbeitsbereiche haben.</a></li>
    <li>Definieren Sie den Hauptzweck jedes Arbeitsbereichs und jeder Partition.</li>
    <li>Definieren Sie die Beziehung zwischen Ihren Arbeitsbereichen und Partitionen.</li></td>
  </tr>
  <tr>
    <td>Dokumentation </td>
    <td><li>Dokumentieren Sie, wie Arbeitsbereiche definiert werden und wie sich dies auf Datenbankpartitionen bezieht (d. h. einen globalen Arbeitsbereich, der alle anzeigt, im Vergleich zu Unternehmenssektoren).</li>
    <li>Importieren Sie neue Datensätze in die entsprechende Partition.</li>
    <li>Definieren Sie den Wert in CRM, der Benutzer in die entsprechende Partition setzt.</li></td>
  </tr>
</tbody>
</table>

## Einstellungen für intelligente Kampagne {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th>Bereich</th>
    <th>Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Einstellungen für intelligente Kampagne </td>
    <td><li>Hinzufügen einer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html">Größenbeschränkung für Smart-Campaign</a>verhindert, dass versehentlich die gesamte Datenbank per E-Mail versendet wird.</li>
    <li>Personenbeschränkungen für Smart-Kampagnen aktivieren</li></td>
  </tr>
</tbody>
</table>

## E-Mail-Einstellungen {#email-settings}

<table>
<thead>
  <tr>
    <th>Bereich</th>
    <th>Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>E-Mail-Standardwerte</td>
    <td><li>Wählen Sie unter Branding Domain Ihre Domäne aus und fügen Sie Ihren E-Mail-CNAME hinzu. Dies sollte im folgenden Format erfolgen: [EmailTrackingCNAME].[Unternehmensdomäne].com.</li></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html">Einrichten von SPF und DKIM</a> für die Zustellbarkeit von E-Mails.</li></td>
  </tr>
</tbody>
</table>

## Kommunikationsbeschr {#communication-limits}

<table>
<thead>
  <tr>
    <th>Bereich</th>
    <th>Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Kommunikationsbeschr</td>
    <td><li>Ort <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html">Kommunikationsgrenzen</a>.</li>
    <li>Bestimmen Sie, ob Ihr Unternehmen eine Richtlinie zu Kommunikationsbeschränkungen benötigt.</li></td>
  </tr>
</tbody>
</table>

## Tags {#tags}

<table>
<thead>
  <tr>
    <th>Bereich</th>
    <th>Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Kanäle</td>
    <td><li>Definieren der Verwendung <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html">channels</a>.</li></td>
  </tr>
  <tr>
    <td>Tags </td>
    <td><li>Definieren der Verwendung <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">tags</a>.</li></td>
  </tr>
  <tr>
    <td>Kalender (falls zutreffend) </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html">Sitzplätze im Marketing-Kalender ausgeben</a> für Personen, die Zugriff benötigen.</li> 
    <li>Einrichten <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">Kalender</a>.</li></td>
  </tr>
</tbody>
</table>

## Datenbankverwaltung {#database-management}

<table>
<thead>
  <tr>
    <th>Bereich</th>
    <th>Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Feldverwaltung</td>
    <td><li>Implementieren der Benennungskonvention für <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank" rel="noopener noreferrer">benutzerdefinierte Felder.</a> Beginnen Sie beispielsweise mit "MKTO".</li>
    <li>Seien Sie bezüglich der zu synchronisierenden Felder selektiv. Je mehr Felder Sie synchronisieren, desto langsamer wird der Synchronisierungszyklus sein.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank" rel="noopener noreferrer">Blockieren von Aktualisierungen in Feldern</a> Sie möchten nur einmal geschrieben werden (d. h. ursprüngliche Lead-Quelle, ursprüngliche Lead-Quelldetails, UTM-Felder für Erstkontakt usw.).</li></td>
  </tr>
  <tr>
    <td>Eigene Aktivitäten </td>
    <td><li>Definieren <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank" rel="noopener noreferrer">Benutzerdefinierte Aktivitäten</a> die spezifisch für Ihr Unternehmen sind.</li></td>
  </tr>
  <tr>
    <td>Benutzerdefinierte Objekte </td>
    <td><li>Überprüfen Sie, wie viele <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank" rel="noopener noreferrer">Benutzerdefinierte Objekte</a> benötigen.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank" rel="noopener noreferrer">Diese benutzerdefinierten Objekte mit Ihrem CRM-System synchronisieren</a>.</li></td>
  </tr>
</tbody>
</table>

## Integrationen {#integrations}

<table>
<thead>
  <tr>
    <th>Bereich</th>
    <th>Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM</td>
    <td><li>Initiieren der CRM-Synchronisierung. Wählen Sie je nach dem von Ihrem Unternehmen verwendeten CRM Folgendes aus: <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html" target="_blank" rel="noopener noreferrer">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html" target="_blank" rel="noopener noreferrer">Microsoft Dynamics</a>.</li>
    <li>Bestimmen Sie den Zugriffstyp, der für den Zugriff auf Ihr CRM-System erforderlich ist.</li>
    <li>Identifizieren Sie Ihren CRM-Administrator zur Fehlerbehebung.</li></td>
  </tr>
  <tr>
    <td>Sales Insight (falls zutreffend)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html" target="_blank" rel="noopener noreferrer">Einrichten von Sales Insight.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank" rel="noopener noreferrer">Stellen Sie den entsprechenden Benutzern Sitze aus.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank" rel="noopener noreferrer">API konfigurieren</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank" rel="noopener noreferrer">Passen Sie die Lead-Bewertungen an.</a></li></td>
  </tr>
</tbody>
</table>
