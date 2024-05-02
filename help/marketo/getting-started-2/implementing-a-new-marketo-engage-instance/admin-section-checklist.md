---
description: Richten Sie den Admin-Abschnitt für Ihre neue Marketo Engage-Instanz ein.
title: Neue Best Practices für Instanzen - Checkliste für Admin-Abschnitte
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: 4fa90a32-7e97-404c-90b1-90d05c2561d0
source-git-commit: fa5b686aabd3aab2d9020758fde00ed06564c76c
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 6%

---

# Best Practices für neue Instanzen: Checkliste für Admin-Abschnitte {#new-instance-best-practices-admin-section-checklist}

Wenden Sie als neuer Administrator, der in einer neuen Marketo Engage-Instanz navigiert, die Checkliste unten an, um Sie durch den Implementierungsprozess zu führen. Wie bei allen Handbüchern können Sie die Checklisten herunterladen [LINK] und verfolgen Sie Ihren Fortschritt.

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
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role" target="_blank">Neue Rolle erstellen</a> oder <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role" target="_blank">Rollen bearbeiten</a> basierend auf den Anforderungen Ihrer Organisation.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user" target="_blank">Weisen Sie den entsprechenden Rollen Benutzer zu</a>. Die Benutzer müssen zum Abonnement in Adobe Admin Console hinzugefügt werden, bevor sie ihre Rollen in Rollen zuweisen können. Siehe Abschnitt "Benutzer"im Abschnitt <a href="/help/marketo/getting-started-2/initial-setup/user-setup.md">Checkliste für die Ersteinrichtung</a>.</li>
    <li>Nachdem Sie die Rollen für Benutzer zugewiesen haben, überprüfen Sie die Anzahl der Benutzer pro Rolle.</li>
    <li>Implementieren Sie für jeden API-Benutzer eine eindeutige Rolle für die einfache Fehlerbehebung.</li></td>
  </tr>
  <tr>
    <td>Dokumentation</td>
    <td><li>Definieren Sie Benutzer und Rollen für Ihre Organisation.</li>
    <li>Definieren Sie Ihren Prozess zum Hinzufügen eines neuen Benutzers/Administrators.</li></td>
  </tr>
  <tr>
    <td>Sandbox (falls zutreffend)</td>
    <td><li>Überprüfen Sie die oben genannten Kategorien für Ihre <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md">Sandbox</a>.</li></td>
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
    <td><li>Bestimmen Sie die Anzahl der<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html" target="_blank"> Arbeitsbereiche</a> und/oder Partitionen, die Ihre Organisation benötigen und <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html" target="_blank">wie viele Benutzer Zugriff auf die einzelnen Arbeitsbereiche haben.</a></li>
    <li>Definieren Sie den Hauptzweck jedes Arbeitsbereichs und jeder Partition.</li>
    <li>Definieren Sie die Beziehung zwischen Ihren Arbeitsbereichen und Partitionen.</li></td>
  </tr>
  <tr>
    <td>Dokumentation</td>
    <td><li>Dokumentieren Sie, wie Arbeitsbereiche definiert werden und wie sich dies auf Datenbankpartitionen bezieht (z. B. einen globalen Arbeitsbereich, der alle Arbeitsbereiche im Vergleich zu Unternehmenssektoren anzeigt).</li>
    <li>Importieren Sie neue Datensätze in die entsprechende Partition.</li>
    <li>Definieren Sie den Wert in Ihrem CRM-System, der Benutzer in die entsprechende Partition setzt.</li></td>
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
    <td><li>Hinzufügen einer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html" target="_blank">Größenbeschränkung für Smart-Campaign</a>verhindert, dass versehentlich die gesamte Datenbank per E-Mail versendet wird.</li></td>
  </tr>
</tbody>
</table>

