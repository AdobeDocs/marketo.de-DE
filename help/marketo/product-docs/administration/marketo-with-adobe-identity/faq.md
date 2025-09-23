---
description: Häufig gestellte Fragen zu Adobe Identity Management - Marketo-Dokumente - Produktdokumentation
title: Häufig gestellte Fragen zu Adobe Identity Management
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1645'
ht-degree: 0%

---

# Häufig gestellte Fragen zu Adobe Identity Management {#adobe-identity-management-faq}

**Was ist Adobe Identity?**

Das Adobe Identity Management-System besteht aus drei Komponenten.

* [!DNL Adobe Identity Service]: Übernimmt die Authentifizierung und Validierung des Endbenutzers, einschließlich Federation und Runtime Single-Sign-On (SSO).

* Adobe Admin Console: Die Admin Console bietet einen zentralen Speicherort für die Verwaltung von Adobe-Berechtigungen in Ihrem gesamten Unternehmen. Es übernimmt die Benutzerverwaltung, den Cloud-Service, die Desktop-Lizenzberechtigungen und die Verbundkonfiguration und bietet Sicherheitsfunktionen zum Schutz vor Datenverlust.

* Adobe User Management-API (UMAPI) : Ermöglicht Unternehmen die Verwaltung von Unternehmensbenutzern und Berechtigungen in der Adobe Admin Console auf API-Ebene.

**Wann werden bestehende Marketo Engage-Abonnements in IMS integriert?**

Bestehende Marketo Engage-Abonnements werden derzeit bei jedem Verkaufsereignis, einschließlich Verlängerungen, Neuverträgen und/oder Nachträgen, in das Adobe IMS migriert. Migrationen außerhalb eines Verkaufsereignisses werden ab Oktober 2024 unterstützt.

**Werden die Marketo Engage-URLs nach der Migration unverändert bleiben?**

Nein. URLs werden nach der Migration im folgenden Format angezeigt: `https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` (die XXXs stellen die Munchkin-ID dar und @tenantID stammt aus Ihrer Adobe-Organisation).

**Müssen wir etwas tun, um uns auf die URL-Änderung vorzubereiten?**

