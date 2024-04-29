---
description: Checkliste für die frühe Einrichtung - Marketo-Dokumente - Produktdokumentation
title: Checkliste für frühe Einrichtung
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 8473c4d59210bb18c3968a56883034febf00c320
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 1%

---

# NEUER BEREICH: Checkliste für frühzeitige Einrichtung {#early-setup-checklist}

Text einfügen.

## Marketo Engage auf Adobe Identity Management {#marketo-engage-on-adobe-identity-management}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Produkt-Admin für Marketo Engage und Abonnement </td>
    <td><li>Vergewissern Sie sich, dass Ihr Adobe Org-Systemadministrator Ihnen eine Adobe Product Admin-Rolle zugewiesen hat.</li>  
    <ul>
    <li>Kontakt <a href="https://helpx.adobe.com/contact.html">Adobe-Kundenunterstützung</a> herauszufinden, wer in Ihrer Organisation <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe Admin Console-Systemadministrator</a> -Berechtigungen.</li></ul>
    <li>Akzeptieren Sie die Einladung "Marketo Engage Product Admin", um Ihre Adobe ID zu aktivieren. Die <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=en#create-a-product-profile">Willkommens-E-Mail</a> wird gesendet, wenn die Rolle in der Adobe Admin Console zugewiesen wird.</li></td>
  </tr>
  <tr>
    <td>Produktprofile</td>
    <td><li>Weisen Sie alle entsprechenden Benutzer der Marketo Engage zu. <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">Produktprofil</a> in Adobe Admin Console.</li>
    <ul>
    <li>Sie können Benutzerrollen nicht in Marketo Engage/Admin/Anwendern und Rollen zuweisen, bevor Sie sie zu einem Produktprofil hinzufügen.</li>
    <li>Jedes Abonnement wird ein eigenständiges Produktprofil sein. Wenn ein unerwünschter Benutzer mehreren Produktprofilen hinzugefügt wird (z. B. Produktions- und Test-Sandbox), müssen Sie den Benutzer aus allen Produktprofilen löschen. Andernfalls haben sie weiterhin Zugriff auf Marketo Engage.</li></ul></td>
  </tr>
  <tr>
    <td>Benutzer</td>
    <td><li>Erstellen einer Richtlinie zum Zeitpunkt <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html">Benutzer erstellen</a>.</li> <li>Erstellen Sie eine Richtlinie, um festzulegen, wann Benutzer entfernt werden sollen.</li>
    <li>Bestimmen, wer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe System Admin- und Marketo Engage Product Admin-Berechtigungen.</a> <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">Benutzer hinzufügen</a> zum gewünschten Produktprofil.</li>
    <li>Erstellen Sie für jeden API-Anwendungsfall einen API-Benutzer.</li></td>
  </tr>
  <tr>
    <td>Support-Administrator </td>
    <td><li>nach <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#create-a-support-ticket-with-admin-console">Senden eines Support-Tickets in Adobe Admin Console</a>müssen Sie die Rolle "Produktsupport-Administrator"von einem Systemadministrator den von Ihnen verwalteten Abonnements zuweisen lassen. Nur ein Systemadministrator in Ihrem Unternehmen kann <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#assign-the-support-admin-role">Sie dieser Rolle zuweisen</a>.</li>
    <li>Möglicherweise haben Sie vom Systemadministrator eine E-Mail mit der Information erhalten, dass Sie der Support-Administrator für Ihr Marketo Engage-Abonnement sind. Wenn ja, klicken Sie auf <a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#assign-the-support-admin-role">"Erste Schritte"in der E-Mail</a> , um Mitglied der Organisation zu werden.</li>
    <li>Bestimmen Sie die entsprechenden Kontakte (mit mindestens einem Backup-Kontakt) und lassen Sie den Systemadministrator die Rolle "Produktsupport-Administrator"im Voraus entsprechend zuweisen.</li></td>
  </tr>
</tbody>
</table>

## Dynamic Chat bei der Adobe Identity Management-Einrichtung {#dynamic-chat-on-adobe-identity-management}

TEXT

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Dynamic Chat Product Admin (falls zutreffend) </td>
    <td><li>Bestätigen Sie, ob Ihr Adobe Org-Systemadministrator Ihnen eine Adobe Product Admin-Rolle zugewiesen hat. Kontakt <a href="https://helpx.adobe.com/contact.html">Adobe-Kundenunterstützung</a> , um herauszufinden, wer in Ihrem Unternehmen über Administratorrechte in der Konsole verfügt.</li>
    <li>Accept <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">Einladung "Dynamic Chat Product Admin"</a>. Die <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">Willkommens-E-Mail</a> wird gesendet, wenn Dynamic Chat in Ihrer Marketo Engage-Instanz aktiviert ist und Sie als Systemadministrator benannt sind.</li></td>
  </tr>
  <tr>
    <td>Produktprofile </td>
    <td><li>Weisen Sie alle entsprechenden Benutzer dem Dynamic Chat-Produktprofil in Adobe Admin Console zu.</li> 
    <ul>
    <li>Wenn ein unerwünschter Benutzer mehreren Produktprofilen hinzugefügt wird, müssen Sie den Benutzer aus allen Produktprofilen löschen. Andernfalls haben sie weiterhin Zugriff auf Dynamic Chat.</li>
    <li>Sie können <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">Bearbeiten von Produktprofilen in Dynamic Chat</a> und erstellen Sie ein benutzerdefiniertes Profil mit einem benutzerdefinierten Satz von <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">In Ihrem Abonnement verfügbare Berechtigungen</a>.</li></td>
  </tr>
  <tr>
    <td>Benutzer </td>
    <td><li>Erstellen Sie eine Richtlinie zum Hinzufügen und Entfernen eines Chat-Benutzers.</li>
    <li>Erstellen Sie eine Richtlinie für die <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">Adobe Dynamic Chat der Produktadministratorberechtigungen.</a></li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">Benutzer zum gewünschten Produktprofil hinzufügen</a>.</li></td>
  </tr>
</tbody>
</table>

## Einrichten laufender Systemaktualisierungen und Kommunikationen

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Adobe Marketo-Statusaktualisierungen </td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">Adobe Marketo Engage-Statusaktualisierungen abonnieren</a>.</li></td>
  </tr>
  <tr>
    <td>Benachrichtigungen </td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">Abonnieren von Administratorbenachrichtigungen</a> für wichtige Probleme wie Fehler in Ihren Smart-Kampagnen und kritische Probleme bei der CRM-Synchronisierung.</li></td>
  </tr>
</tbody>
</table>
