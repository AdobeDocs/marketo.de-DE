---
description: Was ändert sich, wenn Abonnements und Benutzende zur Adobe Admin Console migrieren, einschließlich Systemadministrator- und Produktadministratorrollen, Anmeldung mit Adobe-Identität, URLs und des Migrationszeitplans.
title: Grundlegendes zur Marketo-Abonnement- und -Benutzermigration zur Adobe Admin Console
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '1584'
ht-degree: 98%

---

# Grundlegendes zur Marketo-Abonnement- und -Benutzermigration zur Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

Adobe verbessert die Verwaltung Ihrer Adobe Marketo Engage-Abonnements und -Benutzenden und steigert Ihre Produktivität sowie die Produktivität Ihres Unternehmens. Im Rahmen dieser Änderung migriert Adobe Ihre Marketo Engage-Abonnements und -Benutzenden zur Adobe Admin Console. Dies ist eine erforderliche Migration. Sie hat keine Auswirkungen auf Marketing-Workflows, Inhalte, Integrationen oder Assets.

>[!TIP]
>
>Im [dministratorhandbuch für Unternehmen und Teams](https://helpx.adobe.com/de/enterprise/admin-guide.html){target="_blank"} erfahren Sie, wie Sie mit der Adobe Admin Console Adobe-Berechtigungen für Ihr gesamtes Unternehmen verwalten.

## Was ändert sich? {#what-is-changing}

Im Rahmen der Migration werden Ihr Abonnement und die Benutzerverwaltung von Marketo zur Adobe Admin Console verschoben.

* **Systemadmins verwalten Abonnements in der Adobe Admin Console**. Alle Adobe-Produkte werden in einer Konsole angezeigt.

* **Produktadmins verwalten Benutzende und deren Zugriff in der Adobe Admin Console**. Fügen Sie Benutzende für alle Adobe-Abonnements hinzu und entfernen Sie sie. Die Adobe Admin Console unterstützt einen Ablauf des benutzerbasierten Zugriffs nicht. Benutzende mit nach der Migration ablaufendem Marketo Engage-Zugriff werden dennoch migriert und erhalten nicht ablaufenden Zugriff. Nach der Migration müssen sie am (oder vor dem) gewünschten Ablaufdatum manuell entfernt werden.

* **Benutzende melden sich mit Adobe Identity an**. Adobe migriert bestehende Benutzende zur Adobe Admin Console. Benutzende melden sich nun mit Adobe Identity (entweder mit einer Adobe ID oder Adobe Federated ID (SSO)) bei ihren Marketo-Abonnements an.

* **URLs sehen nach der Migration anders aus**. Marketo Engage wird nicht mehr auf experience.adobe.com bereitgestellt, sondern auf Adobe Experience Cloud. Die URLs weisen das folgende Format auf: `https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` (die XXXs stellen die Munchkin-ID dar und @tenantID stammt aus Ihrer Adobe-Organisation). Sie müssen mit Ihrem IT-Team zusammenarbeiten und alle [am Anfang dieses Artikels](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"} aufgelisteten Adobe-Domains auf die Zulassungsliste setzen, um eine Unterbrechung des Zugriffs auf Marketo Engage zu verhindern.

Die ID-Nummern Ihrer Assets bleiben gleich. Außerdem funktionieren bisherige Links zu und Lesezeichen für Marketo Engage-Assets auf der Domain „engage-xx.marketo.com“ _weiterhin_. Sie müssen sich jedoch zuerst bei der Marketo Engage-Instanz für die URL anmelden, zu der Sie navigieren. Um beispielsweise zu einem Lesezeichen für eine intelligente Kampagne in der Instanz mit der Munchkin-ID 123-ABC-456 zu navigieren, müssen Sie sich zuerst bei der Marketo Engage-Instanz mit der Munchkin-ID 123-ABC-456 anmelden.

Auch wenn dies nicht geplant ist, kann es sein, dass zukünftige Entwicklungsarbeiten diese Umleitungsfunktion beeinträchtigen. Um unerwartete Unterbrechungen zu vermeiden, wird empfohlen, Lesezeichen so schnell wie möglich zu aktualisieren.

## Was ändert sich nicht? {#what-is-not-changing}

* **Die Verwaltung aller anderen Funktionen in Marketo Engage selbst ändert sich nicht**. Dies schließt die Verwaltung von Funktionen, Benutzerrollen, Arbeitsbereichen, Funktionalitäten und Verhaltensweisen ein. Die lokale Benutzerverwaltung (nur API) ist weiterhin auf der Registerkarte _Benutzer und Rollen_ im Admin-Bereich auf Marketo verfügbar.

## Migrations-Timeline {#migration-journey-timeline}

Adobe migriert zuerst Ihre Marketo Engage-Abonnements zur Adobe Admin Console und dann alle bestehenden Benutzenden mit verifizierten E-Mail-Adressen. Wenn Sie Systemadmin oder Marketo-Produktadmin sind, erhalten Sie E-Mails, die Sie durch die Migration führen. Hier ist eine Timeline dessen, was Sie erwarten können:

![](assets/understanding-marketo-subscription-and-user-migration-1.png){width="800" zoomable="yes"}

### Abschluss der Abonnementmigration {#subscription-migration-complete}

Systemadmins erhalten eine E-Mail, wenn die Abonnementmigration zur Adobe Admin Console abgeschlossen ist.

Systemadmins müssen vor Beginn der Benutzermigration möglicherweise einige erforderliche Schritte ausführen, um die Auswirkungen auf Marketo-Benutzende zu minimieren:

* Wenn sich Ihre Marketo-Benutzenden derzeit mit SSO anmelden, müssen Sie SSO in der Adobe Admin Console einrichten, damit sich Ihre Benutzenden weiterhin mit SSO anmelden können. Wenn Ihre Marketo-Benutzenden derzeit nicht SSO verwenden, Sie es jedoch in der Adobe Admin Console einrichten möchten, können Sie dies zu diesem Zeitpunkt in der Migration tun.

* Wenn Sie bereits andere Adobe-Produkte in Ihrer Adobe Admin Console verwalten, kann Adobe Ihr Einverständnis einholen, Benutzende automatisch in Ihre bestehende Konsole zu migrieren. Klicken Sie in der E-Mail auf die Schaltfläche „Erste Schritte“, um zur Einverständnisseite zu navigieren.

An der Benutzerverwaltung ändert sich derzeit nichts. Obwohl Marketo-Produkte in der Admin Console angezeigt werden, verwalten Marketo-Admins weiterhin Benutzende im Bereich „Administrator“ von Marketo. Benutzende melden sich weiterhin mit ihrer Marketo-Identität an, bis die Benutzermigration abgeschlossen ist. Marketo-Produkte können erst dann in der Admin Console verwaltet werden, wenn die Benutzermigration beginnt. Das betrifft auch die Dynamic Chat-Instanz, die mit dem Abonnement verknüpft ist.

>[!NOTE]
>
>Wenn Sie SSO derzeit nicht verwenden, aber über dessen Implementierung nachdenken, empfehlen wir, dies vor der Benutzermigration zu tun. Wenn Sie Single Sign-on implementieren möchten und das Onboarding Ihres Abonnements in Adobe Identity ohne Implementierung von SSO in der Adobe-Organisation abgeschlossen wurde, senden Sie ein Ticket an den [Marketo-Support](https://nation.marketo.com/){target="_blank"} und geben Sie als Thema „Marketo in der Admin Console, Implementierung von SSO“ an.

### Planen der Benutzermigration {#schedule-user-migration}

Nachdem Ihre bzw. Ihr Systemadmin die im vorherigen Abschnitt beschriebenen Voraussetzungen erfüllt hat, plant Adobe Ihre Benutzermigration automatisch 30 Tage im Voraus und kommuniziert mit Marketo-Produktadmins zur Verwaltung der Benutzermigration.

Marketo-Produktadmins:

* Erhalten eine E-Mail mit dem geplanten Startdatum der Benutzermigration 30 Tage im Voraus.

* Erhalten Zugriff auf die Marketo-Migrationskonsole im Bereich „Administrator“ von Marketo, wo sie die Möglichkeit haben, das Migrationsdatum eines Abonnements zu ändern.

>[!NOTE]
>
>Aufgrund der Komplexität der Migration sind Datumsänderungen auf maximal 30 Tage nach dem geplanten Datum beschränkt. Senden Sie eine E-Mail an `marketocares@marketo.com`, wenn Sie eine Änderung auf ein späteres Datum wünschen.

* Sehen in „Mein Marketo“ ein Banner mit einem Countdown bis zum Startdatum der Benutzermigration.

* Erhalten eine Erinnerungs-E-Mail am Tag vor dem Startdatum der Benutzermigration.

### Vorbereiten der Benutzenden auf den Migrationstag {#prepare-users-for-migration-day}

Als Marketo-Produktadmin sollten Sie sicherstellen, dass alle Benutzenden auf den Migrationstag vorbereitet sind.

* Überprüfen Sie den Status der [E-Mail-Überprüfung](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"} für alle Benutzenden im Bereich „Administrator“ von Marketo. Fordern Sie Benutzende dazu auf, ihre E-Mail-Adresse zu verifizieren, wenn sie dies noch nicht getan haben. Unterstützen Sie Benutzende außerdem bei der Bewältigung aller Herausforderungen beim Abschluss des Überprüfungsprozesses.

* Durchsuchen Sie Ihren E-Mail-Posteingang nach Benachrichtigungen zu „gesperrten“ Benutzenden. Weisen Sie gesperrte Benutzende darauf hin, ihr Passwort zurückzusetzen, um ihren Zugriff auf Marketo Engage vor dem Migrationstag wiederherzustellen.

* Bereiten Sie alle Benutzenden auf die bevorstehende Migration zu Adobe Identity vor.

>[!IMPORTANT]
>
>Marketo Engage-Benutzende, die ihre E-Mail-Adresse nicht verifiziert haben oder zum Zeitpunkt der Benutzermigration gesperrt sind, werden nicht zu einer Adobe ID migriert und verlieren nach Abschluss der Abonnementmigration den Zugriff auf das Marketo-Abonnement. Um den Zugriff wiederzuerlangen, muss eine bzw. ein Marketo-Produktadmin sie als neue Benutzende hinzufügen.

### Was am Migrationstag zu erwarten ist {#what-to-expect-on-migration-day}

Alle Marketo-Abonnements mit einer Zeitzone in den USA werden ab Mitternacht (Pacific Standard Time) des Startdatums der Migration migriert. Die Benutzermigration für alle anderen Abonnements beginnt um Mitternacht der für das Abonnement festgelegten Zeitzone.

**Adobe migriert zuerst automatisch Marketo-Admins (mit einer standardmäßigen Admin-Rolle)**. Wenn Marketo-Admins mit der Rolle „Admin Console-Produktadmin“ zu Adobe Identity migriert werden, wird ihnen innerhalb von Marketo die Rolle „Adobe-Produktadmin“ zugewiesen, zusammen mit allen anderen Rollen, die sie zuvor hatten.

**Wenn Ihr Marketo-Abonnement in Marketo und/oder Ihrer Adobe-Organisation kein SSO verwendet**, migriert Adobe die restlichen Benutzenden automatisch. Dieser Workflow soll ein Höchstmaß an Automatisierung bieten und so den Mehraufwand für Adobe Marketo-Benutzende minimieren. Es ist keine Handlung Ihrerseits erforderlich, um die Migration auszuführen.

**Wenn Ihr Marketo-Abonnement in Marketo und/oder Ihrer Adobe-Organisation SSO verwendet**, erhalten Marketo-Admins Zugriff auf den Self-Service-Bereich für die Benutzermigration in der Marketo-Migrationskonsole im Bereich „Administrator“ von Marketo. Zur besseren Steuerung des Benutzermigrationsprozesses können Marketo-Admins sich entscheiden, Benutzende entweder in Batches oder alle gleichzeitig zu migrieren. Nach Auswahl der Benutzenden stehen Admins die Optionen „Jetzt migrieren“ oder „Migration planen“ (für einen späteren Zeitpunkt) zur Verfügung. Dadurch sind Admins sehr flexibel und haben Kontrolle darüber, welche Benutzenden migriert werden und wann dies geschieht.

>[!NOTE]
>
>Bei der Migration der Benutzenden bleibt der Produktzugriff bestehen. Wenn Benutzende zum Zeitpunkt ihrer Benutzermigration angemeldet sind, werden sie abgemeldet und wenige Minuten nach Abschluss der Migration dazu aufgefordert, sich mit Adobe Identity erneut anzumelden. Benutzende müssen die Einladung annehmen, indem sie auf den Link in der Berechtigungs-E-Mail klicken, die nach erfolgreichem Abschluss der Benutzermigration versendet wird.

Wenn Benutzende migriert werden, erhalten sie eine E-Mail von Adobe, in der sie über die Änderungen der Anmeldemethode bei Marketo informiert werden. Benutzende **müssen** eine Einladung annehmen, um sich das erste Mal mit Adobe Identity anmelden zu können. Sie können sich entweder mit einer vorhandenen Adobe ID anmelden oder eine neue Adobe ID mit derselben E-Mail-Adresse einrichten.

Weitere Informationen finden Sie unter [Migrieren zu Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}, [Benutzeranmeldung mit Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"} und [Häufig gestellte Fragen zu Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

## Abschluss der Benutzermigration {#user-migration-complete}

Adobe benachrichtigt alle Systemadmins und Produktadmins per E-Mail, sobald alle Admins und Benutzenden migriert wurden. Derzeit melden sich alle Marketo-Benutzenden für dieses Abonnement mithilfe von Adobe Identity bei Marketo an und Produktadmins verwalten Benutzende nur über die Adobe Admin Console.

## Erhalten von Unterstützung {#get-support}

Wenn Sie zusätzliche Unterstützung bei der Abonnement- oder Benutzermigration benötigen, senden Sie eine E-Mail an `marketocares@marketo.com`.

>[!MORELIKETHIS]
>
>* [Migrieren zu Adobe Identity – Überblick](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}
>* [Benutzeranmeldung mit Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}
>* [Häufig gestellte Fragen zu Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}
>* [Migrieren zu Adobe Identity Management – Tutorial](https://experienceleague.adobe.com/de/docs/marketo-learn/tutorials/fundamentals/migrating-to-adobe-identity-management){target="_blank"}
