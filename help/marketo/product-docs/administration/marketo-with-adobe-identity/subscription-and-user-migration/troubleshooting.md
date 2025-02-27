---
description: Handbuch zur Fehlerbehebung bei Adobe IMS - Marketo-Dokumente - Produktdokumentation
title: Handbuch zur Fehlerbehebung bei Adobe IMS
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: a2186f054e7b7a780098157927651a084e353bd8
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Handbuch zur Fehlerbehebung bei Adobe IMS {#adobe-ims-troubleshooting-guide}

Während der IMS-Benutzermigration wird für jeden migrierten Marketo Engage-Benutzer ein Adobe-Benutzer erstellt. Manchmal wird sie nicht erstellt (aus verschiedenen Gründen, die mit dem Benutzerdatensatz im Active Directory oder Problemen mit der E-Mail-Adresse zusammenhängen). In diesem Fall wird dem Marketo Engage-Administrator der Grund im Feld Migrationsstatus des Benutzers auf der Selbstmigrationskonsole angezeigt.

## Fehlermeldungen {#error-messages}

Verwenden Sie den Abschnitt „Auf dieser Seite“ auf der rechten Seite, um direkt zu einem bestimmten Fehler zu springen und zu erfahren, wie Sie ihn beheben können.

### Nicht im Verzeichnis {#not-in-directory}

_Grundursache_: Der Benutzer existiert nicht in Active Directory (AD). Für alle Organisationen mit SSO, für die die Anzeigensynchronisierung aktiviert ist, ist die Benutzererstellung nur über den Identitätsanbieter (IdP) zulässig. Daher konnte der Benutzer während der Benutzermigration nicht über Admin Console hinzugefügt werden.

_Auflösungen_:

Vorab-Migration - Geben Sie dem Marketo-Administrator die Möglichkeit, den Benutzer bzw. die Benutzerin in der Migrationskonsole zu überspringen. Die Schaltfläche „Migration abgeschlossen“ wird angezeigt, wenn alle Benutzer durch Migration oder Überspringen berücksichtigt werden. Klicken Sie auf die Schaltfläche , um den Prozess der Benutzermigration abzuschließen.

Nach der Migration: Der Benutzer muss dem Active Directory mit entsprechenden Berechtigungen hinzugefügt werden. Marketo Engage Admin, um die Benutzermigration für diesen Benutzer über die Migrationskonsole erneut auszuführen.

### Ungültiges Gmail-Zeichen {#gmail-invalid-character}

_Grundursache_: Gemäß der Adobe-Sicherheitsrichtlinie sind die Zeichen `.` und `+` in einer Gmail-E-Mail-Adresse nicht zulässig. Beide Zeichen sind nur in Nicht-Gmail-E-Mail-Adressen zulässig.

_Auflösungen_:

Vorab-Migration - Geben Sie dem Marketo-Administrator die Möglichkeit, den Benutzer bzw. die Benutzerin in der Migrationskonsole zu überspringen. Die Schaltfläche „Migration abgeschlossen“ wird angezeigt, wenn alle Benutzer durch Migration oder Überspringen berücksichtigt werden. Klicken Sie auf die Schaltfläche , um den Prozess der Benutzermigration abzuschließen.

Nach der Migration - Die E-Mail-Adresse muss in Marketo Engage aktualisiert werden, damit sie der Sicherheitsrichtlinie von Adobe entspricht. Marketo Admin, um die Benutzermigration für diesen Benutzer über die Migrationskonsole erneut auszuführen.

### Inaktiver Benutzer {#inactive-user}

_Grundursache_: Die AD-Synchronisierung ist aktiviert und das Federated-Konto des Benutzers existiert, jedoch im Status „Inaktiv/Deaktiviert“.

_Auflösungen_:

Vorab-Migration - Geben Sie dem Marketo-Administrator die Möglichkeit, den Benutzer bzw. die Benutzerin in der Migrationskonsole zu überspringen. Die Schaltfläche „Migration abgeschlossen“ wird angezeigt, wenn alle Benutzer durch Migration oder Überspringen berücksichtigt werden. Klicken Sie auf die Schaltfläche , um den Prozess der Benutzermigration abzuschließen.

Nach der Migration: Der Status und die ordnungsgemäßen Berechtigungen des Benutzers müssen wiederhergestellt werden. Marketo Engage Admin, um die Benutzermigration für diesen Benutzer über die Migrationskonsole erneut auszuführen.

### Nicht in Domäne {#not-in-domain}

_Grundursache_: Die Domain-Durchsetzung ist in der Admin Console aktiviert, aber die Domain der E-Mail-Adresse der Benutzerin oder des Benutzers ist keine der zulässigen Domains.

_Auflösungen_:

Vorab-Migration - Geben Sie dem Marketo-Administrator die Möglichkeit, den Benutzer bzw. die Benutzerin in der Migrationskonsole zu überspringen. Die Schaltfläche „Migration abgeschlossen“ wird angezeigt, wenn alle Benutzer durch Migration oder Überspringen berücksichtigt werden. Klicken Sie auf die Schaltfläche , um den Prozess der Benutzermigration abzuschließen.

Nach der Migration - Die E-Mail-Adresse muss in Marketo Engage aktualisiert werden, damit sie der Domain Enforcement (DE)-Richtlinie entspricht. Alternativ kann der Systemadministrator die Domain entweder [in einen anderen ](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"}-Ordner (DE) verschieben oder [einen neuen Ordner erstellen](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"} der nicht unter der DE-Richtlinie steht. Marketo Engage Admin, um die Benutzermigration für diesen Benutzer über die Migrationskonsole erneut auszuführen.

### Fehler beim Erstellen {#create-failure}

_Grundursache_ Dieser Fehler kann im Backend aus verschiedenen Gründen auftreten.

_Auflösungen_:

Vorab-Migration - Bitte senden Sie ein Ticket für den technischen Support für die [, die noch nicht migriert ](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

Nach der Migration - Bitte senden Sie einen Support-Fall für die [bereits migrierten](https://experienceleague.adobe.com/home?support-tab=home#support){target="_blank"}.

### Type2e-Benutzerfehler {#type2e-user-failure}

_Grundursache_ Dieser Fehler kann im Backend aus verschiedenen Gründen auftreten.

_Auflösungen_:

Vorab-Migration - Bitte senden Sie ein Ticket für den technischen Support für die [, die noch nicht migriert ](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

Nach der Migration - Bitte senden Sie einen Support-Fall für die [bereits migrierten](https://experienceleague.adobe.com/home?support-tab=home#support){target="_blank"}.
