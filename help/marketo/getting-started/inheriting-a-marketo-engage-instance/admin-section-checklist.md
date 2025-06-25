---
description: Checkliste für geerbte Instanzen - Marketo-Dokumente - Produktdokumentation
title: Checkliste für geerbte Instanzadministratoren
feature: Getting Started
exl-id: 088f3ce9-bf3d-4323-9cde-c39fec06c20e
source-git-commit: b95458ffab422901ef5e674756ae5e413ec542fd
workflow-type: tm+mt
source-wordcount: '1858'
ht-degree: 3%

---

# Vererbte Instanz: Checkliste für den Administratorbereich {#inherited-instance-admin-section-checklist}

Die folgenden Checklisten (nachfolgende Checklisten, die am Ende jedes Artikels verlinkt sind) wurden von Adobe Professional Services mit Beiträgen von Marketo Champions zusammengestellt, damit Sie sich schnell zurechtfinden. Sie können auch [Checklisten herunterladen](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) und Ihren Fortschritt verfolgen.

>[!TIP]
>
>Wenn Sie ein(e) neue(r) Marketo Engage-Benutzer(in) sind und mit vielen der Begriffe nicht vertraut sind, lesen Sie bitte das [Marketo Engage-Glossar](/help/marketo/getting-started/things-to-know/marketo-engage-glossary.md){target="_blank"}.

## Adobe Identity Management {#adobe-identity-management}

