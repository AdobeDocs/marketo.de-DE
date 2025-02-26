---
description: Handbuch zur Fehlerbehebung bei Adobe IMS - Marketo-Dokumente - Produktdokumentation
title: Handbuch zur Fehlerbehebung bei Adobe IMS
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
source-git-commit: eccebb8352c56770dea5af9395c8bc83a08525dd
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Handbuch zur Fehlerbehebung bei Adobe IMS {#adobe-ims-troubleshooting-guide}

Während der IMS-Benutzermigration wird für jeden migrierten Marketo Engage-Benutzer ein Adobe-Benutzer erstellt. Manchmal wird sie nicht erstellt (aus verschiedenen Gründen, die mit dem Benutzerdatensatz im Active Directory oder Problemen mit der E-Mail-Adresse zusammenhängen). In diesem Fall werden dem Marketo Engage-Administrator die Gründe im Feld Migrationsstatus der Benutzerin bzw. des Benutzers auf der Selbstmigrationskonsole angezeigt. Unten finden Sie Informationen zum Beheben verschiedener Probleme bei der Adobe-Benutzererstellung.

## Fehlermeldungen {#error-messages}

* <a href="#not-in-directory">Nicht im Verzeichnis</a>
* <a href="#gmail-invalid-character">Ungültiges Gmail-Zeichen</a>
* <a href="#inactive-user">Inaktiver Benutzer</a>
* <a href="#not-in-domain">Nicht in Domain</a>
* <a href="#create-failure">Fehler beim Erstellen</a>
* <a href="#type2e-user-failure">Type2e-Benutzerfehler</a>



<table>
<thead>
  <tr>
    <th style="width:20%">Fehlermeldung</th>
    <th style="width:40%">Grundursache</th>
    <th style="width:40%">Auflösungen</th>
  </tr>
  </thead>
<tbody>
  <tr>
    <td><i><a id="not-in-directory">Nicht im Verzeichnis</a></i></td>
    <td>Der Benutzer ist nicht in Active Directory (AD) vorhanden. Für alle Organisationen mit SSO, für die die AD-Synchronisierung aktiviert ist, ist die Benutzererstellung nur über den Identitätsanbieter (IdP) zulässig. Daher konnte der Benutzer während der Benutzermigration nicht über Admin Console hinzugefügt werden.</td>
    <td>Migrieren : Der Benutzer muss dem Active Directory mit entsprechenden Berechtigungen hinzugefügt werden. Marketo Admin, um die Benutzermigration für diesen Benutzer über die Migrationskonsole erneut auszuführen. 
    <br>Nicht migrieren - Marketo-Administrator, um den Benutzer in der Migrationskonsole zu überspringen. Die Schaltfläche „Migration abgeschlossen“ wird angezeigt, wenn alle Benutzer durch Migration oder Überspringen berücksichtigt werden. Klicken Sie darauf, um den Prozess der Benutzermigration abzuschließen.</td>
  </tr>
  <tr>
    <td><i><a id="gmail-invalid-character">Ungültiges Gmail-Zeichen</a></i></td>
    <td>Gemäß Adobes Sicherheitsrichtlinie, ".“ und "+"-Zeichen sind nur in einer E-Mail-Adresse der Gmail-Domain zulässig  
    <br>Beide Sonderzeichen sind in einer E-Mail-Adresse, die keine Gmail-Domain ist, zulässig. </td>
    <td>Migrieren : Die E-Mail-Adresse muss in Marketo Engage aktualisiert werden, um die Sicherheitsrichtlinien von Adobe zu erfüllen. Marketo Admin, um die Benutzermigration für diesen Benutzer über die Migrationskonsole erneut auszuführen.<br>Nicht migrieren - Marketo-Administrator, um den Benutzer in der Migrationskonsole zu überspringen. Die Schaltfläche „Migration abgeschlossen“ wird angezeigt, wenn alle Benutzer durch Migration oder Überspringen berücksichtigt werden. Klicken Sie darauf, um den Prozess der Benutzermigration abzuschließen.</td>
  </tr>
  <tr>
    <td><i><a id="inactive-user">Inaktiver Benutzer</a></i></td>
    <td>Die AD-Synchronisierung ist aktiviert und das Federated-Konto des Benutzers existiert, jedoch im Status „Inaktiv/Deaktiviert“.</td>
    <td>Migrieren : Der Status und die ordnungsgemäßen Berechtigungen des Benutzers müssen wiederhergestellt werden. Marketo Admin, um die Benutzermigration für diesen Benutzer über die Migrationskonsole erneut auszuführen.
    <br>Nicht migrieren - Marketo-Administrator, um den Benutzer in der Migrationskonsole zu überspringen. Die Schaltfläche „Migration abgeschlossen“ wird angezeigt, wenn alle Benutzer durch Migration oder Überspringen berücksichtigt werden. Klicken Sie darauf, um den Prozess der Benutzermigration abzuschließen.</td>
  </tr>
  <tr>
    <td><i><a id="not-in-domain">Nicht in Domäne</a></i></td>
    <td>Die Domain-Durchsetzung ist in Admin Console aktiviert, aber die Domain der E-Mail-Adresse des Benutzers ist keine der zulässigen Domains. 
    <br>Richtlinien zur Domain-Durchsetzung werden auf Ordnerebene festgelegt.</td>
    <td>Migrieren - Die E-Mail-Adresse muss in Marketo Engage aktualisiert werden, um der Domain-Durchsetzungsrichtlinie zu entsprechen. Andernfalls kann der Systemadministrator bzw. die Systemadministratorin <a href="https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories"> 
    Verschieben Sie die Domain in ein anderes deaktiviertes Verzeichnis der Domain-Durchsetzung </a>oder <a href="https://helpx.adobe.com/de/enterprise/using/set-up-identity.html">erstellen Sie ein neues Verzeichnis</a>, das nicht unter der DE-Richtlinie steht. Marketo Admin, um die Benutzermigration für diesen Benutzer über die Migrationskonsole erneut auszuführen. <br>Nicht migrieren - Marketo-Administrator, um den Benutzer in der Migrationskonsole zu überspringen. Die Schaltfläche „Migration abgeschlossen“ wird angezeigt, wenn alle Benutzer durch Migration oder Überspringen berücksichtigt werden. Klicken Sie darauf, um den Prozess der Benutzermigration abzuschließen.</td>
  </tr>
  <tr>
    <td><i><a id="create-failure">Fehler beim Erstellen</a></i></td>
    <td>Verschiedene Gründe im Backend.</td>
    <td>Bitte reichen Sie einen Support-Fall ein.</td>
  </tr>
  <tr>
    <td><i><a id="type2e-user-failure">Type2e-Benutzerfehler</a></i></td>
    <td>Verschiedene Gründe im Backend.</td>
    <td>Bitte reichen Sie einen Support-Fall ein.</td>
  </tr>
</tbody>
</table>
