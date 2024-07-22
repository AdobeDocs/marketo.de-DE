---
description: Richten Sie den Admin-Abschnitt für Ihre neue Marketo Engage-Instanz ein.
title: Neue Best Practices für Instanzen - Checkliste für Admin-Abschnitte
feature: Getting Started
exl-id: 4fa90a32-7e97-404c-90b1-90d05c2561d0
source-git-commit: df8087dbaf2b621d0d877eba1c16f160ee9bf460
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 6%

---

# Best Practices für neue Instanzen: Checkliste für Admin-Abschnitte {#new-instance-best-practices-admin-section-checklist}

Wenden Sie als neuer Administrator, der in einer neuen Marketo Engage-Instanz navigiert, die Checkliste unten an, um Sie durch den Implementierungsprozess zu führen. Wie bei all diesen Handbüchern können Sie auch [die Checklisten herunterladen](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) und Ihren Fortschritt verfolgen.

## Rollen {#roles}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Rollen</td>
    <td><li>Überprüfen Sie die vordefinierten Rollen und bestätigen Sie, welche Berechtigungen/Zugriffsberechtigungen die einzelnen Rollen haben.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role" target="_blank">Erstellen Sie eine neue Rolle </a> oder <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role" target="_blank">bearbeiten Sie die Rollen</a> entsprechend den Anforderungen Ihres Unternehmens.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user" target="_blank">Weisen Sie den entsprechenden Rollen Benutzer zu</a>. Die Benutzer müssen zum Abonnement in Adobe Admin Console hinzugefügt werden, bevor sie ihre Rollen in "Rollen"zuweisen können. Siehe Abschnitt Benutzer in der Checkliste <a href="/help/marketo/getting-started/initial-setup/user-setup.md">Ersteinrichtung</a>.</li>
    <li>Nachdem Sie die Rollen für Benutzer zugewiesen haben, überprüfen Sie die Anzahl der Benutzer pro Rolle.</li>
    <li>Implementieren Sie für jeden API-Benutzer eine eindeutige Rolle für die einfache Fehlerbehebung.</li></td>
  </tr>
  <tr>
    <td>Sandbox (falls zutreffend)</td>
    <td><li>Überprüfen Sie die oben genannten Kategorien für Ihre <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">Sandbox</a>.</li></td>
  </tr>
</tbody>
</table>

## Arbeitsb. &amp; Partitionen {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Arbeitsbereiche und Partitionen (falls zutreffend)</td>
    <td><li>Bestimmen Sie die Anzahl der<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html" target="_blank"> Arbeitsbereiche</a> und/oder Partitionen, die Ihr Unternehmen benötigen, und <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html" target="_blank">wie viele Benutzer Zugriff auf jeden Arbeitsbereich haben.</a></li>
    <li>Definieren Sie den Hauptzweck jedes Arbeitsbereichs und jeder Partition.</li>
    <li>Definieren Sie die Beziehung zwischen Ihren Arbeitsbereichen und Partitionen.</li></td>
  </tr>
</tbody>
</table>

## Einstellungen für intelligente Kampagne {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Einstellungen für intelligente Kampagne</td>
    <td><li>Fügen Sie eine <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html" target="_blank">Beschränkung der Größe intelligenter Kampagnen</a> hinzu, um versehentlich den Versand Ihrer gesamten Datenbank zu verhindern.</li></td>
  </tr>
</tbody>
</table>

## Kommunikationsbeschränkungen {#communication-limits}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Kommunikationsbeschränkungen</td>
    <td><li>Implementieren Sie <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html" target="_blank">Kommunikationsbeschränkungen</a>.</li>
    <li>Bestimmen Sie, ob Ihr Unternehmen eine Richtlinie zu Kommunikationsbeschränkungen benötigt.</li></td>
  </tr>
</tbody>
</table>

## Tags {#tags}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Kanäle</td>
    <td><li>Definieren der Verwendung von <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html" target="_blank">Kanälen</a>.</li></td>
  </tr>
  <tr>
    <td>Tags</td>
    <td><li>Definieren Sie, wie Sie <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html" target="_blank">tags</a> verwenden.</li></td>
  </tr>
  <tr>
    <td>Kalender<br> 
    (falls zutreffend)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html" target="_blank">Stellen Sie den Benutzern, die Zugriff benötigen, Marketingkalendersitze aus.</a></li>
    <li>Richten Sie den <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html" target="_blank">Kalender</a> ein.</li></td>
  </tr>
</tbody>
</table>