>[!NOTE]
>
>Dies gilt nur für Marketo Engage-Abonnements, die in das [Adobe Identity Management System (IMS) integriert ](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}. Wenn Adobe IMS noch nicht in Ihr Abonnement integriert wurde, fahren Sie mit dem Erlebnis [Legacy-Benutzerrollen und -Berechtigungen](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"} in Marketo Engage > Admin > Benutzer und Rollen fort.

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th> 
   <th>Review Focus</th>
  </tr> 
  <tr> 
   <td>Abonnement und Marketo Engage-Produktadministrator</td> 
   <td><li>Wurde Ihr Marketo Engage-Abonnement bereits zu <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md" target="_blank">Adobe IMS</a> migriert? 
<br/>     Wenn ja, wurde Ihnen von Ihrem Adobe Admin Console-Systemadministrator die Rolle "Adobe Admin Console-Produktadministrator“ zugewiesen? Wenn Sie sich nicht sicher sind, wer in Ihrem Unternehmen über Administratorrechte in der Konsole verfügt, wenden Sie sich an die <a href="https://helpx.adobe.com/contact.html" target="_blank">Adobe-Kundenunterstützung</a>.</li>
<li>Haben Sie die Einladung zum "Marketo Engage Product Admin“ angenommen? Die E-Mail wird gesendet, wenn die Rolle in der Adobe Admin Console zugewiesen wird.
<br/>     Suchen Sie andernfalls in Ihrem Posteingang nach der <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md#initial-setup" target="_blank">Begrüßungs-E</a>Mail) und akzeptieren Sie die Einladung zur Aktivierung Ihrer Adobe ID.</li></td>
  </tr>
  <tr> 
   <td>Produktprofil</td> 
   <td><li>Sind alle entsprechenden Benutzenden dem Produktprofil von Marketo Engage in Adobe Admin Console zugewiesen?
<br/>     Ist dies nicht der Fall, stellen Sie sicher<a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md" target="_blank"> dass Sie Benutzende </a> Marketo Engage-Produktprofilen in der Adobe Admin Console hinzufügen und/oder entfernen. Benutzerrollen können unter "Marketo Engage" &gt; „Admin“ &gt; „Benutzer und Rollen“ nicht zugewiesen werden, wenn sie einem Produktprofil hinzugefügt werden.</li>
<p><img src="assets/note-icon.png" alt="Notizensymbol"> HINWEIS: Wenn ein unerwünschter Benutzer mehreren Produktprofilen hinzugefügt wird, müssen Sie ihn aus allen Produktprofilen entfernen. Andernfalls haben sie weiterhin Zugriff auf Marketo Engage.</td>
  </tr>
  <tr> 
   <td>User Management-API</td> 
   <td><li>Verwendet Ihr Abonnement Marketo User Management-APIs?
<br/>     In diesem Fall müssen Sie die <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html" target="_blank">Adobe IMS-APIs</a> verwenden, um künftig Benutzer einzuladen, zu aktualisieren und zu löschen.</li>
<p><img src="assets/note-icon.png" alt="Notizensymbol"> HINWEIS: „Rollenverwaltung“ verbleibt in Marketo Engage und Marketo User Management-APIs können weiterhin für die Rollenverwaltung verwendet werden.</td>
  </tr>
 </tbody> 
</table>

## Benutzer und Rollen {#users-and-roles}

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr> 
  <tr> 
   <td>Benutzer</td> 
   <td><img src="assets/note-icon.png" alt="Notizensymbol"> HINWEIS: Wenn Ihr Abonnement bereits über Adobe IMS erfolgt, fahren Sie mit der folgenden Benutzerverwaltungsprüfung in Adobe Admin Console fort. Gehen Sie andernfalls zu Admin &gt; Benutzer &amp; Rollen &gt; Benutzer in Marketo Engage.
   <p>
   <li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">Wie viele Benutzer </a> es?</li>
<li>Gibt es Benutzer, die entfernt <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md#remove-a-user" target="_blank"> sollen</a>?</li>
<li>Hat Ihr Unternehmen Richtlinien zum Löschen von Benutzern?</li> 
<li>Wie viele Benutzer haben <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">Administratorrechte</a>?</li>
<li>Sollte einer dieser Benutzer in "<a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank"> Rollen“ geändert werden</a></li> 
<li>Wer sind die <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md" target="_blank">API-Benutzer</a> in dieser Instanz?</li></td>
  </tr>
  <tr> 
   <td>Rollen</td> 
   <td><img src="assets/note-icon.png" alt="Notizensymbol"> HINWEIS: Unabhängig davon, ob Sie Marketo mit Adobe Identity verwenden oder nicht, überprüfen Sie in Marketo Engage unter „Admin“ &gt; „Benutzer und Rollen“ &gt; „Rollen“ die Rollenberechtigungen.
   <p><li>Wie viele Rollen gibt es?</li>  
<li>Welche <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">Berechtigungen/Zugriff</a> verfügt jede Rolle? Sollte einer angepasst werden?</li>
<li>Wie viele Benutzer gibt es pro Rolle?</li>
<li>Wie oft <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank"> sich Benutzer </a>?</li>
<li>Hat jeder API-Benutzer seine <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank"> Benutzerrolle</a>? Wenn nicht, sollten Sie dies implementieren, um die Fehlerbehebung zu vereinfachen.</li> 
<li>Stimmen Ihre Benutzerrollen und -berechtigungen mit Ihren Datenschutzrichtlinien für Unternehmen hinsichtlich der Einhaltung von Vorschriften (z. B. <a href="https://gdpr-info.eu/" target="_blank">DSGVO</a>) überein? Erlauben die Unternehmensdaten <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">Datenschutzrichtlinien</a> Benutzern das Herunterladen und Freigeben von Marketo Engage-Benutzerdaten? Ist die Geschäftsgenehmigung nötig?</li></td>
  </tr>
  <tr> 
   <td>Support-Benutzer</td> 
   <td><li>Haben Sie im Support<a href="/help/marketo/getting-started/initial-setup/setup-steps.md#set-up-your-authorized-support-contacts" target="_blank">Portal die entsprechenden autorisierten </a> eingerichtet?</li></td>
  </tr>
  <tr> 
   <td>Interne Dokumentation</td> 
   <td><li>Sind Benutzende und Rollen in Ihrer Organisation klar definiert?</li>
<li>Wie sieht der Prozess für das Hinzufügen eines neuen Benutzers/Administrators aus?</li></td>
  </tr>
  <tr> 
   <td>Sandbox (falls zutreffend)</td> 
   <td><li>Haben Sie eine <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">Sandbox-</a>?
   <br/>     Überprüfen Sie in diesem Fall die oben genannten Kategorien für Ihre Sandbox.</li>
<li>Ist <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">Programmimport</a> mit Ihrer Sandbox verknüpft?</li></td>
  </tr>
 </tbody> 
</table>

## Audit-Protokoll {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr> 
  <tr> 
   <td>Audit-Protokoll</td> 
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">Wer arbeitet in </a> Instanz?</li></td>
  </tr>
 </tbody> 
</table>

## Arbeitsb. &amp; Partitionen {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr> 
  <tr> 
   <td>Arbeitsb. &amp; Partitionen</td> 
   <td><li>Wie viele <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md" target="_blank">Arbeitsbereiche und/oder Partitionen</a> verfügen Sie?</li>
<li>Was ist der Hauptzweck jeder Workspace und Partition?</li>
<li>Müssen entweder <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-a-workspace.md" target="_blank">Arbeitsbereiche</a> oder <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-an-existing-person-partition.md" target="_blank">Partitionen</a> geprüft/geändert werden?</li>
<li>In welcher Beziehung stehen Arbeitsbereiche und Partitionen zueinander?</li>
<li>Wie viele Benutzer <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.md" target="_blank">Zugriff</a> auf jede Workspace?</li></td>
  </tr>
  <tr> 
   <td>Interne Dokumentation</td> 
   <td><li>Wie werden Arbeitsbereiche und Partitionen definiert?</li>
<li>Wie sieht Ihr Prozess aus, um Workspaces zu Ihrer Instanz hinzuzufügen oder Benutzer zu einer Workspace hinzuzufügen?</li></td>
  </tr>
 </tbody> 
</table>

## Intelligente Kampagnen {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr> 
  <tr> 
   <td>Intelligente Kampagnen</td> 
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank">Gibt es eine Einschränkung hinsichtlich </a> Größe von Smart Campaign? 
   <br/>     Falls nicht, sollten Sie eine hinzufügen. Es wird empfohlen, die Smart Campaign-Beschränkungen auf 25 % der Datenbank zu begrenzen, um Überkommunikation zu vermeiden oder die gesamte Datenbank in Workflows zu verarbeiten. Dies schützt nicht nur Ihre Marke, sondern auch die Leistung Ihrer Instanz.</li></td>
  </tr>
 </tbody> 
</table>

## Kommunikationsbeschränkungen {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr> 
  <tr> 
   <td>Kommunikationsbeschränkungen</td> 
   <td><li>Gibt es <a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">Kommunikationsbeschränkungen</a>? Gibt es in Ihrem Unternehmen Richtlinien, bei denen Kommunikationsbeschränkungen erforderlich sein könnten?</li>
<p><img src="assets/note-icon.png" alt="Notizensymbol"> HINWEIS: Es wird empfohlen, die Kommunikation auf 1 pro Tag und 3 pro 7 Tage zu beschränken, wobei <b>nicht</b>-<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">operative</a> E-Mails blockiert werden.</td>
  </tr>
 </tbody> 
</table>

## Tags {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr> 
  <tr> 
   <td>Tags</td> 
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.md" target="_blank">Wie viele Tags </a> es? Wie viele Tags werden verwendet? Müssen irgendwelche hinzugefügt werden?</li>
<li>Sind Tags in Ihren Programmen erforderlich?</li></td>
  </tr>
  <tr> 
   <td>Kanäle</td> 
   <td><li><a href="/help/marketo/product-docs/administration/tags/create-a-program-channel.md" target="_blank">Wie viele Kanäle</a> gibt es? Wie viele sind in Gebrauch?</li>
<li>Sind alle <a href="/help/marketo/product-docs/administration/tags/hide-unhide-a-program-channel.md" target="_blank">Kanalprogrammstatus angemessen</a>? Zeigen sie Fortschritte innerhalb des Programms?</li>
<li>Sind Ihre Kanäle mit bestimmten Programmtypen verbunden?</li>
<li>Welche Status werden für jeden Kanal als erfolgreich erachtet? Stimmen diese mit Ihren Marketing-Zielen überein?</li>
<li>Wird der operative Kanal ordnungsgemäß verwendet?</li>
<li>Ist Ihr Kanalanalyseverhalten für Advanced Report Builder (Revenue Cycle Explorer/RCE) so eingestellt, dass es mit Ihren Programmpraktiken übereinstimmt und die Periodenkosten berücksichtigt?</li></td>
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
   <th>Review Focus</th>
  </tr> 
  <tr> 
   <td>Feldverwaltung</td> 
   <td><li>Wie viele Felder gibt es? 
   <br/>     Klicken Sie <a href="/help/marketo/product-docs/administration/field-management/export-a-list-of-all-marketo-api-field-names.md" target="_blank">Feldnamen exportieren</a>, um eine Liste Ihrer Felder, benutzerdefinierten Felder und ihrer API-Namen anzuzeigen.</li>
<li>Wie viele <a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">benutzerdefinierte Felder</a> gibt es?</li>
<li>Wie viele Felder werden verwendet? 
<br/>     Wählen <a href="/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md" target="_blank"> im Dropdown-Menü Feldaktionen die Option </a>Export von verwendet von) aus, um die zugehörigen Assets eines Felds zu überprüfen.</li>
<li>Wie viele Felder werden zwischen Marketo Engage und Ihrem CRM-System synchronisiert?</li>
<li>Werden CRM-Felder mit den entsprechenden Objekten synchronisiert?</li>
<li>Gibt es eine <a href="/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md" target="_blank">benutzerdefinierte Ansicht</a> für Personendetails? Sollte es sie geben?</li>
<li>Gibt es für Ihre Felder eine Namenskonvention, die auf der Quelle basiert? 
<br/>     Falls nicht, sollten Sie dies implementieren.</li>
<li>Gibt es Felder <a href="/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md" target="_blank">blockiert</a>? 
<br/>     Wenn ja, sollten Sie wissen, warum sie es sind.</li></td>
  </tr>
  <tr> 
   <td>Eigene Aktivitäten</td> 
   <td><li>Gibt es <a href="/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md" target="_blank">benutzerdefinierte Aktivitäten</a>?
