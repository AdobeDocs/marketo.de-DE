---
description: Adobe Identity Management-FAQ - Marketo-Dokumente - Produktdokumentation
title: Häufig gestellte Fragen zu Adobe Identity Management
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: 094a11f9544e0dba75167de229d78e8ff50cf6e8
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 3%

---

# Häufig gestellte Fragen zu Adobe Identity Management {#adobe-identity-management-faq}

**Was ist Adobe Identity?**

Adobe Identity Management System besteht aus drei Komponenten.

* [!DNL Adobe Identity Service]: Verarbeitet die Authentifizierung und Validierung des Endbenutzers, einschließlich Verband und Laufzeit Single-Sign-On (SSO).

* Adobe Admin Console: Die Admin Console bietet einen zentralen Speicherort für die Verwaltung von Adobe-Berechtigungen in Ihrem gesamten Unternehmen. Es verwaltet Benutzerverwaltung, Cloud Service, Berechtigungen für Desktop-Lizenzen, Verknüpfungskonfiguration und bietet Sicherheitsfunktionen zur Datenverlustvermeidung.

* Adobe User Management API (UMAPI): Ermöglicht Unternehmen die Verwaltung von Unternehmensbenutzern und Berechtigungen in der Adobe Admin Console auf API-Ebene.

**Wann werden bestehende Marketo Engage-Abonnements in IMS integriert?**

Bestehende Marketo-Abonnements werden im Laufe dieses Jahres auf das Adobe Identity Management-System migriert. Der Marketo-Support kann keine Aktualisierungen zur Adobe IMS-Migration bereitstellen. Das Adobe Account-Team wird in den kommenden Monaten mit dem voraussichtlichen Zeitplan Kontakt aufnehmen.

**Was ist der Unterschied zwischen einem Adobe Product Admin und einem Marketo Engage Admin?**

* Adobe Product Admin ist eine neue Rolle auf der Marketo-Plattform.
* Adobe Die Produktadministratorrolle wird Benutzern zugewiesen, die in Adobe Admin Console als Produktadministrator hinzugefügt wurden.
* Adobe Product Admin ist eine schreibgeschützte Rolle und kann weder bearbeitet noch aus dem Marketo Engage gelöscht werden.
* Adobe Product Admin hat dieselben Berechtigungen wie ein standardmäßiger Marketo Admin.
* Die Rolle des Marketo Engage-Admins ist weiterhin ein Administrator und wird einem Benutzer unter Marketo Engage zugewiesen.

**Gibt es Änderungen an der Benutzermanagement-API-Client-Unterstützung?**

Ja. Benutzer, die mit Adobe IMS integriert wurden, können nicht alle bestehenden Marketo User Management-APIs verwenden. Bei Einladungs-, Aktualisierungs- und Löschaktionen für Benutzer muss die Adobe [IMS-APIs](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} verwendet werden. Für die Rollenverwaltung gelten weiterhin die Marketo User Management-APIs. Darüber hinaus gibt es keine weiteren Änderungen an der Marketo REST API-Client-Unterstützung.

**Wen kontaktieren wir für Support, wenn wir mit IMS integriert sind?**

Sie folgen dem Standardverfahren für die Kontaktaufnahme [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

**Wenn ich eine Adobe Identity verwende, um auf andere Adobe-Anwendungen zuzugreifen, kann ich diese dann verwenden, um auf Marketo zuzugreifen?**

Selbst wenn Sie über andere Adobe-Produkte verfügen, können Sie erst mit Adobe Identity auf Marketo zugreifen, wenn das Abonnement zu IMS migriert wird.

**Werden Marketo-Benutzerrollen (innerhalb von Arbeitsbereichen) in Adobe Admin Console verwaltet?**

Nein. Die Benutzerrollenverwaltung (innerhalb von Arbeitsbereichen) wird im Marketo Engage abgeschlossen.

**Ich bin ein Marketo-Administrator in einem integrierten IMS-Abonnement und habe keinen Zugriff auf die Admin Console. Wie erhalte ich Zugriff?**

Jedes Adobe-System oder jeder Produktadministrator, der Zugriff auf die Admin Console Ihres Unternehmens hat, kann Ihnen Zugriff gewähren. Wenn Sie sich nicht sicher sind, wer in Ihrem Unternehmen über Administratorrechte in der Konsole verfügt, wenden Sie sich an [Adobe-Kundenunterstützung](https://helpx.adobe.com/contact.html){target="_blank"}.

**Wie kann ein Administrator Benutzer zu Marketo hinzufügen? [!DNL Sales Connect]?**

Während eine Produktkarte in der Admin Console für [!DNL Sales Connect], sollte Admin Console nicht zum Hinzufügen/Verwalten von Benutzern verwendet werden. Über den folgenden Link können Administratoren Benutzer über Marketo verwalten [!DNL Sales Connect]: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Wo erhalte ich weitere Informationen über die Adobe Admin Console?**

[https://helpx.adobe.com/de/enterprise/admin-guide.html](https://helpx.adobe.com/de/enterprise/admin-guide.html){target="_blank"}.

**Wechsele ich immer noch zum Admin-Bereich in Marketo, um Benutzerkontoänderungen für mein Konto vorzunehmen?**

Nein, Sie müssen zu [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Wie funktioniert dies mit der universellen ID von Marketo?**

Diejenigen, die mit einer Adobe-Identität ausgestattet sind, können über den Abonnementschalter im Produkt nahtlos auf alle IMS-fähigen Abonnements zugreifen.

**Funktioniert dies mit SSO?**

Ja. Die Marketo-Integration mit Adobe IMS unterstützt universelle ID-Benutzer und SSO. SSO wird jetzt von Adobe IMS gesteuert und auf Unternehmensebene in der Adobe Admin Console eingerichtet. [Weitere Informationen hier](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

**Wie funktioniert die Geräteregistrierung?**

Adobe IMS unterstützt derzeit keine Funktionen wie die Marketo-Funktion zur Geräteautorisierung.

**Ist es weiterhin möglich, die Funktion &quot;Anmelden im Dialogfeld &quot;Benutzer einladen&quot;zu verwenden, um die Anmeldung eines Benutzers von seiner E-Mail-Adresse aus eindeutig zu machen?**

Nein. Der Workflow Benutzereinladung ist nicht mehr aktiv, wenn ein Abonnement IMS-fähig ist, sodass die Funktion nicht mehr gültig ist. Die Adobe-Identität erfordert, dass die Identität eines Benutzers durch seine E-Mail-Adresse gesteuert wird.

**Haben wir für Adobe IMS die Möglichkeit, Adobe ID, Enterprise ID oder Federated ID zu verwenden?**

Ja, Sie bestimmen den Identitätstyp, den Ihre Organisation unterstützen soll. Weitere Informationen finden Sie hier: [Identitätsübersicht](https://helpx.adobe.com/enterprise/using/identity.html) und hier: [Einrichten der Identität](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

**Welche Produktkarten werden in der Adobe Admin Console unterstützt?**

Folgende Produktkarten werden unterstützt: Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect und Marketo Sales Insight-Aktionen.
