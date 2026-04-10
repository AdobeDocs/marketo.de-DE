---
description: Häufig gestellte Fragen zur Adobe-Identität für Marketo Engage, einschließlich Migration, URLs, SSO, Produktadministrator vs. Marketo-Administrator und Zulassungsauflistung.
title: Häufig gestellte Fragen zu Adobe Identity Management
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: a2c5ee6591b688ca262fbab94f0b13bae481daff
workflow-type: tm+mt
source-wordcount: '1591'
ht-degree: 98%

---

# Häufig gestellte Fragen zu Adobe Identity Management {#adobe-identity-management-faq}

**Was ist Adobe Identity?**

Das Identitäts-Management-System von Adobe besteht aus drei Komponenten.

* [!DNL Adobe Identity Service]: Übernimmt die Authentifizierung und Validierung der Enbenutzenden, einschließlich Single-Sign-on (SSO) für Verbund und Laufzeit.

* Adobe Admin Console: Mit der Admin Console können Adobe-Berechtigungen für Ihr gesamtes Unternehmen zentral an einem Ort verwaltet werden. Hier werden Benutzerverwaltung, Cloud-Service, Desktop-Lizenzberechtigungen und Verbundkonfiguration abgewickelt und Sicherheitsfunktionen zum Schutz vor Datenverlust zur Verfügung gestellt.

* Adobe-API zur Benutzerverwaltung (UMAPI): Ermöglicht Unternehmen die Verwaltung von Unternehmensbenutzenden und Berechtigungen in der Adobe Admin Console auf API-Ebene.

**Wann werden bestehende Marketo Engage-Abonnements mit IMS integriert?**

Bestehende Marketo Engage-Abonnements werden derzeit bei jedem Verkaufsereignis zu Adobe IMS migriert, einschließlich Verlängerungen, Neuverträgen und/oder Vertragszusätzen. Migrationen außerhalb eines Verkaufsereignisses werden seit Oktober 2024 unterstützt.

**Bleiben die Marketo Engage-URLs nach der Migration unverändert?**

Nein. URLs werden nach der Migration im folgenden Format angezeigt: `https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` (die XXXs stellen die Munchkin-ID dar und @tenantID stammt aus Ihrer Adobe-Organisation).

**Müssen Vorbereitungen für die URL-Änderung getroffen werden?**