<br/>     Wenn ja, klicken Sie durch sie, um zu verstehen, welche Aktivitäten nicht mit einem Marketo-Formular, einer E-Mail oder einer Landingpage verbunden sind.</li></td>
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
   <th>Review Focus</th>
  </tr> 
  <tr> 
   <td>E-Mail-Standardeinstellungen</td> 
   <td><li>Sind alle Ihre Standardeinstellungen in Admin &gt; E-Mail auf dem neuesten Stand (z. B. <a href="/help/marketo/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.md" target="_blank"> „von“-E-Mail-Adresse/Titel</a>, <a href="/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md" target="_blank">Branding-Domain</a>, <a href="/help/marketo/product-docs/administration/email-setup/edit-the-unsubscribe-message.md" target="_blank">Nachricht </a>, usw.)?</li></td>
  </tr>
 </tbody> 
</table>

## Integrationen {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>Mit welchem CRM synchronisieren Sie? Salesforce? MS Dynamics? Veeva?</li>
<li>Wird eine <a href="https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758" target="_blank">benutzerdefinierte Synchronisierung</a> verwendet?</li>
<li>[Nur Salesforce] Sind in Ihrer Instanz benutzerdefinierte Synchronisierungsfilter implementiert? 
<p><img src="assets/note-icon.png" alt="Notizensymbol"> HINWEIS: Wenden Sie sich an den Marketo-Support, um benutzerdefinierte Synchronisierungsfilter zu identifizieren, oder fordern Sie die Implementierung einer benutzerdefinierten Synchronisierungsregel an.</li></td>
  </tr>
  <tr> 
   <td>Landingpages</td> 
   <td><li>Wie lautet <a href="/help/marketo/product-docs/administration/settings/edit-landing-page-settings.md" target="_blank">Domain-</a>?</li>
   <li>Wie ist die Homepage festgelegt?</li>
