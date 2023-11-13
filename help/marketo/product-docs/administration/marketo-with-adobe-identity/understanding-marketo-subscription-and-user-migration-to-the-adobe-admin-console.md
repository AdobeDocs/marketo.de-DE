---
description: Grundlegendes zu Marketo-Abonnements und Benutzermigration zur Adobe Admin Console - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zu Marketo-Abonnements und Benutzermigration zur Adobe Admin Console
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: 094a11f9544e0dba75167de229d78e8ff50cf6e8
workflow-type: tm+mt
source-wordcount: '1189'
ht-degree: 0%

---

# Grundlegendes zu Marketo-Abonnements und Benutzermigration zur Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

Adobe verbessert die Verwaltung Ihrer Adobe Marketo Engage-Abonnements und -Benutzer und erhöht so die Produktivität für Sie und Ihr Unternehmen. Im Rahmen dieser Änderung migriert Adobe Ihre Marketo Engage-Abonnements und -Benutzer in die Adobe Admin Console. Dies ist eine erforderliche Migration und hat keine Auswirkungen auf Marketing-Workflows, Inhalte, Integrationen oder Assets.

Erfahren Sie, wie Sie mit der Adobe Admin Console Ihre Adobe-Berechtigungen in Ihrer gesamten Organisation verwalten können. [Administratorhandbuch für Unternehmen und Teams](https://helpx.adobe.com/de/enterprise/admin-guide.html){target="_blank"}.

## Was ändert sich? {#what-is-changing}

Im Rahmen der Migration wechseln Ihr Abonnement und Ihre Benutzerverwaltung von der Marketo-Anwendung zur Adobe Admin Console.

* **Systemadministratoren verwalten Abonnements in Adobe Admin Console**. Alle Adobe-Produkte werden in einer Konsole angezeigt.

* **Produktadministratoren verwalten Benutzer und deren Zugriff auf Adobe Admin Console**. Fügen Sie Benutzer für alle Adobe-Abonnements hinzu und entfernen Sie sie.

* **Benutzer melden sich mit Adobe Identity an**. Adobe migriert bestehende Benutzer in die Adobe Admin Console. Die Benutzer melden sich mit ihrer neuen Adobe-Identität bei ihren Marketo-Abonnements an - entweder mit einer Adobe ID- oder einer Adobe-Federated ID (SSO).

* **Es gibt keine Änderung an der Verwaltung aller anderen Funktionen** innerhalb der Marketo Engage-Anwendung selbst, einschließlich der Verwaltung von Funktionen, Benutzerrollen, Arbeitsbereichen, Funktionen und Verhaltensweisen.

## Timeline zur Migration Journey {#migration-journey-timeline}

Adobe migriert zuerst Ihre Marketo Engage-Abonnements in die Adobe Admin Console und migriert dann alle bestehenden Benutzer mit verifizierten E-Mail-Adressen. Wenn Sie Systemadministrator oder Marketo-Produktadministrator sind, erhalten Sie E-Mails, die Sie durch die Migration-Journey führen. Im Folgenden finden Sie eine Timeline zu den erwarteten Funktionen:

### Abonnement-Migration abgeschlossen {#subscription-migration-complete}

Systemadministratoren erhalten eine E-Mail, wenn die Abonnementmigration zu Adobe Admin Console abgeschlossen ist.

Systemadministratoren müssen möglicherweise einige erforderliche Schritte ausführen, bevor die Benutzermigration beginnt, um die Auswirkungen auf Marketo-Benutzer zu minimieren:

* Wenn sich Ihre Marketo-Benutzer derzeit mit SSO anmelden, müssen Sie SSO in der Adobe Admin Console einrichten, damit sich Ihre Benutzer weiterhin mit SSO anmelden können. Wenn Ihre Marketo-Benutzer derzeit keine SSO verwenden, Sie sie jedoch in Adobe Admin Console einrichten möchten, können Sie dies zu diesem Zeitpunkt im Journey der Migration tun.

* Wenn Sie bereits andere Adobe-Produkte in Ihrer Adobe Admin Console verwalten, kann Adobe Ihre Zustimmung einholen, um Benutzer automatisch in Ihre bestehende Konsole zu migrieren. Klicken Sie in der E-Mail auf die Schaltfläche &quot;Erste Schritte&quot;, um zur Einverständnisseite zu navigieren.

Die Benutzerverwaltung ändert sich derzeit nicht. Marketo-Administratoren verwalten Benutzer weiterhin im Marketo Admin-Bereich. Benutzer können sich bis zur vollständigen Benutzermigration weiterhin mit ihrer Marketo Identity anmelden.

### Benutzermigration planen {#schedule-user-migration}

Nachdem Ihr Systemadministrator die im vorherigen Abschnitt beschriebenen Voraussetzungen erfüllt hat, plant Adobe automatisch die Benutzermigration 30 Tage im Voraus und kommuniziert mit Marketo-Produktadministratoren, um die Benutzermigration zu verwalten.

Marketo-Produktadministratoren:

* Sie erhalten eine E-Mail mit dem geplanten Startdatum der Benutzermigration 30 Tage im Voraus.

* Erhalten Sie Zugriff auf die Marketo Migration Console im Marketo-Admin-Bereich, wo Sie die Möglichkeit haben, das Migrationsdatum eines Abonnements zu ändern.

>[!NOTE]
>
>Aufgrund der Komplexität der Migration sind Datumsänderungen auf maximal 30 Tage nach dem geplanten Datum beschränkt. E-Mail an senden `marketocares@marketo.com` , wenn Sie ein späteres Datum benötigen.

* Zeigen Sie in My Marketo ein Banner mit einem Countdown zum Startdatum der Benutzermigration an.

* Sie erhalten eine Erinnerungsmail am Tag vor dem Startdatum der Benutzermigration.

### Benutzer für den Migrationstag vorbereiten {#prepare-users-for-migration-day}

Als Marketo-Produktadministrator sollten Sie sicherstellen, dass alle Benutzer auf den Migrationstag vorbereitet sind.

* Überprüfen [E-Mail-Verifizierung](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"} -Status für alle Benutzer im Marketo-Admin-Bereich. Ermutigen Sie Benutzer, die ihre E-Mail-Adresse nicht überprüft haben, dies zu tun, und helfen Sie Benutzern, alle Probleme beim Abschluss des Verifizierungsprozesses zu lösen.

* Bereiten Sie alle Benutzer auf die bevorstehende Migration auf Adobe Identity vor.

>[!NOTE]
>
>Wenn Benutzer migrieren, erhalten sie eine E-Mail von der Adobe, in der sie über die Änderung der Anmeldung bei Marketo informiert werden. Die Benutzer werden eingeladen, erstmals eine Einladung zur Anmeldung mit Adobe Identity anzunehmen, indem sie sich entweder mit einer bestehenden Adobe ID anmelden oder eine neue mit derselben E-Mail-Adresse einrichten.

>[!IMPORTANT]
>
>Wenn ein Marketo Engage-Benutzer seine E-Mail-Adresse nicht verifiziert, wird er nicht in eine Adobe ID migriert und verliert nach Abschluss der Migration für das Abonnement den Zugriff auf das Marketo-Abonnement. Um wieder Zugriff zu erhalten, muss ein Marketo-Produktadministrator sie als neuen Benutzer hinzufügen.

### Was erwartet man am Migrationstag? {#what-to-expect-on-migration-day}

Alle Marketo-Abonnements mit einer US-Zeitzone werden ab Mitternacht, Pacific Standard Time, des Startdatums der Migration migriert. Die Benutzermigration für alle anderen Abonnements beginnt um Mitternacht der angegebenen Zeitzone des Abonnements.

**Adobe migriert Marketo-Administratoren zuerst automatisch.**. Wenn Marketo-Administratoren zu Adobe Identity migriert werden, erhalten sie in der Marketo-Anwendung die Adobe Product Admin-Rolle sowie alle anderen Rollen, die sie zuvor hatten.

**Wenn Ihr Marketo-Abonnement weniger als 75 Benutzer hat**, migriert Adobe automatisch den Rest Ihrer Benutzer. Dieser Workflow soll ein Höchstmaß an Automatisierung bieten, um den Verwaltungsaufwand für Adobe Marketo-Benutzer zu minimieren. Zum Ausführen der Migration ist keine Aktion Ihrerseits erforderlich.

**Wenn Ihr Marketo-Abonnement mehr als 75 Benutzer umfasst**, erhalten Produktadministratoren von Marketo Zugriff auf den Bereich &quot;Self-Service-Benutzermigration&quot;der Marketo Migration Console, der sich im Marketo-Admin-Bereich befindet. Für diejenigen, die während des Benutzermigrationsprozesses eine bessere Kontrolle benötigen, können Marketo-Produktadministratoren mit der Auswahl von Benutzern beginnen, die in Batches oder alle gleichzeitig migriert werden sollen. Sobald Benutzer ausgewählt sind, haben Administratoren die Möglichkeit, &quot;Jetzt migrieren&quot;oder &quot;Migration planen&quot;für einen späteren Zeitpunkt zu verwenden, wodurch Administratoren die ultimative Flexibilität und Kontrolle darüber erhalten, welche Benutzer wann migriert werden.

>[!NOTE]
>
>Während der Benutzermigration geht der Zugriff auf das Produkt nicht verloren. Wenn ein Benutzer während der Migration des Benutzers angemeldet ist, wird er abgemeldet und innerhalb von Minuten mit Adobe Identity aufgefordert, sich erneut anzumelden, nachdem die Migration abgeschlossen ist.

Wenn Benutzer migriert werden, erhalten sie eine E-Mail von der Adobe, in der sie über die Änderung der Anmeldung bei Marketo informiert werden. Die Benutzer werden eingeladen, erstmals eine Einladung zur Anmeldung mit Adobe Identity anzunehmen, indem sie sich entweder mit einer bestehenden Adobe ID anmelden oder eine neue Adobe ID mit derselben E-Mail-Adresse einrichten.

Weitere Informationen finden Sie unter [User Sign-in mit Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"} and [Adobe Identity Management FAQ](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

## Benutzermigration abgeschlossen {#user-migration-complete}

Adobe benachrichtigt alle Systemadministratoren und Produktadministratoren per E-Mail, sobald alle Administratoren und Benutzer migriert wurden. Derzeit melden sich alle Marketo-Benutzer für dieses Abonnement mit Adobe Identity bei Marketo an, und Produktadministratoren verwalten Benutzer nur auf Adobe Admin Console.

## Support erhalten {#get-support}

Zusätzliche Unterstützung bezüglich Ihrer An- oder Benutzermigration per E-Mail `marketocares@marketo.com`.
