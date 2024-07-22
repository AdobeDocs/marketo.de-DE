---
description: Übernommene Checkliste für Instanzadministratoren - Marketo-Dokumente - Produktdokumentation
title: Checkliste für geerbte Instanzadministratoren
feature: Getting Started
exl-id: 088f3ce9-bf3d-4323-9cde-c39fec06c20e
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '1858'
ht-degree: 3%

---

# Vererbte Instanz: Checkliste für den Administratorbereich {#inherited-instance-admin-section-checklist}

Die folgenden Checklisten (nachfolgende Checklisten, die am Ende jedes Artikels mit verknüpft sind) wurden von Adobe Professional Services mit Eingaben von Marketo Champions zusammengestellt, damit Sie schnell auf den neuesten Stand kommen können. Sie können auch [die Checklisten herunterladen](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) und Ihren Fortschritt verfolgen.

>[!TIP]
>
>Wenn Sie ein neuer Marketo Engage-Benutzer sind und nicht mit vielen der Begriffe vertraut sind, sehen Sie sich bitte das [Marketo Engage-Glossar](/help/marketo/getting-started/things-to-know/marketo-engage-glossary.md){target="_blank"} an.

## Adobe Identity Management {#adobe-identity-management}

>[!NOTE]
>
>Dies gilt nur für Marketo Engage-Abonnements, die im [Adobe Identity Management System (IMS)](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"} integriert sind. Wenn Ihr Abonnement noch nicht mit Adobe IMS integriert wurde, fahren Sie mit dem [alten Benutzerrollen- und Berechtigungserlebnis](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"} unter Marketo Engage > Admin > Benutzer und Rollen fort.

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th> 
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Produkt-Admin für Marketo Engage und Abonnement</td> 
   <td><li>Wurde Ihr Marketo Engage-Abonnement bereits in <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md" target="_blank">Adobe IMS</a> migriert? 
<br/>     Wenn ja, wurde Ihnen von Ihrem Adobe Admin Console-Systemadministrator die Rolle "Adobe Admin Console-Produktadministrator"zugewiesen? Wenn Sie sich nicht sicher sind, wer in Ihrem Unternehmen über Administratorrechte in der Konsole verfügt, wenden Sie sich an die <a href="https://helpx.adobe.com/contact.html" target="_blank">Adobe-Kundenunterstützung</a>.</li>
<li>Haben Sie die Einladung "Marketo Engage Product Admin"angenommen? Die E-Mail wird gesendet, wenn die Rolle in der Adobe Admin Console zugewiesen wird.
<br/>     Wenn nicht, suchen Sie in Ihrem Posteingang nach der <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md#initial-setup" target="_blank">Begrüßungs-E-Mail</a> und nehmen Sie die Einladung zur Aktivierung Ihrer Adobe ID an.</li></td>
  </tr>
  <tr> 
   <td>Produktprofil</td> 
   <td><li>Sind alle entsprechenden Benutzer dem Marketo Engage-Produktprofil in Adobe Admin Console zugewiesen?
<br/>     Ist dies nicht der Fall, stellen Sie sicher, dass Sie in der Adobe Admin Console <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md" target="_blank">Benutzer hinzufügen und/oder aus Marketo Engage-Produktprofilen entfernen</a>. Sie können Benutzerrollen nicht unter Marketo Engage &gt; Admin &gt; Benutzer und Rollen zuweisen, wenn sie einem Produktprofil hinzugefügt werden.</li>
<p><img src="assets/note-icon.png" alt="Notizsymbol"> HINWEIS: Wenn ein unerwünschter Benutzer mehreren Produktprofilen hinzugefügt wird, müssen Sie den Benutzer aus allen Produktprofilen entfernen. Andernfalls haben sie immer noch Zugriff auf Marketo Engage.</td>
  </tr>
  <tr> 
   <td>User Management-API</td> 
   <td><li>Verwendet Ihr Abonnement beliebige Marketo User Management-APIs?
<br/>     In diesem Fall müssen Sie <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html" target="_blank">Adobe IMS-APIs</a> verwenden, um Benutzer einzuladen, zu aktualisieren und zu löschen, die in Zukunft auf die Site folgen.</li>
<p><img src="assets/note-icon.png" alt="Notizsymbol"> HINWEIS: "Rollenverwaltung"verbleibt im Marketo Engage, und Marketo User Management-APIs können weiterhin für die Rollenverwaltung verwendet werden.</td>
  </tr>
 </tbody> 