<li>Was ist der <a href="/help/marketo/product-docs/administration/settings/set-a-fallback-page.md" target="_blank">Fallback-</a>?</li>
<li>Ist das Vorbefüllen von Formularen aktiviert?</li>
<li>Sind <a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/enable-personalized-urls-for-your-account.md" target="_blank">personalisierte URLs</a> aktiviert?</li>
<li>Gibt es Regeln für "<a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/redirect-a-marketo-landing-page-to-another-page.md" target="_blank">" </a>?</li>
<li>Haben Sie Domain-Aliase eingerichtet? Verfolgen Sie, wie Sie Ihre Domain-Aliase verwenden?</li>
<li>Ist <a href="https://nation.marketo.com/t5/knowledgebase/setting-up-secured-domains-for-marketo-landing-pages-first-time/ta-p/250370" target="_blank">Geschützte Domains für Landingpages</a> aktiviert? 
<br/>     Bestätigen Sie, ob Ihre Landingpage-Assets eine „http“-URL enthalten.</li></td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>Ist Ihr <a href="/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md" target="_blank">Munchkin-Trackingcode</a> auf Ihrer Website (keine Marketo Engage-Landingpage)?</li>
<li>Ist eine <a href="/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md" target="_blank">Do Not Track</a>-Browser-Anfrage aktiviert?</li>
<li>Ist Ihre <a href="https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking" target="_blank">Munchkin-API</a> konfiguriert? 
<p><img src="assets/tip-icon.png" alt="Tipp-Symbol">TIPP: Wenn Sie keine Dokumentation darüber haben, wo sich der Munchkin-Code auf Ihrer Website befindet, können Sie alle URLs anzeigen, indem Sie einen <a href="/help/marketo/product-docs/reporting/basic-reporting/report-types/web-page-activity-report.md" target="_blank">Web Page Activity Report</a> erstellen.</li></td>
  </tr>
  <tr> 
   <td>Webdienste</td> 
   <td><li>Sind <a href="/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md" target="_blank">IP-Einschränkungen</a> aktiviert? Sollten sie das sein?</li>
