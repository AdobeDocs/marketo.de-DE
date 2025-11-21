---
description: Bevor Sie Ihre neue Marketo Engage-Instanz einrichten, müssen Sie ein paar grundlegende Schritte für die kontinuierliche Nutzung durchführen. Zu diesen Schritten gehören die Einrichtung von Benutzerkonten, die Einrichtung von Admins zur Unterstützung und das Abonnieren laufender Systemaktualisierungen.
short-description: Erfahren Sie nach Abschluss der ersten Einrichtungsschritte, wie Sie grundlegende Elemente erstellen, um eine reibungslose fortlaufende Nutzung zu gewährleisten.
title: Benutzer-Setup-Checkliste
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 7%

---

# Benutzer-Setup-Checkliste {#user-setup-checklist}

Nachdem Sie nun alle &quot;[&#x200B; Einrichtungsschritte“ abgeschlossen haben](/help/marketo/getting-started/initial-setup/setup-steps.md){target="_blank"} ist es an der Zeit, einige grundlegende Elemente einzurichten, um eine reibungslose fortlaufende Verwendung sicherzustellen. Dadurch wird die Grundlage für Ihre Journey mit Marketo Engage gelegt und Sie können die Funktionen von nutzen. Los geht‘s!

>[!NOTE]
>
>Sie können diese Checkliste ([&#x200B; einer Liste mit Best &#x200B;](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx)) für Ihre neue Instanz auch herunterladen und die Schritte sofort abhaken.

## Marketo Engage auf Adobe Identity Management {#marketo-engage-on-adobe-identity-management}

Ihre neuen Marketo Engage-Abonnements wurden in das [Adobe Identity Management System (IMS) &#x200B;](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html). Fahren Sie mit der folgenden Überprüfung der Benutzerverwaltung in Adobe Admin Console fort.

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Abonnement und Marketo Engage-Produktadministrator</td>
    <td><li>Vergewissern Sie sich, dass Ihnen von Ihrem Adobe-Organisations-Systemadministrator die Rolle "Adobe-Produktadministrator“ zugewiesen wurde.</li>
    <ul>
    <li>Wenden Sie sich an das Adobe-Account-Team (Ihren Account Manager) oder senden Sie eine E-Mail an <code>marketocares@marketo.com</code>, um herauszufinden, wer in Ihrem Unternehmen über <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe Admin Console-</a> verfügt.</li></ul>
    <li>Akzeptieren Sie die Einladung "Marketo Engage-Produktadministrator“, um Ihre Adobe ID zu aktivieren. Die <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=en#create-a-product-profile">Begrüßungs-E</a>Mail wird gesendet, wenn die Rolle in der Adobe Admin Console zugewiesen wird.</li></td>
  </tr>
  <tr>
    <td>Produktprofile</td>
    <td><li>Weisen Sie alle gewünschten Benutzenden dem Marketo Engage-Produktprofil <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">Adobe Admin Console</a> zu.</li>
    <ul>
    <li>Vor dem Hinzufügen zu einem Produktprofil können Sie in Marketo Engage &gt; Admin &gt; Benutzer &amp; Rollen keine Benutzerrollen zuweisen.</li>
    <li>Jedes Abonnement ist ein eigenständiges Produktprofil. Wenn ein unerwünschter Benutzer mehreren Produktprofilen hinzugefügt wird (z. B. Produktions- und Test-Sandbox), müssen Sie den Benutzer aus allen Produktprofilen löschen. Andernfalls haben sie weiterhin Zugriff auf Marketo Engage.</li></ul></td>
  </tr>
  <tr>
    <td>Benutzer</td>
    <td><li>Erstellen Sie eine Richtlinie zum Zeitpunkt der <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html">Erstellung eines Benutzers</a>.</li> <li>Erstellen Sie eine Richtlinie zum Zeitpunkt der Benutzerentfernung.</li>
    <p><img src="assets/note-icon.png" alt="Notizensymbol"> HINWEIS: Sie müssen Systemadministrator sein, um Benutzer entfernen zu können.
    <li>Legen Sie fest, wer über <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe-Systemadministrator- und Marketo Engage-Produktadministrator-Berechtigungen verfügen soll.</a> <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">Benutzer hinzufügen</a> zum gewünschten Produktprofil hinzufügen.</li>
    <li>Erstellen Sie für jeden API-Anwendungsfall einen API-Benutzer.</li></td>
  </tr>
  <tr>
    <td>User Management-API (falls zutreffend)</td>
    <td><li>Verwenden Sie die <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html">Adobe User Management-</a>, um Benutzer einzuladen, zu aktualisieren und zu löschen.</li>
    <li>Verwenden Sie die <a href="https://developer.adobe.com/umapi/">Adobe User Management-</a>, um Rollen (z. B. Administratoren, Support-Administratoren, Entwickler) hinzuzufügen oder zu entfernen.</li>
    </td>
  </tr>
  <tr>
    <td>Produktsupport-Administrator</td>
    <td><li>Um <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#create-a-support-ticket-with-admin-console">Support-Ticket in der Adobe Admin Console einreichen</a>, muss Ihnen von einem Systemadministrator die Rolle „Produktsupport-Administrator“ zugewiesen worden sein. Nur ein Systemadministrator in Ihrer Organisation kann <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#assign-the-support-admin-role">Sie dieser Rolle zuweisen</a>.</li>
    <li>Möglicherweise haben Sie eine E-Mail vom Systemadministrator erhalten, in der Sie angegeben haben, dass Sie der Support-Administrator für Ihr Marketo Engage-Abonnement sind. Wenn ja, klicken <a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#assign-the-support-admin-role"> in der E-Mail auf </a>Erste Schritte“, um der Organisation beizutreten.</li>
    <li>Bestimmen Sie die entsprechenden Kontakte (mit mindestens einem Backup-Kontakt) und weisen Sie dem Systemadministrator die Rolle des Produktsupport-Administrators entsprechend zu.</li></td>
  </tr>
</tbody>
</table>

## Einrichten von Dynamic Chat in Adobe Identity Management {#dynamic-chat-on-adobe-identity-management}

Um [Dynamic Chat](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html), den nativen Kanal zur Konversationsautomatisierung in Marketo Engage, zu verwenden, fahren Sie mit der Einrichtung der Benutzerberechtigungen fort, indem Sie die folgenden Schritte in der [Adobe Admin Console &#x200B;](https://adminconsole.adobe.com/){target="_blank"}.

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Abonnement und Dynamic Chat-Produktadministrator (falls zutreffend)</td>
    <td><li>Vergewissern Sie sich, dass Ihnen von Ihrem Adobe-Organisations-Systemadministrator die Rolle "Adobe-Produktadministrator“ zugewiesen wurde.</li>
    <ul><li>Wenden Sie sich an das Adobe-Account-Team (Ihren Account Manager) oder senden Sie eine E-Mail an <code>marketocares@marketo.com</code>, um herauszufinden, wer in Ihrem Unternehmen über <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe Admin Console-</a> verfügt.</li></ul>
    <li>Akzeptieren Sie die Einladung des <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html"> Dynamic Chat</a>Produktadministrators. Die <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">Begrüßungs-E</a>Mail wird gesendet, wenn Dynamic Chat in Ihrer Marketo Engage-Instanz aktiviert ist und Sie als Systemadministrator bestimmt werden.</li></td>
  </tr>
  <tr>
    <td>Produktprofile</td>
    <td><li>Weisen Sie alle gewünschten Benutzenden dem Produktprofil des dynamischen Chats in Adobe Admin Console zu.</li>
    <ul>
    <li>Wenn ein unerwünschter Benutzer mehreren Produktprofilen hinzugefügt wird, müssen Sie ihn aus allen Produktprofilen löschen. Andernfalls haben sie weiterhin Zugriff auf Dynamic Chat.</li>
    <li>Sie können <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">Produktprofile in Dynamic Chat bearbeiten</a> und ein benutzerdefiniertes Profil mit einem benutzerdefinierten Satz von (<a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions"> in Ihrem Abonnement verfügbaren) </a>.</li></td>
  </tr>
  <tr>
    <td>Benutzer</td>
    <td><li>Erstellen Sie eine Richtlinie darüber, wann ein Chat-Benutzer hinzugefügt und entfernt werden soll.</li>
    <li>Erstellen Sie eine Richtlinie für Benutzer mit <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">Adobe Dynamic Chat-Produktadministratorberechtigungen.</a></li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">Fügen Sie dem gewünschten Produktprofil Benutzer hinzu</a>.</li></td>
  </tr>
</tbody>
</table>

## Einrichten laufender Systemaktualisierungen und Kommunikationen {#system-updates}

<table>
<thead>
  <tr>
    <th style="width:20%">Bereich</th>
    <th style="width:80%">Aktionselemente</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Statusaktualisierungen zu Adobe Marketo</td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">Adobe Marketo Engage-Statusaktualisierungen abonnieren</a>.</li></td>
  </tr>
  <tr>
    <td>Benachrichtigungen</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">Abonnieren Sie Admin</a>Benachrichtigungen für kritische Probleme wie Fehler in Ihren Smart-Kampagnen und kritische Probleme bei der CRM-Synchronisierung.</li></td>
  </tr>
</tbody>
</table>

<p>

Nachdem Ihr Marketo Engage-Konto nun einsatzbereit ist, lesen Sie bitte den Abschnitt [Best Practices für eine neue Marketo Engage-Instanz](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/where-to-start.md){target="_blank"}, um Ihre Investition optimal zu nutzen und sich für den langfristigen Erfolg einzurichten.