</table>

## Benutzer und Rollen {#users-and-roles}

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Benutzer</td> 
   <td><img src="assets/note-icon.png" alt="Notizsymbol"> HINWEIS: Wenn Ihr Abonnement bereits über Adobe IMS erfolgt, fahren Sie mit der folgenden Benutzerverwaltungsprüfung in Adobe Admin Console fort. Andernfalls navigieren Sie zu Admin &gt; Benutzer und Rollen &gt; Benutzer im Marketo Engage.
   <p>
   <li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">Wie viele Benutzer gibt es</a>?</li>
<li>Gibt es Benutzer, die <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md#remove-a-user" target="_blank">entfernt</a> werden sollten?</li>
<li>Verfügt Ihr Unternehmen über Richtlinien zum Löschen von Benutzern?</li> 
<li>Wie viele Benutzer haben <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">Administratorberechtigungen</a>?</li>
<li>Sollte einer dieser Benutzer in <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">andere Rollen geändert werden?</a></li> 
<li>Wer sind die <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md" target="_blank">API-Benutzer</a> in dieser Instanz?</li></td>
  </tr>
  <tr> 
   <td>Rollen</td> 
   <td><img src="assets/note-icon.png" alt="Notizsymbol"> HINWEIS: Unabhängig davon, ob Sie Marketo mit Adobe Identity verwenden oder nicht, fahren Sie mit der Überprüfung der Rollenberechtigungen unter Marketo Engage unter Admin &gt; Benutzer und Rollen &gt; Rollen fort.
   <p><li>Wie viele Rollen gibt es?</li>  
<li>Welche <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">Berechtigungen/Zugriffsberechtigungen</a> hat jede Rolle? Sollte eine Anpassung vorgenommen werden?</li>
<li>Wie viele Benutzer gibt es pro Rolle?</li>
<li>Wie oft melden sich Benutzer <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">bei</a> an?</li>
<li>Verfügt jeder API-Benutzer über seine <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">eigene Benutzerrolle</a>? Falls nicht, sollten Sie dies implementieren, um die Fehlerbehebung zu vereinfachen.</li> 
<li>Stimmen Ihre Benutzerrollen und Berechtigungen mit Ihren Datenschutzrichtlinien für Unternehmen überein, um die Einhaltung von Vorschriften zu gewährleisten (z. B. <a href="https://gdpr-info.eu/" target="_blank">DSGVO</a>)? Erlauben die Unternehmensdaten <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">Datenschutzrichtlinien</a> Benutzern, Marketo Engage-Benutzerdaten herunterzuladen und freizugeben? Ist das Genehmigungsverfahren erforderlich?</li></td>
  </tr>
  <tr> 
   <td>Support-Benutzer</td> 
   <td><li>Haben Sie die entsprechenden <a href="/help/marketo/getting-started/initial-setup/setup-steps.md#set-up-your-authorized-support-contacts" target="_blank">berechtigten Kontakte</a> im Support-Portal eingerichtet?</li></td>
  </tr>
  <tr> 
   <td>Interne Dokumentation</td> 
   <td><li>Sind Benutzer und Rollen in Ihrer Organisation klar definiert?</li>
<li>Wie wird ein neuer Benutzer/Administrator hinzugefügt?</li></td>
  </tr>
  <tr> 
   <td>Sandbox (falls zutreffend)</td> 
   <td><li>Verfügen Sie über eine <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">Sandbox-Instanz</a>?
   <br/>     Wenn ja, überprüfen Sie die oben genannten Kategorien für Ihre Sandbox.</li>
<li>Ist <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">Programmimport</a> mit Ihrer Sandbox verknüpft?</li></td>
  </tr>
 </tbody> 
</table>

## Audit-Trail {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Audit-Trail</td> 
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">Wer arbeitet</a> in der Instanz?</li></td>
  </tr>
 </tbody> 
</table>

## Arbeitsb. &amp; Partitionen {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Arbeitsb. &amp; Partitionen</td> 
   <td><li>Wie viele <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md" target="_blank">Arbeitsbereiche und/oder Partitionen</a> haben Sie?</li>
