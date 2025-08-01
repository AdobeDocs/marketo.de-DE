---
description: Handbuch zur Fehlerbehebung bei der Adobe IMS-Benutzermigration - Marketo-Dokumente - Produktdokumentation
title: Handbuch zur Fehlerbehebung bei der Adobe IMS-Benutzermigration
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 1%

---

# Handbuch zur Fehlerbehebung bei der Adobe IMS-Benutzermigration {#adobe-ims-user-migration-troubleshooting-guide}

Während der IMS-Benutzermigration wird für jeden migrierten Marketo Engage-Benutzer ein Adobe-Benutzer erstellt (es sei denn, er existiert bereits mit derselben E-Mail-Adresse). Manchmal wird er nicht erstellt, was auf den Datensatz des Benutzers im Active Directory oder Probleme mit der E-Mail-Adresse zurückgeführt werden kann.

Dieser Artikel für Benutzer, die Selbstmigrationen durchführen, listet jede Fehlermeldung auf, die Sie möglicherweise im Feld Status der Selbstmigrationskonsole sehen.

>[!NOTE]
>
>Die Ordner-/Domain-bezogenen Fehler können von einer anderen Organisation/Admin Console ausgelöst werden, in der eine Verzeichnisvertrauensstellung eingerichtet ist oder die Domain angefordert wurde.

## Fehlermeldungen {#error-messages}

Bestimmen Sie zunächst, ob der Benutzer migriert werden muss oder nicht, da dies Auswirkungen auf die zu befolgenden Auflösungsschritte hat.

Verwenden Sie den Abschnitt „Auf dieser Seite“ rechts, um direkt zu einem bestimmten Fehler zu springen.

### Ungültiges Gmail-Zeichen {#gmail-invalid-character}

**Grundursache**: Gemäß der Adobe-Sicherheitsrichtlinie sind die Zeichen `.` und `+` in einer Gmail-E-Mail-Adresse nicht zulässig. Beide Zeichen sind in Nicht-Gmail-E-Mail-Adressen zulässig.

**Auflösungen**:

_Wenn der Benutzer migriert werden muss_ - Die E-Mail-Adresse muss in Marketo Engage aktualisiert werden, um die Adobe-Sicherheitsrichtlinie zu erfüllen, und erneut überprüft werden. Marketo Admin, um die Benutzermigration für diesen Benutzer über die Migrationskonsole erneut auszuführen.

_Wenn der Benutzer nicht **&#x200B;**&#x200B;migriert werden muss_ - Marketo Engage-Administrator, um den Benutzer in der Migrationskonsole zu überspringen. Die Schaltfläche „Migration abgeschlossen“ wird angezeigt, wenn alle Benutzer durch Migration oder Überspringen berücksichtigt werden. Klicken Sie auf die Schaltfläche , um den Prozess der Benutzermigration abzuschließen.

### Benutzer nicht im Verzeichnis {#user-not-in-directory}

**Grundursache**: Der Benutzer existiert nicht in Active Directory (AD). Für alle Organisationen mit SSO, für die die Anzeigensynchronisierung aktiviert ist, ist die Benutzererstellung nur über den Identitätsanbieter (IdP) zulässig. Daher konnte der Benutzer während der Benutzermigration nicht über Admin Console hinzugefügt werden.

**Auflösungen**:

_Wenn der Benutzer migriert werden muss_ - Der Benutzer muss von einem Systemadministrator mit den entsprechenden Berechtigungen zum Active Directory hinzugefügt werden. Marketo Engage Admin, um die Benutzermigration für diesen Benutzer über die Migrationskonsole erneut auszuführen.

_Wenn der Benutzer nicht **&#x200B;**&#x200B;migriert werden muss_ - Marketo Engage-Administrator, um den Benutzer in der Migrationskonsole zu überspringen. Die Schaltfläche „Migration abgeschlossen“ wird angezeigt, wenn alle Benutzer durch Migration oder Überspringen berücksichtigt werden. Klicken Sie auf die Schaltfläche , um den Prozess der Benutzermigration abzuschließen.

### Inaktiver Benutzer {#inactive-user}

**Grundursache**: Die AD-Synchronisierung ist aktiviert und das Federated-Konto des Benutzers existiert, jedoch im Status „Inaktiv/Deaktiviert“.

**Auflösungen**:

_Wenn der Benutzer migriert werden muss_ - Der Status des Benutzers und seine Berechtigungen müssen von einem Systemadministrator wiederhergestellt werden. Marketo Engage Admin, um die Benutzermigration für diesen Benutzer über die Migrationskonsole erneut auszuführen.

_Wenn der Benutzer nicht **&#x200B;**&#x200B;migriert werden muss_ - Marketo Engage-Administrator, um den Benutzer in der Migrationskonsole zu überspringen. Die Schaltfläche „Migration abgeschlossen“ wird angezeigt, wenn alle Benutzer durch Migration oder Überspringen berücksichtigt werden. Klicken Sie auf die Schaltfläche , um den Prozess der Benutzermigration abzuschließen.

### Ungültige Domain {#invalid-domain}

**Ursache**: Die Domain-Durchsetzung ist in der Admin Console aktiviert. Die Domain der E-Mail-Adresse des Benutzers ist jedoch keine der zulässigen Domains oder die Domain wurde in einer anderen Organisation/Admin Console beansprucht.

**Auflösungen**:

_Wenn der Benutzer migriert werden muss_ (und die Domain-Durchsetzung in der migrierenden Organisation aktiviert ist) - Die E-Mail-Adresse muss in Marketo Engage aktualisiert werden, um die Domain Enforcement (DE)-Richtlinie zu erfüllen. Alternativ kann der Systemadministrator die Domain entweder [in einen anderen ](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"}-Ordner (DE) verschieben oder [einen neuen Ordner erstellen](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"} der nicht unter der DE-Richtlinie steht. Marketo Engage Admin, um die Benutzermigration für diesen Benutzer über die Migrationskonsole erneut auszuführen.

_Wenn der Benutzer migriert werden muss_ (und die Domain-Durchsetzung in einer anderen Organisation aktiviert ist) - Ein Systemadministrator der Organisation, in der die Domain beansprucht wurde, muss die E-Mail-Adresse des Benutzers zur Ausnahmeliste hinzufügen. Marketo Engage Admin, um die Benutzermigration für diesen Benutzer über die Migrationskonsole erneut auszuführen.

_Wenn der Benutzer nicht **&#x200B;**&#x200B;migriert werden muss_ - Marketo Engage-Administrator, um den Benutzer in der Migrationskonsole zu überspringen. Die Schaltfläche „Migration abgeschlossen“ wird angezeigt, wenn alle Benutzer durch Migration oder Überspringen berücksichtigt werden. Klicken Sie auf die Schaltfläche , um den Prozess der Benutzermigration abzuschließen.

### Type2e-Fehler {#type2e-failure}

**Grundursache**: Die Erstellung eines zusammengeführten Benutzerkontos (für Single Sign-On) ist während der Benutzermigration fehlgeschlagen, da für dieselbe E-Mail-Adresse wie ein einzelner Benutzer bereits eine Adobe ID vorhanden ist.

**Auflösungen**:

1. Entfernen Sie den einzelnen Benutzer aus der Adobe-Organisation. Hinweis: Der Benutzer verliert den Zugriff auf alle Produkte und muss später erneut berechtigt werden.
1. Führen Sie die Benutzermigration erneut aus, damit ein zusammengeführtes Benutzerkonto für diesen Benutzer erstellt wird.
1. Fügen Sie die Benutzenden den Produkten hinzu, auf die sie zuvor Zugriff hatten.

### Benutzererstellung fehlgeschlagen {#user-creation-failed}

[Siehe unten](#failed)

### Marketo-Berechtigung gescheitert {#marketo-entitlement-failed}

[Siehe unten](#failed)

### Pendo-Migration fehlgeschlagen {#pendo-migration-failed}

[Siehe unten](#failed)

### Migration der Benutzerdaten fehlgeschlagen {#user-data-migration-failed}

[Siehe unten](#failed)

### Synchronisierung der Produktdaten fehlgeschlagen {#product-data-sync-failed}

[Siehe unten](#failed)

### Adobe-Berechtigung fehlgeschlagen {#adobe-entitlement-failed}

[Siehe unten](#failed)

### Abmelden des Benutzers fehlgeschlagen {#user-sign-out-failed}

[Siehe unten](#failed)

### Adobe ID-Erstellung fehlgeschlagen {#adobe-id-creation-failed}

[Siehe unten](#failed)

### Fehlgeschlagen {#failed}

**Grundursache**: Diese Fehler können im Backend aus verschiedenen Gründen auftreten.

**Auflösungen**:

Senden Sie ein Ticket für den technischen Support mit relevanten Details für den [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
