---
description: Adobe Identity Management-FAQ - Marketo-Dokumente - Produktdokumentation
title: Häufig gestellte Fragen zu Adobe Identity Management
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: ab1ea483998d6cb37277b18adf2c1d3371bb40e6
workflow-type: tm+mt
source-wordcount: '1202'
ht-degree: 0%

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

Anz. Die Benutzerrollenverwaltung (innerhalb von Arbeitsbereichen) wird im Marketo Engage abgeschlossen.

**Ich bin ein Marketo-Administrator in einem integrierten IMS-Abonnement und habe keinen Zugriff auf die Admin Console. Wie erhalte ich Zugriff?**

Jedes Adobe-System oder jeder Produktadministrator, der Zugriff auf die Admin Console Ihres Unternehmens hat, kann Ihnen Zugriff gewähren. Wenn Sie sich nicht sicher sind, wer in Ihrem Unternehmen über Administratorrechte in der Konsole verfügt, wenden Sie sich an [Adobe-Kundenunterstützung](https://helpx.adobe.com/contact.html){target="_blank"}.

**Wie kann ein Administrator Benutzer zu Marketo hinzufügen? [!DNL Sales Connect]?**

Während eine Produktkarte in der Admin Console für [!DNL Sales Connect], sollte Admin Console nicht zum Hinzufügen/Verwalten von Benutzern verwendet werden. Über den folgenden Link können Administratoren Benutzer über Marketo verwalten [!DNL Sales Connect]: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Wo erhalte ich weitere Informationen über die Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/de/enterprise/admin-guide.html){target="_blank"}.

**Wechsele ich immer noch zum Admin-Bereich in Marketo, um Benutzerkontoänderungen für mein Konto vorzunehmen?**

Nein, Sie müssen zu [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Wie funktioniert dies mit der universellen ID von Marketo?**

Diejenigen, die mit einer Adobe-Identität ausgestattet sind, können über den Abonnementschalter im Produkt nahtlos auf alle IMS-fähigen Abonnements zugreifen.

**Funktioniert dies mit SSO?**

Ja. Die Marketo-Integration mit Adobe IMS unterstützt universelle ID-Benutzer und SSO. SSO wird jetzt von Adobe IMS gesteuert und auf Unternehmensebene in der Adobe Admin Console eingerichtet. [Weitere Informationen hier](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

* **Ich bin bereits an Adobe Identity angeschlossen und möchte jetzt SSO implementieren. Was mache ich?**

Wenn Sie Single Sign-On implementieren möchten und Ihr Abonnement auf Adobe Identity integriert wurde, ohne dass SSO in der Adobe-Org implementiert ist, senden Sie bitte ein Ticket an [Marketo-Support](https://nation.marketo.com/){target="_blank"} und geben Sie das Thema als &quot;Marketo on Admin Console, implementieren von SSO&quot;an.

**Wie funktioniert die Geräteregistrierung?**

Adobe IMS unterstützt derzeit keine Funktionen wie die Marketo-Funktion zur Geräteautorisierung.

**Ist es weiterhin möglich, die Funktion &quot;Anmelden im Dialogfeld &quot;Benutzer einladen&quot;zu verwenden, um die Anmeldung eines Benutzers von seiner E-Mail-Adresse aus eindeutig zu machen?**

Anz. Der Workflow Benutzereinladung ist nicht mehr aktiv, wenn ein Abonnement IMS-fähig ist, sodass die Funktion nicht mehr gültig ist. Die Adobe-Identität erfordert, dass die Identität eines Benutzers durch seine E-Mail-Adresse gesteuert wird.

**Haben wir für Adobe IMS die Möglichkeit, Adobe ID, Enterprise ID oder Federated ID zu verwenden?**

Ja, Sie bestimmen den Identitätstyp, den Ihre Organisation unterstützen soll. Weitere Informationen finden Sie hier: [Identitätsübersicht](https://helpx.adobe.com/enterprise/using/identity.html) und hier: [Einrichten der Identität](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

**Welche Produktkarten werden in der Adobe Admin Console unterstützt?**

Folgende Produktkarten werden unterstützt: Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect und Marketo Sales Insight-Aktionen.

**Was passiert, wenn meine Benutzeranmeldung nicht mit meiner E-Mail übereinstimmt, wenn ich zu einer Adobe Identity migriert werde?**

Aktuelle Marketo-Benutzer mit anderen Anmeldungen als ihre E-Mail-Adresse melden sich nicht mehr mit dieser Berechtigung an, nachdem sie zu einer Adobe-Identität migriert wurden. Adobe Identitäten authentifizieren sich immer mit der E-Mail-Adresse eines Benutzers.

**Was passiert nach der Adobe Identity-Migration, wenn mein Abonnement IP-Einschränkungseinstellungen verwendet?**

Wenn Abonnements für Adobe Identity integriert sind, werden IP-Einschränkungseinstellungen nicht in die Adobe Admin Console migriert. Zu den IP-Einschränkungseinstellungen von Marketo gehören das Zulassen des Zugriffs nur von bestimmten IP-Adressen aus und das Blockieren des Zugriffs auf bestimmte IP-Adressen. Derzeit unterstützt das Adobe Identity Management-System keine IP-Einschränkungsfunktionen.

Im Jahr 2024 wird das Adobe Identity Management-System eine Funktion veröffentlichen, die nur bestimmte IP-Adressen unterstützt. Dadurch wird eine Umstellung für Marketo-Benutzer unterstützt, die diese Funktion derzeit nutzen. Diejenigen, die diese Funktion derzeit verwenden, werden erst dann einer Benutzermigration unterzogen, wenn die Funktion veröffentlicht wurde. Sobald die Funktion bereitgestellt wurde, werden die Benutzer über die geplante Migration informiert. Weitere Informationen über die Funktion werden bereitgestellt, sofern verfügbar.

Benutzer, die derzeit die IP-Beschränkung verwenden und bestimmte Adressen am Zugriff hindern, können diese Funktion nach der Migration zu Adobe Identity nicht mehr verwenden, da sie von Adobe Identity Management System nicht unterstützt wird.

**Was passiert nach der Adobe-Identitätsmigration, wenn ich Benutzer mit einer Rolle habe, die die Option &quot;Single Sign-On umgehen&quot;hat?**

Wenn Abonnements für Adobe Identity integriert sind, wird Single Sign-On (SSO) für alle Adobe-Benutzer auf Organisationsebene eingerichtet. Wenn SSO eingerichtet ist, wird sie für alle Marketo-Benutzer/alle Marketo-Instanzen in dieser Adobe-Organisation erzwungen. Zuvor hat Marketo unterstützt, dass eine Benutzerrolle so eingerichtet werden kann, dass sie die Option &quot;Single Sign-On umgehen&quot;hat. Dies wird vom Adobe Identity Management System nicht unterstützt.

**Ich habe mehr als ein Abonnement, aber nicht alle haben Single Sign On aktiviert. Was passiert nach der Adobe-Identitätsmigration?**

Wenn Abonnements für Adobe Identity integriert sind, wird Single Sign-On (SSO) auf der Ebene der Adobe-Organisation eingerichtet. Das bedeutet, dass SSO für alle Produktinstanzen in der Adobe-Org gilt. Wenn SSO eingerichtet ist, gilt dies für alle Marketo-Instanzen in dieser Adobe-Organisation. Zuvor unterstützte Marketo diese Einstellung auf Instanzenebene. Dies wird vom Adobe Identity Management System nicht unterstützt.