<li>Was ist der primäre Zweck jeder Workspace und Partition?</li>
<li>Müssen Ihre <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-a-workspace.md" target="_blank">Arbeitsbereiche</a> oder <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-an-existing-person-partition.md" target="_blank">Partitionen</a> geprüft/geändert werden?</li>
<li>Welche Beziehung besteht zwischen Ihren Arbeitsbereichen und Partitionen?</li>
<li>Wie viele Benutzer <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.md" target="_blank">haben Zugriff auf </a> auf die einzelnen Workspace?</li></td>
  </tr>
  <tr> 
   <td>Interne Dokumentation</td> 
   <td><li>Wie werden Arbeitsbereiche und Partitionen definiert?</li>
<li>Wie verläuft Ihr Prozess, um Ihrer Instanz Arbeitsbereiche hinzuzufügen oder Benutzer zu einer Workspace hinzuzufügen?</li></td>
  </tr>
 </tbody> 
</table>

## Intelligente Kampagnen {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Intelligente Kampagnen</td> 
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank">Haben Sie eine Beschränkung</a> für die Größe von Smart-Kampagnen? 
   <br/>     Ist dies nicht der Fall, können Sie eine hinzufügen. Es wird empfohlen, die Beschränkung der intelligenten Kampagne auf 25 % Ihrer Datenbank zu begrenzen, um eine Überkommunikation oder Verarbeitung Ihrer gesamten Datenbank in Workflows zu vermeiden. Dies schützt nicht nur Ihre Marke, sondern schützt auch die Leistung Ihrer Instanz.</li></td>
  </tr>
 </tbody> 
</table>

## Kommunikationsbeschränkungen {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Kommunikationsbeschränkungen</td> 
   <td><li>Gibt es <a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">Kommunikationsbeschränkungen</a>? Verfügt Ihr Unternehmen über Richtlinien, bei denen Kommunikationsbeschränkungen erforderlich sein könnten?</li>
<p><img src="assets/note-icon.png" alt="Notizsymbol"> HINWEIS: Es wird empfohlen, Ihre Kommunikation auf 1 pro Tag und 3 pro 7 Tage zu begrenzen, wobei die E-Mails <b>non</b>-<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">operations</a> blockiert werden.</td>
  </tr>
 </tbody> 
</table>

## Tags {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Tags</td> 
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.md" target="_blank">Wie viele Tags gibt es?</a> Wie viele Tags werden verwendet? Müssen noch weitere hinzugefügt werden?</li>
<li>Sind Tags in Ihren Programmen erforderlich?</li></td>
  </tr>
  <tr> 
   <td>Kanäle</td> 
   <td><li><a href="/help/marketo/product-docs/administration/tags/create-a-program-channel.md" target="_blank">Wie viele Kanäle</a> gibt es? Wie viele werden verwendet?</li>
<li>Sind alle <a href="/help/marketo/product-docs/administration/tags/hide-unhide-a-program-channel.md" target="_blank">Kanalprogrammstatus angemessen</a>? Zeigen sie Fortschritte im Rahmen des Programms?</li>
<li>Sind Ihre Kanäle mit bestimmten Programmtypen verbunden?</li>
<li>Welche Status werden für jeden Kanal als erfolgreich betrachtet? Stimmen diese mit Ihren Marketing-Zielen überein?</li>
<li>Wird der operationelle Kanal ordnungsgemäß verwendet?</li>
<li>Ist für "Erweiterter Report Builder"(Umsatz-Cycle Explorer/RCE) das Verhalten Ihrer Kanalanalyse so eingestellt, dass es mit den Programmpraktiken übereinstimmt, die Zeitraumkosten enthalten?</li></td>
  </tr>
  <tr> 
   <td>Marketing-Kalender (falls zutreffend)</td> 
   <td><li>Wie viele <a href="/help/marketo/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.md" target="_blank">Kalendereintragstypen</a> gibt es? Sind sie alle noch relevant?</li></td>
  </tr>
 </tbody> 
</table>

## Datenbankverwaltung {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Feldverwaltung</td> 
   <td><li>Wie viele Felder gibt es? 
   <br/>     Klicken Sie auf <a href="/help/marketo/product-docs/administration/field-management/export-a-list-of-all-marketo-api-field-names.md" target="_blank">Feldnamen exportieren</a> , um eine Liste Ihrer Felder, benutzerdefinierten Felder und deren API-Namen anzuzeigen.</li>