Ja. Nach der Migration wird Marketo Engage von experience.adobe.com nach Adobe Experience Cloud bereitgestellt. Auf die Zulassungsliste setzen Sie müssen mit Ihrem IT-Team zusammenarbeiten, um alle aufgelisteten Adobe-Domains [am Anfang dieses Artikels) ](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"}, um eine Unterbrechung des Marketo Engage-Zugriffs zu verhindern.

Bisherige Links und Lesezeichen zu Marketo Engage-Assets auf der Domain engage-xx.marketo.com _funktionieren_. Sie müssen sich jedoch zuerst bei der Marketo Engage-Instanz für die URL anmelden, zu der Sie navigieren. Um beispielsweise zu einem Lesezeichen für eine Smart-Campaign-Instanz mit der Munchkin-ID 123-ABC-456 zu navigieren, müssen Sie sich zuerst mit der Munchkin-ID 123-ABC-456 bei der Marketo Engage-Instanz anmelden.

Auch wenn dies nicht geplant ist, können zukünftige Entwicklungsarbeiten diese Umleitungsfunktion beschädigen. Um unerwartete Unterbrechungen zu vermeiden, wird empfohlen, Lesezeichen so schnell wie möglich zu aktualisieren.

**Funktioniert dies mit SSO?**

Ja. Die Integration mit Adobe IMS unterstützt Benutzer mit universeller ID und SSO. SSO wird jetzt von Adobe IMS gesteuert und auf Unternehmensebene in der Adobe Admin Console eingerichtet. Es gibt jedoch Unterschiede zwischen der ID-initiierten Unterstützung für Marketo Engage und der SP-initiierten Unterstützung für Adobe ([ Informationen finden Sie hier](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}). Wenn Sie Hilfe zu SSO-Unterschieden nach der Migration zu Admin Console benötigen, wenden Sie sich an die [Adobe-Kundenunterstützung](https://helpx.adobe.com/contact.html){target="_blank"}.

**Was ist der Unterschied zwischen einem Adobe-Produktadministrator und einem Marketo Engage-Administrator?**

* &quot;Adobe Product Admin“ ist eine neue Rolle in der Marketo-Plattform.
* Die Rolle &quot;Adobe-Produktadministrator“ wird Benutzenden gewährt, die in Adobe Admin Console als Produktadministrator hinzugefügt wurden
* Adobe Product Admin ist eine schreibgeschützte Rolle und kann nicht bearbeitet oder aus Marketo Engage gelöscht werden.
* Adobe-Produktadministrator hat dieselben Rechte und Berechtigungen wie ein standardmäßiger Marketo-Administrator.
* Die Rolle eines Marketo Engage-Administrators ist weiterhin Admin und wird Benutzenden in Marketo Engage gewährt.
* Nur Benutzende mit der standardmäßigen Marketo-Administratorrolle werden in der Admin Console als Marketo-Produktadministrator zugewiesen.

**Gibt es Änderungen bei der Client-Unterstützung für die User Management-API?**

Ja. Wer in Adobe IMS integriert wurde, kann nicht alle vorhandenen Marketo User Management-APIs nutzen. Für Aktionen zum Einladen, Aktualisieren und Löschen von Benutzern sollten die [IMS-APIs](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} von Adobe verwendet werden. Für die Rollenverwaltung gelten weiterhin die Marketo User Management-APIs. Darüber hinaus gibt es keine weiteren Änderungen an der Client-Unterstützung der Marketo REST-API.

**An wen wenden wir uns, wenn wir mit IMS integriert sind, um Unterstützung zu erhalten?**

* Pre-User-Migration: Support-Fälle in der [Marketing Nation-Community](https://nation.marketo.com/t5/support/ct-p/Support) oder E-Mail-`customercare@marketo.com`.

* Migration nach der Benutzermigration: Fälle, in denen die Datei unterstützt wird, z[ B. in der Marketing Nation Community ](https://nation.marketo.com/t5/support/ct-p/Support) E-Mail-`customercare@marketo.com`.

* Abschluss der Migration nach dem Support: Produktsupport-Administratoren können Fälle über das Experience League Support-Portal einreichen.

Wenn Sie über Ultimate Success verfügen, haben Sie Zugriff auf den Admin Console Migration White Glove Service. Wenden Sie sich an das Adobe Account Team (Ihren Account Manager), um Hilfe zu erhalten.

**Wenn ich eine Adobe-Identität verwende, um auf andere Adobe-Programme zuzugreifen, kann ich diese verwenden, um auf Marketo zuzugreifen?**

Selbst wenn Sie andere Adobe-Produkte haben, können Sie erst dann mit Adobe Identity auf Marketo zugreifen, wenn das Abonnement zu IMS migriert wurde.

**Werden Marketo-Benutzerrollen (innerhalb von Arbeitsbereichen) in Adobe Admin Console verwaltet?**

Nein. Die Verwaltung von Benutzerrollen (innerhalb von Arbeitsbereichen) wird in Marketo Engage abgeschlossen.

**Ich bin Marketo-Administrator in einem integrierten IMS-Abonnement und habe keinen Zugriff auf Admin Console. Wie erhalte ich Zugriff?**

Jedes Adobe-System oder jeder Produktadministrator, das bzw. der Zugriff auf die Admin Console Ihres Unternehmens hat, kann Ihnen Zugriff gewähren. Wenn Sie sich nicht sicher sind, wer in Ihrem Unternehmen über Administratorrechte in der Konsole verfügt, wenden Sie sich an die [Adobe-Kundenunterstützung](https://helpx.adobe.com/contact.html){target="_blank"}.

**Wie würde ein Administrator Benutzer zu Marketo [!DNL Sales Connect] hinzufügen?**

Zwar wird es in Admin Console für [!DNL Sales Connect] eine Produktkarte geben, doch sollte Admin Console nicht zum Hinzufügen/Verwalten von Benutzenden verwendet werden. Über den folgenden Link können Administratoren Benutzer über Marketo [!DNL Sales Connect] verwalten: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Wo erhalte ich weitere Informationen über die Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/de/enterprise/admin-guide.html){target="_blank"}.

**Gehe ich immer noch zum Abschnitt Admin in Marketo, um Benutzerkontoänderungen für mein Konto vorzunehmen?**

Nein, Sie müssen zu „account.adobe.com[&#128279;](https://account.adobe.com){target="_blank"}.

**Wie funktioniert dies mit der universellen ID von Marketo?**

Diejenigen, die sich für Adobe Identity entschieden haben, können über den Abonnementschalter im Produkt nahtlos auf alle IMS-aktivierten Abonnements zugreifen.

**Funktioniert dies mit SSO?**

Ja. Die Marketo-Integration mit Adobe IMS unterstützt Benutzer mit universeller ID und SSO. SSO wird jetzt von Adobe IMS gesteuert und auf Unternehmensebene in der Adobe Admin Console eingerichtet. [Weitere Informationen finden Sie hier](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

**Ich wurde bereits zu Adobe Identity hinzugefügt und möchte jetzt SSO implementieren. Was soll ich tun?**

Wenn Sie Single Sign-On implementieren möchten und Ihr Abonnement in Adobe Identity integriert wurde, ohne dass SSO in der Adobe-Organisation implementiert ist, senden Sie ein Ticket an den [Marketo-Support](https://nation.marketo.com/){target="_blank"} und geben Sie das Thema als &quot;Marketo auf Admin Console, Implementierung von SSO“ an.

**Wie funktioniert die Geräteautorisierung?**

Adobe IMS unterstützt derzeit keine Geräteautorisierungsfunktion von Marketo.

**Ist es weiterhin möglich, die Funktion „Anmelden im Dialogfeld „Benutzer einladen“ zu verwenden, um die Anmeldung eines Benutzers aus seiner E-Mail eindeutig zu machen?**

Nein. Der Workflow zum Einladen von Benutzenden ist nicht mehr aktiv, wenn ein Abonnement IMS-aktiviert ist, sodass die Funktion nicht mehr gültig ist. Adobe-Identität erfordert, dass die Identität eines Benutzers von seiner E-Mail-Adresse gesteuert wird.

**Haben wir für Adobe IMS die Möglichkeit, Adobe ID, Enterprise ID oder Federated ID zu verwenden?**

Ja, Sie bestimmen den Identitätstyp, den Ihre Organisation unterstützen soll. Weitere Informationen finden Sie hier: [Identitätsübersicht](https://helpx.adobe.com/de/enterprise/using/identity.html) und hier: [Einrichten der Identität](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

**Welche Produktkarten werden in der Adobe Admin Console unterstützt?**

Die unterstützten Produktkarten sind: Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect und Marketo Sales Insight-Aktionen.

**Was passiert, wenn meine Benutzeranmeldung nicht mit meiner E-Mail-Adresse übereinstimmt, wenn ich zu einer Adobe-Identität migriert werde?**

Aktuelle Marketo Engage-Benutzer mit Anmeldungen, die sich von ihrer E-Mail-Adresse unterscheiden, melden sich nach der Migration zu einer Adobe-Identität nicht mehr mit diesen Anmeldedaten an. Adobe-Identitäten authentifizieren sich immer mit der E-Mail-Adresse eines Benutzers. Sie können eine Adobe-Identitäts-E-Mail-Adresse unter [account.adobe.com) ](https://account.adobe.com){target="_blank"}.

**Was passiert nach der Adobe-Identitätsmigration, wenn mein Abonnement IP-Einschränkungseinstellungen verwendet?**

Wenn Abonnements in Adobe Identity integriert werden, werden die IP-Einschränkungseinstellungen nicht in die Adobe Admin Console migriert. Zu den IP-Einschränkungseinstellungen von Marketo gehören das Zulassen des Zugriffs von bestimmten IP-Adressen und das Blockieren des Zugriffs auf bestimmte IP-Adressen. Derzeit unterstützt Adobe Identity Management System keine IP-Einschränkungsfunktionen.

Ab Mitte 2025 wird Adobe Identity Management System eine Funktion veröffentlichen, die nur bestimmte IP-Adressen zulässt. Dies ist eine Übergangslösung für Marketo-Benutzende, die diese Funktion derzeit verwenden. Benutzer, die diese Funktion derzeit verwenden, werden erst dann einer Benutzermigration unterzogen, wenn die Funktion veröffentlicht wurde. Sobald die Funktion bereitgestellt wurde, werden die Benutzer über die geplante Migration benachrichtigt. Weitere Informationen zur Funktion werden bereitgestellt, sofern verfügbar.

Benutzende, die derzeit die IP-Einschränkung verwenden und dadurch den Zugriff auf bestimmte Adressen blockieren, können diese Funktion nach der Migration zu Adobe Identity nicht mehr verwenden, da sie vom Adobe Identity Management System nicht unterstützt wird.

**Was passiert nach der Migration von Adobe Identity, wenn ich Benutzende mit einer Rolle habe, die die Option „Single Sign-On umgehen“ hat?**

Adobe Admin Console enthält ein standardmäßiges Business ID-Verzeichnis. Benutzende, die nicht zu den Domains gehören, die in Federated ID-Ordnern in einer Adobe-Organisation beansprucht werden, werden diesem Ordner mit dem Identitätstyp Adobe ID zugewiesen. Diese Benutzenden können auf Marketo Engage zugreifen, ohne Single Sign-On (SSO) verwenden zu müssen, und das Lizenzeigentum verbleibt beim Unternehmen, nicht bei den Einzelpersonen.

**Ich habe mehr als ein Abonnement, aber nicht alle haben Single Sign-On aktiviert. Was passiert nach der Migration von Adobe Identity?**

Wenn Abonnements in Adobe Identity integriert werden, wird Single Sign-On (SSO) auf Adobe-Organisationsebene eingerichtet. Dies bedeutet, dass SSO für alle Produktinstanzen in der Adobe-Organisation gilt. Wenn SSO eingerichtet wird, gilt dies für alle Marketo-Instanzen in dieser Adobe-Organisation. Zuvor wurde diese Einstellung von Marketo auf Instanzebene unterstützt. Dies wird vom Adobe Identity Management-System nicht unterstützt.

**Sind Änderungen an CNAMEs, SPF oder DKIM erforderlich, die wir derzeit für Marketo Engage nach der Adobe-Identitätsmigration verwenden?**

Nein, diese Konfigurationen haben keine Auswirkungen.

**Wie kann ich verhindern, dass Sitzungen abgehen?**

In [Erweiterte Einstellungen](https://helpx.adobe.com/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"} können Sie die gewünschte maximale Sitzungsdauer anpassen (Systemadministratorberechtigungen erforderlich). Es wird empfohlen, diese Einstellung nach der Produktmigration, aber vor der Benutzermigration festzulegen.

**Ich muss jetzt zu Experience Cloud navigieren, um auf Marketo Engage zuzugreifen. Gibt es eine Möglichkeit, diesen Fluss zu straffen?**

Ja. Sie können ein Browser-Lesezeichen für den Link erstellen, der nach dem Klicken auf die Schaltfläche **Launch** auf der Einstiegsseite der Marketo Engage-Instanz gestartet wird, um diese Seite künftig zu umgehen.

![](assets/faq-1.png)