Ja. Nach der Migration wird Marketo Engage nicht mehr auf experience.adobe.com bereitgestellt, sondern auf Adobe Experience Cloud. Sie müssen mit Ihrem IT-Team zusammenarbeiten und alle [am Anfang dieses Artikels](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"} aufgelisteten Adobe-Domains auf die Zulassungsliste setzen, um eine Unterbrechung des Marketo Engage-Zugriffs zu verhindern.

Bisherige Links zu und Lesezeichen für Marketo Engage-Assets auf der Domain „engage-xx.marketo.com“ funktionieren _weiterhin_. Sie müssen sich jedoch zuerst bei der Marketo Engage-Instanz für die URL anmelden, zu der Sie navigieren. Um beispielsweise zu einem Lesezeichen für eine intelligente Kampagne in der Instanz mit der Munchkin-ID 123-ABC-456 zu navigieren, müssen Sie sich zuerst bei der Marketo Engage-Instanz mit der Munchkin-ID 123-ABC-456 anmelden.

Auch wenn dies nicht geplant ist, kann es sein, dass zukünftige Entwicklungsarbeiten diese Umleitungsfunktion beeinträchtigen. Um unerwartete Unterbrechungen zu vermeiden, wird empfohlen, Lesezeichen so schnell wie möglich zu aktualisieren.

**Funktioniert dies mit SSO?**

Ja. Die Integration mit Adobe IMS unterstützt Benutzende mit universeller ID und SSO. SSO wird jetzt von Adobe IMS gesteuert und auf Unternehmensebene in der Adobe Admin Console eingerichtet. Es gibt jedoch Unterschiede zwischen der IdP-initiierten Unterstützung für Marketo Engage und der SP-initiierten Unterstützung für Adobe ([Informationen dazu finden Sie hier](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}). Wenn Sie Informationen zu SSO-Unterschieden nach der Migration zu Admin Console benötigen, wenden Sie sich an die [Adobe-Kundenunterstützung](https://helpx.adobe.com/de/contact.html){target="_blank"}.

**Was ist der Unterschied zwischen den Rollen „Adobe-Produktadmin“ und „Marketo Engage-Admin“?**

* „Adobe-Produktadmin“ ist eine neue Rolle in der Marketo-Plattform.
* Die Rolle „Adobe-Produktadmin“ wird Benutzenden gewährt, die in der Adobe Admin Console als Produktadmin hinzugefügt werden.
* Die Rolle „Adobe-Produktadmin“ ist schreibgeschützt und kann nicht bearbeitet oder aus Marketo Engage gelöscht werden.
* Die Rolle „Adobe-Produktadmin“ hat dieselben Rechte und Berechtigungen wie standardmäßige Marketo-Admins.
* Die Rolle „Marketo Engage-Admin“ ist weiterhin eine Admin-Rolle und wird Benutzenden in Marketo Engage gewährt.
* Nur Benutzende mit der standardmäßigen Marketo-Admin-Rolle werden als Marketo-Produktadmin in der Admin Console zugewiesen.

**Gibt es Änderungen bei der Client-Unterstützung für die API zur Benutzerverwaltung?**

Ja. Personen, deren Onboarding in Adobe IMS abgeschlossen wurde, können nicht alle vorhandenen Marketo-APIs zur Benutzerverwaltung nutzen. Zum Einladen, Aktualisieren und Löschen von Benutzenden sollten die Adobe [IMS-APIs](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} verwendet werden. Für die Rollenverwaltung werden weiterhin die Marketo-APIs zur Benutzerverwaltung eingesetzt. Darüber hinaus gibt es keine weiteren Änderungen an der Client-Unterstützung der Marketo-REST-APIs.

**Wo gibt es Unterstützung nach der Integration mit IMS?**

* Vor der Benutzermigration: Wenden Sie sich mit Support-Fällen an die [Marketing-Nation-Community](https://nation.marketo.com/t5/support/ct-p/Support) oder senden Sie eine E-Mail an `marketocares@adobe.com`.

* Nach der Benutzermigration: Wenden Sie sich mit Support-Fällen an die [Marketing-Nation-Community](https://nation.marketo.com/t5/support/ct-p/Support?profile.language=de) oder senden Sie eine E-Mail an `marketocares@adobe.com`.

* Unterstützung nach Abschluss der Migration: Produkt-Support-Admins können Fälle über das Experience League Support-Portal einreichen.

Wenn Sie über Ultimate Success verfügen, haben Sie Zugriff auf den Admin Console Migration White Glove Service. Wenden Sie sich an das Adobe-Accountteam (Ihre Kundenbetreuung), um Unterstützung zu erhalten.

**Wenn ich Adobe Identity für den Zugriff auf andere Adobe-Anwendungen verwende, kann ich es auch für den Zugriff auf Marketo verwenden?**

Selbst wenn andere Adobe-Produkte in Ihrem Besitz sind, können Sie erst dann mit Adobe Identity auf Marketo zugreifen, wenn das Abonnement zu IMS migriert wurde.

**Werden Marketo-Benutzerrollen (innerhalb von Arbeitsbereichen) in der Adobe Admin Console verwaltet?**

Nein. Benutzerrollen (innerhalb von Arbeitsbereichen) werden in Marketo Engage verwaltet.

**Ich bin Marketo-Admin in einem integrierten IMS-Abonnement und habe keinen Zugriff auf die Admin Console. Wie erhalte ich Zugriff?**

Jedes Adobe-System bzw. alle Produktadmins mit Zugriff auf die Admin Console Ihres Unternehmens können Ihnen Zugriff gewähren. Wenn Sie sich nicht sicher sind, wer in Ihrem Unternehmen über Adminrechte in der Konsole verfügt, wenden Sie sich an die [Adobe-Kundenunterstützung](https://helpx.adobe.com/de/contact.html){target="_blank"}.

**Wie fügen Admins Benutzende zu Marketo [!DNL Sales Connect] hinzu?**

Obwohl eine Produktkarte für [!DNL Sales Connect] in der Admin Console vorgesehen ist, sollte die Admin Console nicht zum Hinzufügen/Verwalten von Benutzenden verwendet werden. Admins können den folgenden Link verwenden, um Benutzende über Marketo [!DNL Sales Connect] zu verwalten: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}

**Wo erhalte ich weitere Informationen über die Adobe Admin Console?**

[https://helpx.adobe.com/de/enterprise/admin-guide.html](https://helpx.adobe.com/de/enterprise/admin-guide.html){target="_blank"}.

**Nehme ich Benutzerkontoänderungen für mein Konto immer noch im Abschnitt „Administrator“ in Marketo vor?**

Nein, Sie müssen zu [account.adobe.com](https://account.adobe.com){target="_blank"} navigieren.

**Wie funktioniert dies mit der universellen ID von Marketo?**

Personen, deren Onboarding in Adobe Identity abgeschlossen wurde, können über Abonnementwechsel im Produkt nahtlos auf alle in IMS aktivierten Abonnements zugreifen.

**Funktioniert dies mit SSO?**

Ja. Die Marketo-Integration mit Adobe IMS unterstützt Benutzende mit universeller ID und SSO. SSO wird jetzt von Adobe IMS gesteuert und auf Unternehmensebene in der Adobe Admin Console eingerichtet. [Weitere Informationen finden Sie hier](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

**Mein Onboarding in Adobe Identity ist bereits abgeschlossen und ich möchte nun SSO implementieren. Was muss ich tun?**

Wenn Sie Single Sign-on implementieren möchten und das Onboarding Ihres Abonnements in Adobe Identity ohne Implementierung von SSO in der Adobe-Organisation abgeschlossen wurde, senden Sie ein Ticket an den [Marketo-Support](https://nation.marketo.com/){target="_blank"} und geben Sie als Thema „Marketo in der Admin Console, Implementierung von SSO“ an.

**Wie funktioniert die Geräteautorisierung?**

Adobe IMS unterstützt derzeit keine Funktion, die der Geräteautorisierung von Marketo ähnelt.

**Ist es weiterhin möglich, die Funktion „Anmeldung im Dialogfenster Benutzer einladen“ zu verwenden, damit die Anmeldung einer Benutzerin bzw. eines Benutzers basierend auf der E-Mail-Adresse eindeutig ist?**

Nein. Der Workflow zum Einladen von Benutzenden ist nicht mehr aktiv, wenn ein Abonnement in IMS aktiviert wurde. Die Funktion ist also nicht mehr gültig. Adobe Identity erfordert, dass die Identität einer Benutzerin bzw. eines Benutzers von der E-Mail-Adresse gesteuert wird.

**Gibt es für Adobe IMS die Möglichkeit, Adobe ID, Enterprise ID oder Federated ID zu verwenden?**

Ja, Sie bestimmen den Identitätstyp, den Ihre Organisation unterstützen soll. Weitere Informationen finden Sie hier: [Überblick über Identitäten](https://helpx.adobe.com/de/enterprise/using/identity.html) und hier: [Einrichten von Identitäten](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

**Welche Produktkarten werden in der Adobe Admin Console unterstützt?**

Die unterstützten Produktkarten sind: Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect und Marketo Sales Insight-Aktionen.

**Was passiert, wenn meine Benutzeranmeldung bei der Migration zu Adobe Identity nicht mit meiner E-Mail-Adresse übereinstimmt?**

Aktuelle Marketo Engage-Benutzende mit Anmeldungen, die sich von ihrer E-Mail-Adresse unterscheiden, melden sich nach der Migration zu Adobe Identity nicht mehr mit diesen Anmeldedaten an. Authentifizierungen mit Adobe Identity geschehen immer über die E-Mail-Adresse einer Benutzerin bzw. eines Benutzers. Sie können eine E-Mail-Adresse für Adobe Identity unter [account.adobe.com](https://account.adobe.com){target="_blank"} aktualisieren.

**Was passiert nach der Migration zu Adobe Identity, wenn mein Abonnement IP-Einschränkungseinstellungen verwendet?**

Ihre aktuellen IP-Einschränkungen bleiben bis zum 1. Quartal 2026 aktiv (dies gilt für Abonnements, für die sie vor der Migration aktiviert waren). Diese Einschränkungen gelten auch für Adobe ID-Benutzende. Ihre Zugriffssteuerungen funktionieren also weiterhin wie erwartet.

Ab dem 1. Quartal 2026 werden die alten IP-Einschränkungen eingestellt. Ab diesem Zeitpunkt wird der IP-basierte Zugriff ausschließlich in der Adobe Admin Console (AAC) verwaltet. Um den sicheren Zugriff aufrechtzuerhalten, müssen Sie IP-Einschränkungen in AAC konfigurieren. Weitere Informationen finden Sie in diesem [Blogpost von Marketing Nation](https://nation.marketo.com/t5/product-blogs/updated-important-update-ip-restrictions-feature-transition/ba-p/358420){target="_blank"}.

**Was passiert nach der Migration zu Adobe Identity mit Benutzenden, die die Option einer Umgehung von Single Sign-on aktiviert haben?**

Die Adobe Admin Console enthält ein standardmäßiges Unternehmens-ID-Verzeichnis. Benutzende, die nicht zu den Domains gehören, die in Federated ID-Verzeichnissen in einer Adobe-Organisation beansprucht werden, werden diesem Verzeichnis mit dem Identitätstyp „Adobe ID“ zugewiesen. Diese Benutzenden können ohne Single Sign-on (SSO) auf Marketo Engage zugreifen und das Lizenzeigentum verbleibt beim Unternehmen, nicht bei den Einzelpersonen.

**Ich verfüge über mehrere Abonnements, aber nicht für alle ist Single Sign-on aktiviert. Was passiert nach der Migration zu Adobe Identity?**

Wenn das Onboarding von Abonnements in Adobe Identity abgeschlossen ist, wird Single Sign-on (SSO) auf Adobe-Organisationsebene eingerichtet. Dies bedeutet, dass SSO für alle Produktinstanzen in der Adobe-Organisation gilt. Wenn SSO eingerichtet ist, gilt dies für alle Marketo-Instanzen in dieser Adobe-Organisation. Zuvor wurde diese Einstellung von Marketo auf Instanzebene unterstützt. Dies wird vom Identitäts-Management-System von Adobe nicht unterstützt.

**Sind nach der Migration zu Adobe Identity Änderungen an CNAMEs, SPF oder DKIM erforderlich, die derzeit für Marketo Engage verwendet werden?**

Nein, es gibt keine Auswirkungen auf diese Konfigurationen.

**Wie kann ich verhindern, dass ein Timeout für Sitzungen ausgelöst wird?**

Unter [Erweiterte Einstellungen](https://helpx.adobe.com/de/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"} können Sie die gewünschte maximale Sitzungsdauer anpassen (Systemadmin-Berechtigungen erforderlich). Es wird empfohlen, diese Einstellung nach der Produktmigration, jedoch vor der Benutzermigration festzulegen.

**Ich muss jetzt zu Experience Cloud navigieren, um auf Marketo Engage zuzugreifen. Gibt es eine Möglichkeit, diesen Ablauf zu optimieren?**

Ja. Sie können ein Browser-Lesezeichen für den Link erstellen, der nach Klicken auf die Schaltfläche **Starten** auf der Startseite der Marketo Engage-Instanz aufgerufen wird, um diese Seite in Zukunft zu umgehen.

![](assets/faq-1.png)