<li>Wie viele <a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">benutzerdefinierte Felder</a> gibt es?</li>
<li>Wie viele Felder werden verwendet? 
<br/>     Wählen Sie im Dropdown-Menü Feldaktionen die Option <a href="/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md" target="_blank">Verwendet von exportieren</a> aus, um zugehörige Assets eines Felds zu überprüfen.</li>
<li>Wie viele Felder werden zwischen Marketo Engage und Ihrem CRM synchronisiert?</li>
<li>Werden CRM-Felder mit den entsprechenden Objekten synchronisiert?</li>
<li>Gibt es einen <a href="/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md" target="_blank">benutzerdefinierten Ansichtssatz</a> für Personendetails? Sollte es denn geben?</li>
<li>Verfügen Sie über eine auf der Quelle basierende Namenskonvention für Ihre Felder? 
<br/>     Wenn nicht, sollten Sie die Implementierung in Erwägung ziehen.</li>
<li>Gibt es Felder <a href="/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md" target="_blank">blockiert</a>? 
<br/>     Wenn ja, sollten Sie wissen, warum sie das sind.</li></td>
  </tr>
  <tr> 
   <td>Eigene Aktivitäten</td> 
   <td><li>Gibt es <a href="/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md" target="_blank">benutzerdefinierte Aktivitäten</a>?
<br/>     Wenn ja, durchklicken Sie sie, um zu verstehen, welche Aktivitäten nicht mit einem Marketo-Formular, einer E-Mail oder einer Landingpage verbunden sind.</li></td>
  </tr>
  <tr> 
   <td>Benutzerdefinierte Objekte</td> 
   <td><li>Wie viele <a href="/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md" target="_blank">benutzerdefinierte Objekte</a> gibt es? Wie werden sie mit Ihrem CRM synchronisiert?</li>
<li>Wie werden diese benutzerdefinierten Objekte von Ihren Programmen und Listenabfragen verwendet?</li></td>
  </tr>
 </tbody> 
</table>

## E-Mail {#email}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>E-Mail-Standardeinstellungen</td> 
   <td><li>Sind all Ihre Standardeinstellungen unter Admin &gt; E-Mail aktuell (z. B. <a href="/help/marketo/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.md" target="_blank">"from" email/label</a>, <a href="/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md" target="_blank">branding domain</a>, <a href="/help/marketo/product-docs/administration/email-setup/edit-the-unsubscribe-message.md" target="_blank">unsubscribe message</a> usw.)?</li></td>
  </tr>
 </tbody> 
</table>

## Integrationen {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>Mit welchem CRM synchronisieren Sie? Salesforce? MS Dynamics? Veeva?</li>
<li>Verwenden Sie eine <a href="https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758" target="_blank">benutzerdefinierte Synchronisierung</a>?</li>
<li>[Nur Salesforce] Ist für Ihre Instanz benutzerdefinierte Synchronisierungsfilter implementiert? 
<p><img src="assets/note-icon.png" alt="Notizsymbol"> HINWEIS: Wenden Sie sich an den Marketo-Support, um benutzerdefinierte Synchronisierungsfilter zu ermitteln oder die Implementierung einer benutzerspezifischen Synchronisierungsregel anzufordern.</li></td>
  </tr>
  <tr> 
   <td>Landing Page</td> 
   <td><li>Wie lautet die <a href="/help/marketo/product-docs/administration/settings/edit-landing-page-settings.md" target="_blank">Domäne </a>?</li>
   <li>Wie ist die Homepage eingestellt?</li>
<li>Was ist der <a href="/help/marketo/product-docs/administration/settings/set-a-fallback-page.md" target="_blank">Fallback als </a> festgelegt?</li>
<li>Ist das Vorausfüllen des Formulars aktiviert?</li>
<li>Sind <a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/enable-personalized-urls-for-your-account.md" target="_blank">personalisierte URLs</a> aktiviert?</li>
<li>Gibt es Regeln für <a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/redirect-a-marketo-landing-page-to-another-page.md" target="_blank">Umleitungen</a>?</li>
<li>Haben Sie Domain-Aliase? Verfolgen Sie, wie Sie Ihre Domain-Aliase verwenden?</li>
<li>Ist <a href="https://nation.marketo.com/t5/knowledgebase/setting-up-secured-domains-for-marketo-landing-pages-first-time/ta-p/250370" target="_blank">gesicherte Domänen für Einstiegsseiten</a> aktiviert? 
<br/>     Bestätigen Sie, ob Ihre Landingpage-Assets eine "http"-URL enthalten.</li></td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>Ist Ihr <a href="/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md" target="_blank">Munchkin-Trackingcode</a> auf Ihrer Website (keine Marketo Engage-Landingpage)?</li>
<li>Ist eine Browseranforderung vom Typ <a href="/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md" target="_blank">Nicht verfolgen</a> aktiviert?</li>
<li>Ist Ihre <a href="https://experienceleague.adobe.com/docs/marketo-developer/marketo/javascriptapi/lead-tracking.html" target="_blank">Munchkin-API</a> konfiguriert? 
<p><img src="assets/tip-icon.png" alt="Tippsymbol">TIPP: Wenn Ihnen die Dokumentation fehlt, in der sich der Munchkin-Code auf Ihrer Website befindet, können Sie alle URLs anzeigen, indem Sie einen <a href="/help/marketo/product-docs/reporting/basic-reporting/report-types/web-page-activity-report.md" target="_blank">Web-Seiten-Aktivitätsbericht</a> erstellen.</li></td>
  </tr>
  <tr> 
   <td>Webdienste</td> 
   <td><li>Sind <a href="/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md" target="_blank">IP-Einschränkungen</a> aktiviert? Sollen sie das sein?</li>