<li>Welche Benutzer/Apps führen API-Aufrufe in Ihrer Instanz durch?</li>
<li>Erreichen oder nähern Sie sich Ihrem API-Limit?
<br/>     Wenn ja, sollten Sie sie erhöhen oder Ihre Instanz überprüfen, um diese API-Aufrufe zu reduzieren.</li></td>
  </tr>
  <tr> 
   <td>Adobe Dynamic Chat (falls anwendbar)</td> 
<td>Für die folgenden Schritte ist der Zugriff auf die <a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a> erforderlich. Wenn Sie noch kein Adobe ID eingerichtet haben, finden <a href="https://helpx.adobe.com/manage-account/using/create-update-adobe-id.html" target="_blank"> hier Informationen dazu</a>.
<br/>
<li>Haben Sie die Einladung zum <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.md" target="_blank">Dynamic Chat-</a> angenommen? Die E-Mail wird gesendet, wenn Dynamic Chat in Ihrer Marketo Engage-Instanz aktiviert ist und Sie als Systemadministrator bestimmt werden.
<br/>     Suchen Sie andernfalls in Ihrem Posteingang nach der Begrüßungs-E-Mail und akzeptieren Sie die Einladung zum Einrichten Ihrer Adobe ID.</li>   
<li>Haben Sie die <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user" target="_blank">gewünschten Benutzer</a> zum Dynamic Chat-Produktprofil in Adobe Admin Console hinzugefügt?
<li>Stellen Sie sicher, dass Ihren berechtigten Benutzenden das Dynamic Chat-Produktprofil zu ihrer Adobe-Identität hinzugefügt wurde. Rollen vom Typ „Zugriff auf Dynamic Chat" können nicht in Marketo Engage &gt; „Admin“ &gt; „Benutzer und Rollen“ zugewiesen werden, wenn sie einem Produktprofil hinzugefügt werden.</li>
<li>Sind auf der Registerkarte „Produktprofile“ die Standardberechtigungen für Profile an die Anforderungen Ihres Unternehmens angepasst?<br/> 
Ist dies nicht der Fall, bearbeiten Sie die Berechtigungen für das jeweilige Profil. </li>
<li>Wenn Sie mehr als ein Abonnement haben, werden Ihre Benutzer zu den richtigen Abonnements hinzugefügt?</li>
<br>
Nachdem Sie die Prüfung der Einstellungen für Benutzer und Rollen abgeschlossen haben, melden Sie sich bei Dynamic Chat an, um mit der Prüfung fortzufahren.  
<li>Haben Sie <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md" target="_blank">Ihre Marketo Engage-Instanz</a> mit Dynamic Chat verbunden?</li>
<li>Sind die fünf Standardprofile mit vordefinierten Berechtigungen auf Ihre Organisation anwendbar?<br/> 
     Andernfalls können Sie sie <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#edit-existing-permissions" target="_blank">in Dynamic Chat bearbeiten</a>. Sie können auch <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#create-a-profile" target="_blank">Benutzerdefiniertes Profil erstellen</a> mit einem benutzerdefinierten Berechtigungssatz.</li>
<li>Um Ihren Benutzerinnen und Benutzern Zugriff auf Dynamic Chat zu gewähren, haben Sie in „Zugriff auf Dynamic Chat" die entsprechende Marketo Engage-Rolle unter „Admin“ &gt; „Benutzerinnen und Benutzer &amp; Rollen“ &gt; „Rollen“ ausgewählt?
<br/><img src="assets/note-icon.png" alt="Notizensymbol"> HINWEIS: Die Rollen „Admin“ und „Marketing-Benutzer“ sollten Zugriff auf Dynamic Chat haben.</li>
</td>
  </tr>
  <td>Marketo Sales Insight (falls zutreffend)</td> 
   <td><li>Wurde das <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">MSI-Paket installiert</a>?</li>
