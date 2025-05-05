---
description: Richten Sie den Admin-Bereich für Ihre neue Marketo Engage-Instanz ein.
title: Best Practices für neue Instanzen - Checkliste für den Admin-Abschnitt
feature: Getting Started
exl-id: 4fa90a32-7e97-404c-90b1-90d05c2561d0
source-git-commit: df8087dbaf2b621d0d877eba1c16f160ee9bf460
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 6%

---

# Best Practices für neue Instanzen: Checkliste für den Admin-Abschnitt {#new-instance-best-practices-admin-section-checklist}

Wenden Sie als neuer Administrator, der in einer neuen Marketo Engage-Instanz navigiert, die folgende Checkliste an, um Sie durch den Implementierungsprozess zu führen. Wie bei allen diesen Handbüchern können Sie auch [Checklisten herunterladen](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) und Ihren Fortschritt verfolgen.

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
    <td><li>Überprüfen Sie die vordefinierten Rollen und bestätigen Sie, welche Berechtigungen/Zugriffsrechte jede Rolle hat.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=de#create-a-new-role" target="_blank">Erstellen Sie eine neue Rolle</a> oder <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=de#edit-a-role" target="_blank">bearbeiten Sie die Rollen</a> je nach den Anforderungen Ihres Unternehmens.</li>
    <li><a href="https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user" target="_blank">Weisen Sie Benutzende den entsprechenden Rollen zu</a>. Die Benutzenden müssen zum Abonnement in Adobe Admin Console hinzugefügt werden, bevor sie ihre Rollen in „Rollen“ erteilen können. Weitere Informationen finden Sie im Abschnitt Benutzer in der <a href="/help/marketo/getting-started/initial-setup/user-setup.md">Checkliste für die Ersteinrichtung</a>.</li>
    <li>Nachdem Sie die Rollen für Benutzer zugewiesen haben, überprüfen Sie die Anzahl der Benutzer pro Rolle.</li>
    <li>Implementieren Sie für jeden API-Benutzer eine eindeutige Rolle, um die Fehlerbehebung zu erleichtern.</li></td>
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
    <td><li>Bestimmen Sie die Anzahl <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html?lang=de" target="_blank"> Workspaces </a>/oder Partitionen, die Ihr Unternehmen benötigt, und <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html?lang=de" target="_blank">wie viele Benutzer Zugriff auf jeden Workspace haben.</a></li>
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
    <td><li>Fügen Sie eine <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html?lang=de" target="_blank">Einschränkung für die Größe von Smart Campaign</a> hinzu, um zu verhindern, dass versehentlich Ihre gesamte Datenbank per E-Mail versendet wird.</li></td>
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
    <td><li>Implementieren <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html?lang=de" target="_blank">Kommunikationsbeschränkungen</a>.</li>
    <li>Stellen Sie fest, ob Ihr Unternehmen eine Richtlinie zu Kommunikationsbeschränkungen benötigt.</li></td>
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
    <td><li>Definieren, wie (Kanäle<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html?lang=de" target="_blank"> verwendet </a>.</li></td>
  </tr>
  <tr>
    <td>Tags</td>
    <td><li>Definieren, wie „Tags<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html?lang=de" target="_blank"> verwendet </a>.</li></td>
  </tr>
  <tr>
    <td>Kalender<br> 
    (falls zutreffend)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html?lang=de" target="_blank">Ausgabe von Lizenzen für Marketing-Kalender</a> an diejenigen, die Zugriff benötigen.</li>
    <li>Richten Sie den <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html?lang=de" target="_blank">Kalender</a> ein.</li></td>
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
    <td><li>Implementieren Sie eine Namenskonvention für <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html?lang=de" target="_blank">benutzerdefinierte Felder</a> (z. B. beginnend mit „MKTO„).</li>
    <li>Seien Sie bezüglich der Felder, die Sie synchronisieren, selektiv. Je mehr Felder Sie synchronisieren, desto langsamer wird der Synchronisierungszyklus.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html?lang=de" target="_blank">Blockaktualisierungen von Feldern</a> die einmal geschrieben werden sollen (z. B. ursprüngliche Lead-Quelle, ursprüngliche Lead-Quelldetails, UTM-Felder für den Erstkontakt usw.).</li></td>
  </tr>
  <tr>
    <td>Eigene Aktivitäten</td>
    <td><li>Definieren Sie <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html?lang=de" target="_blank">benutzerdefinierte Aktivitäten</a> die speziell für Ihr Unternehmen gelten.</li></td>
  </tr>
  <tr>
    <td>Benutzerdefinierte Objekte</td>
    <td><li>Überprüfen Sie, wie <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html?lang=de" target="_blank"> (benutzerdefinierte Objekte</a> Sie benötigen.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html?lang=de" target="_blank">Synchronisieren Sie diese benutzerdefinierten Objekte</a> mit Ihrem CRM.</li></td>
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
    <td><li>Identifizieren Sie die Berechtigungen, die Sie für den Zugriff auf Ihr CRM benötigen.</li>
    <li>Identifizieren Sie Ihren CRM-Administrator, um Fehler zu beheben.</li></td>
  </tr>
  <tr>
    <td>Webdienste</td>
    <td><li>Bestimmen Sie die Benutzer/Apps, die <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html?lang=de" target="_blank">API-Aufrufe</a> in Ihrer Instanz ausführen können.</li>
    <li>Überprüfen Sie alle Apps, die API-Aufrufe ausführen, und stellen Sie fest, ob eine Erhöhung oder Verringerung der API-Aufrufe erforderlich ist.</li></td>
  </tr>
  <tr>
    <td>LaunchPoint</td>
    <td><li>Richten Sie <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html?lang=de" target="_blank">LaunchPoint</a>-Services für Ihr Unternehmen ein. Jeder LaunchPoint sollte mit einem eindeutigen API-Benutzer gepaart sein, um die Fehlerbehebung zu unterstützen.</li></td>
  </tr>
  <tr>
    <td>Interaktive Webinare (falls zutreffend)</td>
    <td><li>Zum Erstellen interaktiver Webinare steht auf der Registerkarte „Interaktives Webinar“ die integrierte Webinar-Funktion <a href="https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management" target="_blank">Marketo Engage. Fügen Sie Benutzende zum Abschnitt </a> hinzu.</li>
    <p><img src="assets/note-icon.png" alt="Notizensymbol"> HINWEIS: Interaktive Webinare werden nur für Produktionsinstanzen bereitgestellt.</td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (falls anwendbar)</td>
    <td><li>Weisen Sie Benutzende den <a href="https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role" target="_blank">Zugriff auf Dynamic Chat'-Rollen</a> in "Marketo Engage" &gt; „Admin“ &gt; „Benutzende und Rollen“ zu.</li></td>
  </tr>
  <tr>
    <td>Sales Insight (falls zutreffend)</td>
    <td><li><a href="https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account" target="_blank">Richten Sie die Aktion „Sales Insights</a> ein, indem Sie „Sales Insights“ &gt; „Aktionskonfiguration“ wählen.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html?lang=de#invite-individual-users-to-msi-actions" target="_blank">Problem-Lizenzen</a> an entsprechende Benutzer.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html?lang=de" target="_blank">Konfigurieren der API</a>.</li>
    <li>Anpassen der <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html?lang=de" target="_blank">Lead-Bewertungen</a>.</li></td>
  </tr>
  <tr>
    <td>Sales Connect (falls zutreffend)</td>
    <td><li>Laden Sie die entsprechenden Marketo Engage-Administratoren in die <a href="https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance" target="_blank">Sales Connect-Instanz</a> ein.</li>
    <li>Schließen Sie die <a href="https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins" target="_blank">zusätzliche Sales Connect-Admin-Einrichtung</a> in Sales Connect und Salesforce ab.</li></td>
  </tr>
  <tr>
    <td>Webhooks (falls zutreffend)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html?lang=de" target="_blank">Erstellen Sie alle erforderlichen Webhooks</a> für Ihr Unternehmen.</li>
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
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html?lang=de" target="_blank">Treasure Chest aktivieren</a> um mit Pilotfunktionen zu experimentieren.</li>
    <li>Bestimmen Sie die Funktionen, die Sie ein- oder ausschalten möchten.</li></td>
  </tr>
  <tr>
    <td>Kampagnenprüfung </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html?lang=de" target="_blank">Campaign Inspector aktivieren</a> um alle Ihre Smart-Kampagnen an einem Ort anzuzeigen.</li></td>
  </tr>
</tbody>
</table>