<li>Welche Benutzer/Apps führen API-Aufrufe in Ihrer Instanz durch?</li>
<li>Haben Sie Ihr API-Limit erreicht oder stehen Sie kurz davor?
<br/>     Falls ja, sollten Sie sie erhöhen oder Ihre Instanz überprüfen, um diese API-Aufrufe zu reduzieren.</li></td>
  </tr>
  <tr> 
   <td>Adobe Dynamic Chat (falls zutreffend)</td> 
<td>Für die folgenden Schritte ist Zugriff auf den <a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a> erforderlich. Wenn Sie noch keine Adobe ID eingerichtet haben, erfahren Sie <a href="https://helpx.adobe.com/manage-account/using/create-update-adobe-id.html" target="_blank">, wie Sie dies hier vornehmen können</a>.
<br/>
<li>Haben Sie die Einladung <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.md" target="_blank">Dynamic Chat Product Admin</a> angenommen? Die E-Mail wird gesendet, wenn Dynamic Chat in Ihrer Marketo Engage-Instanz aktiviert ist und Sie als Systemadministrator benannt sind.
<br/>     Wenn nicht, suchen Sie nach der Begrüßungs-E-Mail in Ihrem Posteingang und nehmen Sie die Einladung zur Einrichtung Ihrer Adobe ID an.</li>   
<li>Haben Sie die <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user" target="_blank">gewünschten Benutzer</a> zum Dynamic Chat-Produktprofil in Adobe Admin Console hinzugefügt?
<li>Stellen Sie sicher, dass Ihren berechtigten Benutzern das Dynamic Chat-Produktprofil zu ihrer Adobe-Identität hinzugefügt wird. Sie können unter Marketo Engage &gt; Admin &gt; Dynamic Chat keine Rollen zuweisen, wenn diese einem Produktprofil hinzugefügt werden.</li>
<li>Entsprechen die Standardprofilberechtigungen auf der Registerkarte "Produktprofile"den Anforderungen Ihres Unternehmens?<br/> 
Wenn nicht, bearbeiten Sie die Berechtigungen für das spezifische Profil. </li>
<li>Wenn Sie mehr als ein Abonnement haben, werden Ihre Benutzer zu den richtigen Abonnements hinzugefügt?</li>
<br>
Sobald Sie die Prüfung der Benutzer- und Benutzereinstellungen abgeschlossen haben, melden Sie sich bei Dynamic Chat an, um Ihre Prüfung fortzusetzen.  
<li>Haben Sie <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md" target="_blank">Ihre Marketo Engage-Instanz</a> mit Dynamic Chat verbunden?</li>
<li>Gelten die fünf Standardprofile mit vordefinierten Berechtigungen für Ihre Organisation?<br/> 
     Ist dies nicht der Fall, können Sie diese <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#edit-existing-permissions" target="_blank">in Dynamic Chat</a> bearbeiten. Sie können auch <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#create-a-profile" target="_blank">ein benutzerdefiniertes Profil </a> mit benutzerdefinierten Berechtigungen erstellen.</li>
