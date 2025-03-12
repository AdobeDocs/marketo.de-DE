---
description: Handbuch zur Fehlerbehebung bei der Adobe IMS-Benutzermigration - Marketo-Dokumente - Produktdokumentation
title: Handbuch zur Fehlerbehebung bei der Adobe IMS-Benutzermigration
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: e96bc8676a73694ec60f46bb045f2a6ea5d8069c
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Handbuch zur Fehlerbehebung bei der Adobe IMS-Benutzermigration {#adobe-ims-user-migration-troubleshooting-guide}

Während der IMS-Benutzermigration wird für jeden migrierten Marketo Engage-Benutzer ein Adobe-Benutzer erstellt (es sei denn, er existiert bereits mit derselben E-Mail-Adresse). Manchmal wird er nicht erstellt, was auf den Datensatz des Benutzers im Active Directory oder Probleme mit der E-Mail-Adresse zurückgeführt werden kann. In diesem Fall wird dem Marketo Engage-Administrator der Grund im Feld Migrationsstatus des Benutzers in der Selbstmigrationskonsole angezeigt.

## Fehlermeldungen {#error-messages}

Bestimmen Sie zunächst, ob der Benutzer migriert werden muss oder nicht, da dies Auswirkungen auf die zu befolgenden Auflösungsschritte hat.

Verwenden Sie den Abschnitt „Auf dieser Seite“ rechts, um direkt zu einem bestimmten Fehler zu springen.

### Nicht im Verzeichnis {#not-in-directory}

**Grundursache**: Der Benutzer existiert nicht in Active Directory (AD). Für alle Organisationen mit SSO, für die die Anzeigensynchronisierung aktiviert ist, ist die Benutzererstellung nur über den Identitätsanbieter (IdP) zulässig. Daher konnte der Benutzer während der Benutzermigration nicht über Admin Console hinzugefügt werden.

**Auflösungen**:

_Wenn der Benutzer nicht migriert werden muss_ - Marketo Engage-Administrator, um den Benutzer in der Migrationskonsole zu überspringen. Die Schaltfläche „Migration abgeschlossen“ wird angezeigt, wenn alle Benutzer durch Migration oder Überspringen berücksichtigt werden. Klicken Sie auf die Schaltfläche , um den Prozess der Benutzermigration abzuschließen.

_Wenn der Benutzer migriert werden muss_ - Der Benutzer muss von einem Systemadministrator mit den entsprechenden Berechtigungen zum Active Directory hinzugefügt werden. Marketo Engage Admin, um die Benutzermigration für diesen Benutzer über die Migrationskonsole erneut auszuführen.

### Ungültiges Gmail-Zeichen {#gmail-invalid-character}

**Grundursache**: Gemäß der Adobe-Sicherheitsrichtlinie sind die Zeichen `.` und `+` in einer Gmail-E-Mail-Adresse nicht zulässig. Beide Zeichen sind in Nicht-Gmail-E-Mail-Adressen zulässig.

**Auflösungen**:

_Wenn der Benutzer nicht migriert werden muss_ - Marketo Engage-Administrator, um den Benutzer in der Migrationskonsole zu überspringen. Die Schaltfläche „Migration abgeschlossen“ wird angezeigt, wenn alle Benutzer durch Migration oder Überspringen berücksichtigt werden. Klicken Sie auf die Schaltfläche , um den Prozess der Benutzermigration abzuschließen.

_Wenn der Benutzer migriert werden muss_ - Die E-Mail-Adresse muss in Marketo Engage aktualisiert werden, um die Sicherheitsrichtlinien von Adobe zu erfüllen, und erneut überprüft werden. Marketo Admin, um die Benutzermigration für diesen Benutzer über die Migrationskonsole erneut auszuführen.

### Inaktiver Benutzer {#inactive-user}

**Grundursache**: Die AD-Synchronisierung ist aktiviert und das Federated-Konto des Benutzers existiert, jedoch im Status „Inaktiv/Deaktiviert“.

**Auflösungen**:

_Wenn der Benutzer nicht migriert werden muss_ - Marketo Engage-Administrator, um den Benutzer in der Migrationskonsole zu überspringen. Die Schaltfläche „Migration abgeschlossen“ wird angezeigt, wenn alle Benutzer durch Migration oder Überspringen berücksichtigt werden. Klicken Sie auf die Schaltfläche , um den Prozess der Benutzermigration abzuschließen.

_Wenn der Benutzer migriert werden muss_ - Der Status und die Berechtigungen des Benutzers müssen wiederhergestellt werden. Marketo Engage Admin, um die Benutzermigration für diesen Benutzer über die Migrationskonsole erneut auszuführen.

### Nicht in Domäne {#not-in-domain}

**Grundursache**: Die Domain-Durchsetzung ist in der Admin Console aktiviert, aber die Domain der E-Mail-Adresse der Benutzerin oder des Benutzers ist keine der zulässigen Domains.

**Auflösungen**:

_Wenn der Benutzer nicht migriert werden muss_ - Marketo Engage-Administrator, um den Benutzer in der Migrationskonsole zu überspringen. Die Schaltfläche „Migration abgeschlossen“ wird angezeigt, wenn alle Benutzer durch Migration oder Überspringen berücksichtigt werden. Klicken Sie auf die Schaltfläche , um den Prozess der Benutzermigration abzuschließen.

_Wenn der Benutzer migriert werden muss_ - Die E-Mail-Adresse muss in Marketo Engage aktualisiert werden, damit sie der Domain Enforcement (DE)-Richtlinie entspricht. Alternativ kann der Systemadministrator die Domain entweder [in einen anderen ](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"}-Ordner (DE) verschieben oder [einen neuen Ordner erstellen](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"} der nicht unter der DE-Richtlinie steht. Marketo Engage Admin, um die Benutzermigration für diesen Benutzer über die Migrationskonsole erneut auszuführen.

### Fehler beim Erstellen {#create-failure}

**Grundursache** Dieser Fehler kann im Backend aus verschiedenen Gründen auftreten.

**Auflösungen**:

Senden Sie ein Ticket für den technischen Support mit relevanten Details für den [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

### Type2e-Benutzerfehler {#type2e-user-failure}

**Grundursache** Dieser Fehler kann im Backend aus verschiedenen Gründen auftreten.

**Auflösungen**:

Senden Sie ein Ticket für den technischen Support mit relevanten Details für den [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