## Datenbankverwaltung {#database-management}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Feldverwaltung</td>
    <td><li>Implementieren Sie eine Benennungsregel für <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank">benutzerdefinierte Felder</a> (z. B. beginnend mit "MKTO").</li>
    <li>Seien Sie bezüglich der zu synchronisierenden Felder selektiv. Je mehr Felder Sie synchronisieren, desto langsamer wird der Synchronisierungszyklus sein.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank">Blockaktualisierungen zu Feldern</a>, die Sie einmal schreiben möchten (z. B. ursprüngliche Lead-Quelle, ursprüngliche Lead-Quelldetails, UTM-Felder für Erstkontakt usw.).</li></td>
  </tr>
  <tr>
    <td>Eigene Aktivitäten</td>
    <td><li>Definieren Sie <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank">benutzerdefinierte Aktivitäten</a>, die für Ihr Unternehmen spezifisch sind.</li></td>
  </tr>
  <tr>
    <td>Benutzerdefinierte Objekte</td>
    <td><li>Überprüfen Sie, wie viele <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank">benutzerdefinierte Objekte</a> Sie benötigen.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank">Synchronisieren Sie diese benutzerdefinierten Objekte</a> mit Ihrem CRM-System.</li></td>
  </tr>
</tbody>
</table>

## Integrationen {#integrations}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM </td>
    <td><li>Bestimmen Sie die Berechtigungen, die Sie für den Zugriff auf Ihr CRM-System benötigen.</li>
    <li>Identifizieren Sie Ihren CRM-Administrator zur Fehlerbehebung.</li></td>
  </tr>
  <tr>
    <td>Webdienste</td>
    <td><li>Bestimmen Sie die Benutzer/Apps, die <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html" target="_blank">API-Aufrufe</a> in Ihrer Instanz durchführen können.</li>
    <li>Überprüfen Sie alle Apps, die API-Aufrufe durchführen, und ermitteln Sie, ob eine Erhöhung oder Verringerung der API-Aufrufe erforderlich ist.</li></td>
  </tr>
  <tr>
    <td>LaunchPoint</td>
    <td><li>Richten Sie <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">LaunchPoint</a>-Dienste für Ihr Unternehmen ein. Jeder LaunchPoint sollte mit einem eindeutigen API-Benutzer gepaart werden, um die Fehlerbehebung zu unterstützen.</li></td>
  </tr>
  <tr>
    <td>Interaktive Webinare (falls zutreffend)</td>
    <td><li>Zum Erstellen interaktiver Webinare, der integrierten Webinar-Funktion von Marketo Engage, fügen Sie <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management" target="_blank">Benutzer zum Abschnitt "Benutzer"hinzu</a> auf der Registerkarte "Interaktives Webinar".</li>
    <p><img src="assets/note-icon.png" alt="Notizsymbol"> HINWEIS: Interaktive Webinare werden nur für Produktionsinstanzen bereitgestellt.</td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (falls zutreffend)</td>
    <td><li>Weisen Sie Benutzer <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role" target="_blank">'Access Dynamic Chat'-Rollen</a> unter Marketo Engage &gt; Admin &gt; Benutzer und Rollen zu.</li></td>
  </tr>
  <tr>
    <td>Sales Insight (falls zutreffend)</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account" target="_blank">Richten Sie die Aktion "Sales Insight"</a> in Sales Insight &gt; Aktionskonfiguration ein.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank">Stellen Sie den entsprechenden Benutzern Sitzplätze </a> aus.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank">Konfigurieren Sie die API</a>.</li>
    <li>Passen Sie die <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank">Lead-Bewertungen</a> an.</li></td>
  </tr>
  <tr>
    <td>Sales Connect (falls zutreffend)</td>
    <td><li>Laden Sie die entsprechenden Marketo Engage-Administratoren zur <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance" target="_blank">Sales Connect-Instanz</a> ein.</li>
    <li>Führen Sie die <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins" target="_blank">zusätzlichen Setup des Sales Connect-Administrators</a> in Sales Connect und Salesforce aus.</li></td>
  </tr>
  <tr>
    <td>Webhooks (falls zutreffend)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html" target="_blank">Erstellen Sie alle erforderlichen Webhooks</a> für Ihr Unternehmen.</li>
    </td>
  </tr>
</tbody>
</table>

## Schatzkiste {#treasure-chest}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Schatzkiste </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html" target="_blank">Aktivieren Sie Treasure Chest</a> , um mit Piloting-Funktionen zu experimentieren.</li>
    <li>Bestimmen Sie die Funktionen, die Sie aktivieren oder deaktivieren möchten.</li></td>
  </tr>
  <tr>
    <td>Kampagnenprüfung </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html" target="_blank">Aktivieren Sie den Kampagneninspektor</a> , um alle Ihre Smart-Kampagnen an einem Ort anzuzeigen.</li></td>
  </tr>
</tbody>
</table>