<li>Haben Sie die Option "Zugriff auf Dynamic Chat" auf die entsprechende Marketo Engage-Rolle unter Admin &gt; Benutzer und Rollen &gt; Rollen aktiviert, um Ihren Benutzern Zugriff auf Dynamic Chat zu ermöglichen?
<br/><img src="assets/note-icon.png" alt="Notizsymbol"> HINWEIS: Die Rollen "Admin"und "Marketing-Benutzer"sollten Zugriff auf Dynamic Chat haben.</li>
</td>
  </tr>
  <td>Marketo Sales Insight (falls zutreffend)</td> 
   <td><li>Wurde das <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">MSI-Paket installiert</a>?</li>
<li>Haben Sie <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">auf die neueste Version von Sales Insight</a> aktualisiert?</li>
<li>Haben Sie die Konfiguration von Sales Insight abgeschlossen? <br/>     Enterprise/Unlimited users <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">klicken Sie hier</a>, Professional Users <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">klicken Sie hier</a>.</li>
<li>Haben Sie <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">Ihren Benutzern je nach Anzahl der von Ihnen gekauften Plätze Zugriff gewährt</a>?</li>
<li>Sind <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md" target="_blank">Sterne und Flammen</a> angepasst?</li></td>
  </tr>
  <tr> 
   <td>Startpunkt (falls zutreffend)</td> 
   <td><li>Welche Dienste haben Sie konfiguriert (z. B. <a href="/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md" target="_blank">BrightTALK</a>, <a href="/help/marketo/product-docs/administration/additional-integrations/connect-brighttalk-to-marketo.md" target="_blank">Zoom</a> usw.)? Sind sie kurz vor ihrem Ablauf?</li>
<li><a href="https://nation.marketo.com/t5/knowledgebase/viewing-your-number-of-api-calls-to-marketo/ta-p/254256" target="_blank">Wie viele API-Aufrufe</a> verwenden Ihre Integrationen?</li>
<li>Verfügen Sie über die richtigen Integrationen für Ihre Anwendungsfälle?</li></td>
  </tr>
  <tr> 
   <td>Webhooks (falls zutreffend)</td> 
   <td><li><a href="/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md" target="_blank">Welche Verbindungen</a> haben Sie eingerichtet?</li>
<li>Wird es nicht mehr verwendet?</li></td>
  </tr>
  <tr> 
   <td>Mobile Apps (falls zutreffend)</td> 
   <td><li>Welche <a href="/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md" target="_blank">mobilen Apps</a> haben Sie?</li>
<li>Wurden <a href="/help/marketo/product-docs/mobile-marketing/push-notifications/adding-a-new-test-device.md" target="_blank">Testgeräte</a> hinzugefügt?</li></td>
  </tr>
 </tbody> 
</table>

## Schatzkiste {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Schatzkiste</td> 
   <td><li>Was ist in der <a href="/help/marketo/product-docs/administration/settings/enable-or-disable-treasure-chest-features.md" target="_blank">Schatztruhe</a> aktiviert?</li>
<li>Gibt es Funktionen, die aktiviert oder deaktiviert werden sollten?</li></td>
  </tr>
  <tr> 
   <td>Kampagnenprüfung</td> 
   <td><li>Ist <a href="/help/marketo/product-docs/administration/settings/campaign-inspector.md" target="_blank">Kampagneninspektor</a> aktiviert?
<br/>Ist dies nicht der Fall, sollten Sie es aktivieren, um einfach festzustellen, welche Kampagnen aktiv sind: aktive Kampagnen, Synchronisierung mit Ihrem CRM-System und/oder Löschen von Datensätzen.</li></td>
  </tr>
 </tbody> 
</table>

## Warnhinweise und Aktualisierungen {#alerts-and-updates}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Fokus überprüfen</th>
  </tr> 
  <tr> 
   <td>Marketo Engage-Statusaktualisierungen</td> 
   <td><li>Hat Ihre Instanz <a href="https://nation.marketo.com/t5/knowledgebase/how-to-subscribe-to-status-page-notifications/ta-p/296749" target="_blank">Marketo Engage Status-Updates</a> abonniert?</li></td>
  </tr>
  <tr> 
   <td>Warnhinweise</td> 
   <td><li>Gibt es <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md" target="_blank">aktive Warnhinweise</a>, die von Marketo Engage an interne Teams gesendet werden?</li>
<li>Wenn ja, funktionieren diese Ausschreibungen ordnungsgemäß?</li></td>
  </tr>
  <tr> 
   <td>Benachrichtigungen</td> 
   <td><li>Sind Sie für den entsprechenden Administrator <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md" target="_blank">notifications</a> angemeldet?</li></td>
  </tr>
 </tbody> 
</table>