## E-Mail-Einstellungen {#email-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>E-Mail-Standardwerte</td>
    <td><li>Wählen Sie unter Branding Domain Ihre Domäne aus und fügen Sie Ihren E-Mail-CNAME hinzu. Dies sollte im folgenden Format erfolgen: [EmailTrackingCNAME].[Unternehmensdomäne].com.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console" target="_blank">Support für Marketo kontaktieren</a> , um es mit einer SSL-Zertifikatsbereitstellung zu sichern. Dieser Vorgang kann bis zu drei Werktage dauern.</li></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html" target="_blank">Einrichten von SPF und DKIM</a> für die Zustellbarkeit von E-Mails.</li></td>
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
    <td><li>Initiieren <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html" target="_blank">Kommunikationsbeschränkungen</a>.</li>
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
    <td><li>Definieren der Verwendung <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html" target="_blank">channels</a>.</li></td>
  </tr>
  <tr>
    <td>Tags</td>
    <td><li>Definieren der Verwendung <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html" target="_blank">tags</a>.</li></td>
  </tr>
  <tr>
    <td>Kalender (falls zutreffend)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html" target="_blank">Sitzplätze im Marketing-Kalender ausgeben</a> für Personen, die Zugriff benötigen.</li>
    <li>Richten Sie die <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html" target="_blank">Kalender</a>.</li></td>
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
    <td><li>Implementieren einer Benennungskonvention für <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank">benutzerdefinierte Felder</a> (z. B. mit "MKTO").</li>
    <li>Seien Sie bezüglich der zu synchronisierenden Felder selektiv. Je mehr Felder Sie synchronisieren, desto langsamer wird der Synchronisierungszyklus sein.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank">Blockieren von Aktualisierungen in Feldern</a> Sie möchten ein einziges Mal schreiben (z. B. ursprüngliche Lead-Quelle, ursprüngliche Lead-Quelldetails, UTM-Felder für Erstkontakt usw.).</li></td>
  </tr>
  <tr>
    <td>Eigene Aktivitäten</td>
    <td><li>Definieren <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html">Benutzerdefinierte Aktivitäten</a> die spezifisch für Ihr Unternehmen sind.</li></td>
  </tr>
  <tr>
    <td>Benutzerdefinierte Objekte</td>
    <td><li>Überprüfen Sie, wie viele <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html">Benutzerdefinierte Objekte</a> benötigen.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html">Diese benutzerdefinierten Objekte mit Ihrem CRM-System synchronisieren</a>.</li></td>
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
    <td><li>Initiieren der CRM-Synchronisierung. Wählen Sie je nach dem von Ihrem Unternehmen verwendeten CRM Folgendes aus: <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html">Microsoft Dynamics</a>.</li>
    <li>Bestimmen Sie den Zugriffstyp, der für den Zugriff auf Ihr CRM-System erforderlich ist.</li>
    <li>Identifizieren Sie Ihren CRM-Administrator zur Fehlerbehebung.</li></td>
  </tr>
  <tr>
    <td>Webdienste</td>
    <td><li>Bestimmen Sie die Benutzer/Apps, die <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html">API-Aufrufe</a> in Ihrer Instanz.</li>
    <li>Überprüfen Sie alle Apps, die API-Aufrufe durchführen, und ermitteln Sie, ob eine Erhöhung oder Verringerung der API-Aufrufe erforderlich ist.</li></td>
  </tr>
  <tr>
    <td>LaunchPoint</td>
    <td><li>Einrichten <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html">LaunchPoint</a> Dienstleistungen für Ihr Unternehmen. Jeder LaunchPoint sollte mit einem eindeutigen API-Benutzer gepaart werden, um die Fehlerbehebung zu unterstützen.</li></td>
  </tr>
  <tr>
    <td>Interaktive Webinare (falls zutreffend)</td>
    <td>HINWEIS: Interaktive Webinare werden nur für Produktionsinstanzen bereitgestellt.
    <li>Zur Erstellung interaktiver Webinare, der integrierten Webinar-Funktion, <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management">Benutzer zum Abschnitt "Benutzer"hinzufügen</a> auf der Registerkarte "Interaktives Webinar".</li></td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (falls zutreffend)</td>
    <td><li>Benutzer zuweisen zu <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role">Rollen "Access Dynamic Chat"</a> unter Marketo Engage &gt; Admin &gt; Benutzer und Rollen.</li></td>
  </tr>
  <tr>
    <td>Sales Insight (falls zutreffend)</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account">Einrichten der Aktion "Sales Insight"</a> unter Sales Insight &gt; Aktionskonfiguration.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions">Stellen Sie den entsprechenden Benutzern Sitze aus.</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html">API konfigurieren</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html">Lead-Bewertungen anpassen</a>.</li></td>
  </tr>
  <tr>
    <td>Sales Connect (falls zutreffend)</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance">Laden Sie die entsprechenden Marketo Engage-Administratoren zur Sales Connect-Instanz ein.</a>.</li>
    <li>Führen Sie die <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins">Einrichtung eines zusätzlichen Sales Connect-Administrators</a> in Sales Connect und Salesforce.</li></td>
  </tr>
  <tr>
    <td>Webhooks (falls zutreffend)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html">Alle erforderlichen Webhooks erstellen</a> für Ihr Geschäft.</li>
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
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html">Aktivieren der Schatztruhe</a> , um mit Pilotenfunktionen zu experimentieren.</li>
    <li>Bestimmen Sie die Funktionen, die Sie aktivieren oder deaktivieren möchten.</li></td>
  </tr>
  <tr>
    <td>Kampagnenprüfung </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html">Aktivieren des Campaign-Inspektors</a> , um alle Ihre Smart-Kampagnen gleichzeitig anzuzeigen.</li></td>
  </tr>
</tbody>
</table>
