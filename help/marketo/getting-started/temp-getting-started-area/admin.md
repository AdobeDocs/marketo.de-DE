---
description: NEUER BEREICH - Marketo-Dokumente - Produktdokumentation
title: NEUER BEREICH
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: d65903d64d068a6f919df78258654414f3b76426
workflow-type: tm+mt
source-wordcount: '985'
ht-degree: 6%

---

# NEU: Admin-Checkliste {#new-area-admin-checklist}

Text einfügen.

## Rollen {#roles}

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
    <td>Rollen</td>
    <td><li>Überprüfen Sie die vordefinierten Rollen und bestätigen Sie, welche Berechtigungen/Zugriffsberechtigungen die einzelnen Rollen haben.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role">Neue Rolle erstellen</a> oder <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role">Rollen bearbeiten</a> basierend auf den Anforderungen Ihrer Organisation und wie oft sich Benutzer anmelden.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#assign-roles-to-a-user">Weisen Sie den entsprechenden Rollen Benutzer zu</a>.</li>
    <li>Nachdem Sie die Rollen für Benutzer zugewiesen haben, überprüfen Sie die Anzahl der Benutzer pro Rolle.</li>  <li>Implementieren Sie für jeden API-Benutzer eine eindeutige Rolle für die einfache Fehlerbehebung.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Dokumentation</td>
    <td>Definieren Sie Benutzer und Rollen für Ihre Organisation. <br>Definieren Sie Ihren Prozess zum Hinzufügen eines neuen Benutzers/Administrators.</td>
    <td></td>
  </tr>
  <tr>
    <td>Sandbox (falls zutreffend)</td>
    <td>Überprüfen Sie die oben genannten Kategorien für Ihre Sandbox, falls Sie eine haben.</td>
    <td></td>
  </tr>
</tbody>
</table>