<li>Haben <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank"> ein Upgrade auf die neueste Version von Sales Insight </a>?</li>
<li>Haben Sie die Sales Insight-Konfiguration abgeschlossen? <br/>     Enterprise/Unlimited Users <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">hier klicken</a>, Professional Users <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">hier klicken</a>.</li>
<li>Haben Sie <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">Zugriff auf Ihre Benutzer erteilt</a> basierend auf der Anzahl der erworbenen Lizenzen?</li>
<li>Sind <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md" target="_blank">Sterne und Flammen</a> angepasst?</li></td>
  </tr>
  <tr> 
   <td>Startpunkt (falls zutreffend)</td> 
   <td><li>Welche Services haben Sie konfiguriert (z. B. <a href="/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md" target="_blank">BrightTALK</a>, <a href="/help/marketo/product-docs/administration/additional-integrations/connect-brighttalk-to-marketo.md" target="_blank">Zoom</a> usw.)? Sind irgendwelche in der Nähe ihres Ablaufs?</li>
<li><a href="https://nation.marketo.com/t5/knowledgebase/viewing-your-number-of-api-calls-to-marketo/ta-p/254256" target="_blank">Wie viele API-Aufrufe </a> Ihre Integrationen?</li>
<li>Verfügen Sie über die richtigen Integrationen für Ihre Anwendungsfälle?</li></td>
  </tr>
  <tr> 
   <td>Webhooks (falls zutreffend)</td> 
   <td><li><a href="/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md" target="_blank">Welche Verbindungen</a> haben Sie eingerichtet?</li>
<li>Werden keine mehr verwendet?</li></td>
  </tr>
  <tr> 
   <td>Mobile Apps (falls zutreffend)</td> 
   <td><li>Welche <a href="/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md" target="_blank">Mobile Apps</a> haben Sie?</li>
<li>Wurden <a href="/help/marketo/product-docs/mobile-marketing/push-notifications/adding-a-new-test-device.md" target="_blank">Testgeräte</a> hinzugefügt?</li></td>
  </tr>
 </tbody> 
</table>

## Schatzkiste {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr> 
  <tr> 
   <td>Schatzkiste</td> 
   <td><li>Was ist in der <a href="/help/marketo/product-docs/administration/settings/enable-or-disable-treasure-chest-features.md" target="_blank">Schatztruhe“ </a>?</li>
<li>Gibt es Funktionen, die ein- oder ausgeschaltet werden sollten?</li></td>
  </tr>
  <tr> 
   <td>Kampagnenprüfung</td> 
   <td><li>Ist <a href="/help/marketo/product-docs/administration/settings/campaign-inspector.md" target="_blank">Kampagneninspektor</a> aktiviert?
<br/>Wenn nicht, sollten Sie sie aktivieren, um leicht zu erkennen, welche Kampagnen aktiv sind: mit Ihrem CRM synchronisieren und/oder Datensätze löschen.</li></td>
  </tr>
 </tbody> 
</table>

## Warnhinweise und Aktualisierungen {#alerts-and-updates}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Bereich</th>
   <th>Review Focus</th>
  </tr> 
  <tr> 
   <td>Statusaktualisierungen zu Marketo Engage</td> 
   <td><li>Ist Ihre Instanz für <a href="https://nation.marketo.com/t5/knowledgebase/how-to-subscribe-to-status-page-notifications/ta-p/296749" target="_blank">Marketo Engage-Statusaktualisierungen abonniert</a>?</li></td>
  </tr>
  <tr> 
   <td>Warnhinweise</td> 
   <td><li>Gibt es <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md" target="_blank">aktive Warnhinweise</a> die von Marketo Engage an interne Teams gesendet werden?</li>
<li>Wenn ja, funktionieren diese Warnhinweise ordnungsgemäß?</li></td>
  </tr>
  <tr> 
   <td>Benachrichtigungen</td> 
   <td><li>Sind geeignete Admin-Benachrichtigungen (<a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md" target="_blank">) </a>?</li></td>
  </tr>
 </tbody> 
</table>