## Arbeitsbereiche und Partitionen {#workspaces-partitions}

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
    <td>Arbeitsbereiche und Partitionen </td>
    <td><li>Bestimmen Sie die Anzahl der<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html"> Arbeitsbereiche</a> und/oder Partitionen, die Ihre Organisation benötigen und <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html">wie viele Benutzer Zugriff auf die einzelnen Arbeitsbereiche haben.</a></li>
    <li>Definieren Sie den Hauptzweck jedes Arbeitsbereichs und jeder Partition.</li>
    <li>Definieren Sie die Beziehung zwischen Ihren Arbeitsbereichen und Partitionen.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Dokumentation</td>
    <td><li>Dokumentieren Sie, wie Arbeitsbereiche definiert werden und wie sich dies auf Datenbankpartitionen bezieht (d. h. einen globalen Arbeitsbereich, der alle anzeigt, im Vergleich zu Unternehmenssektoren).</li>
    <li>Importieren Sie neue Datensätze in die entsprechende Partition.</li>
    <li>Definieren Sie den Wert in CRM, der Benutzer in die entsprechende Partition setzt.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Einstellungen für intelligente Kampagne {#smart-campaign-settings}

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
    <td>Einstellungen für intelligente Kampagne </td>
    <td><li>Hinzufügen einer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html">Größenbeschränkung für Smart-Campaign</a>verhindert, dass versehentlich die gesamte Datenbank per E-Mail versendet wird.</li>
    <li>Personenbeschränkungen für Smart-Kampagnen aktivieren</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## E-Mail-Einstellungen {#email-settings}

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
    <td>E-Mail-Standardwerte</td>
    <td><li>Wählen Sie unter Branding Domain Ihre Domäne aus und fügen Sie Ihren E-Mail-CNAME hinzu. Dies sollte im folgenden Format erfolgen: [EmailTrackingCNAME].[Unternehmensdomäne].com.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html">Einrichten von SPF und DKIM</a> für die Zustellbarkeit von E-Mails.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Kommunikationsbeschr {#communication-limits}

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
    <td>Kommunikationsbeschr</td>
    <td><li>Ort <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html">Kommunikationsgrenzen</a>.</li>
    <li>Bestimmen Sie, ob Ihr Unternehmen eine Richtlinie zu Kommunikationsbeschränkungen benötigt.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Tags {#tags}

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
    <td>Kanäle</td>
    <td><li>Definieren der Verwendung <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html">channels</a>.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Tags </td>
    <td><li>Definieren der Verwendung <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">tags</a>.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Kalender (falls zutreffend) </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html">Sitzplätze im Marketing-Kalender ausgeben</a> für Personen, die Zugriff benötigen.</li> 
    <li>Einrichten <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">Kalender</a>.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Datenbankverwaltung {#database-management}

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
    <td>Feldverwaltung</td>
    <td><li>Implementieren der Benennungskonvention für <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank">benutzerdefinierte Felder.</a> Beginnen Sie beispielsweise mit "MKTO".</li>
    <li>Seien Sie bezüglich der zu synchronisierenden Felder selektiv. Je mehr Felder Sie synchronisieren, desto langsamer wird der Synchronisierungszyklus sein.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank">Blockieren von Aktualisierungen in Feldern</a> Sie möchten nur einmal geschrieben werden (d. h. ursprüngliche Lead-Quelle, ursprüngliche Lead-Quelldetails, UTM-Felder für Erstkontakt usw.).</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Eigene Aktivitäten </td>
    <td><li>Definieren <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank">Benutzerdefinierte Aktivitäten</a> die spezifisch für Ihr Unternehmen sind.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Benutzerdefinierte Objekte </td>
    <td><li>Überprüfen Sie, wie viele <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank">Benutzerdefinierte Objekte</a> benötigen.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank">Diese benutzerdefinierten Objekte mit Ihrem CRM-System synchronisieren</a>.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Integrationen {#integrations}

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
    <td>CRM</td>
    <td><li>Initiieren der CRM-Synchronisierung. Wählen Sie je nach dem von Ihrem Unternehmen verwendeten CRM Folgendes aus: <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html" target="_blank">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html" target="_blank">Microsoft Dynamics</a>.</li>
    <li>Bestimmen Sie den Zugriffstyp, der für den Zugriff auf Ihr CRM-System erforderlich ist.</li>
    <li>Identifizieren Sie Ihren CRM-Administrator zur Fehlerbehebung.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Sales Insight (falls zutreffend)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html" target="_blank">Einrichten von Sales Insight.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank">Stellen Sie den entsprechenden Benutzern Sitze aus.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank">API konfigurieren</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank">Passen Sie die Lead-Bewertungen an.</a></li></td>
    <td></td>
  </tr>
  <tr>
    <td>Landing Pages </td>
    <td>HINWEIS: Sind Sie Launch Pack-Kunde? Sie können diesen Schritt überspringen. Ihr Berater wird Ihnen während Ihres Startaufrufs ein Dokument mit IT-Setup-Anweisungen zur Verfügung stellen. <br>Richten Sie Ihre Landingpage-Domäne mit einer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html" target="_blank">CNAME</a> und <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html" target="_blank">Domänen- und Seiteninformationen eingeben</a>. Dies sollte in folgendem Format erfolgen: [LandingPageCNAME].[Unternehmensdomäne].com <br>Wählen Sie einen CNAME für Ihre Landingpages aus. Beispiele: <br>* **go**.[Unternehmensdomäne].com <br>* **www2**.[Unternehmensdomäne].com <br>* **lp**.[Unternehmensdomäne].com <br>TIPP: Halten Sie es kurz! Kürzere URLs sind leichter zu merken. Wir empfehlen "go" als Domäne. <br>Fügen Sie Ihren Landingpage-Vorlagen Analytics-Trackingcode (z. B. Google Analytics oder Adobe Analytics) hinzu. </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Edit+Landing+Page+Settings">Einstellungen der Landingpage bearbeiten</a></td>
  </tr>
  <tr>
    <td rowspan="2">Munchkin </td>
    <td rowspan="2">HINWEIS: Wenn Sie Launch Pack-Kunde sind, überspringen Sie diesen Schritt. Ihr Berater stellt Ihnen im Dokument mit IT-Setup-Anweisungen Munchkin-Code zur Verfügung. <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html" target="_blank">Munchkin-Trackingcode hinzufügen</a> auf Ihrer Website. Munchkin-Code kann <a href="https://developers.marketo.com/javascript-api/lead-tracking/" target="_blank">hartcodiert</a> oder über Google Tag Manager bereitgestellt werden.</td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Add+Munchkin+Tracking+Code+to+Your+Website">Hinzufügen des Munchkin-Trackingcodes zu Ihrer Website</a> </td>
  </tr>
  <tr>
    <td><a href="https://developers.marketo.com/javascript-api/lead-tracking/">Lead-Tracking</a> </td>
  </tr>
  <tr>
    <td>Web-Services </td>
    <td>Aktivieren <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html" target="_blank">IP-Einschränkungen</a> gegebenenfalls. <br>Bestimmen Sie die Benutzer/Apps, die <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html" target="_blank">API-Aufrufe</a> in Ihrer Instanz. <br>Überprüfen Sie alle Apps, die API-Aufrufe durchführen, und ermitteln Sie, ob eine Erhöhung oder Kürzung für die API-Aufrufe erforderlich ist.</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html#product-docs">Erstellen einer Zulassungsliste für IP-basierten API-Zugriff </a> </td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (falls zutreffend) </td>
    <td>Verwendung <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html" target="_blank">Dynamic Chat</a>, dem nativen Kanal für die Konversationsinteraktion in Marketo Engage, fahren Sie mit der Einrichtung der Benutzerberechtigungen fort, indem Sie die folgenden Schritte ausführen: <a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a>. <br> <br>Bestätigen Sie, ob Ihr Adobe Org-Systemadministrator Ihnen eine Adobe Product Admin-Rolle zugewiesen hat. Kontakt <a href="https://helpx.adobe.com/contact.html" target="_blank">Adobe-Kundenunterstützung</a><a href="https://helpx.adobe.com/contact.html)." target="_blank">https://helpx.adobe.com/contact.html</a> , um herauszufinden, wer in Ihrem Unternehmen über Administratorrechte in der Konsole verfügt. <br>Accept <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html" target="_blank">Einladung "Dynamic Chat Product Admin"</a>. Die <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html" target="_blank">Willkommens-E-Mail</a> wird gesendet, wenn Dynamic Chat in Ihrer Marketo Engage-Instanz aktiviert ist und Sie als Systemadministrator benannt sind.  <br>Weisen Sie alle entsprechenden Benutzer dem Marketo Engage-Produktprofil in Adobe Admin Console zu. <br>Sie können Benutzerrollen nicht in Marketo Engage/Admin/Anwendern und Rollen zuweisen, bevor Sie sie zu einem Produktprofil hinzufügen.  <br>Wenn ein unerwünschter Benutzer mehreren Produktprofilen hinzugefügt wird, müssen Sie den Benutzer aus allen Produktprofilen löschen. Andernfalls haben sie weiterhin Zugriff auf Dynamic Chat. </td>
    <td> </td>
  </tr>
  <tr>
    <td>Startpunkt (falls zutreffend) </td>
    <td>Richten Sie alle erforderlichen ein <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">LaunchPoint</a> Dienstleistungen für Ihr Unternehmen.  <br>HINWEIS: Interaktive Webinare sind eine integrierte Webinar-Funktion mit nativer Integration in Adobe Connect. Es ist keine zusätzliche Integration erforderlich, Ihre Instanz muss jedoch <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">mit Adobe Connect as a LaunchPoint Service synchronisieren.</a>  </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Additional+Integrations">Zusätzliche Integrationen</a> </td>
  </tr>
  <tr>
    <td>Webhooks (falls zutreffend)</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html" target="_blank">Alle erforderlichen Webhooks erstellen</a> für Ihr Geschäft.  </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Create+a+Webhook">Webhook erstellen</a> </td>
  </tr>
</tbody>
</table>

## Schatzkiste {#treasure-chest}

<table>
<thead>
  <tr>
    <th>Bereich</th>
    <th>Aktionselement</th>
    <th>Priorität</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Schatzkiste</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html" target="_blank">Aktivieren der Schatztruhe</a> , um mit Pilotenfunktionen zu experimentieren.  <br>Bestimmen Sie die Funktionen, die Sie aktivieren oder deaktivieren möchten.</td>
    <td>Text</td>
  </tr>
  <tr>
    <td>Kampagnenprüfung </td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html" target="_blank">Aktivieren des Campaign-Inspektors</a> , um alle Ihre Smart-Kampagnen gleichzeitig anzuzeigen.</td>
    <td>Text</td>
  </tr>
</tbody>
</table>
