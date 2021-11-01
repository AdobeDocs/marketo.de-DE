---
description: Übersicht - Marketo-Dokumente - Produktdokumentation
title: Überblick
hide: true
hidefromtoc: true
source-git-commit: 1161d193261af10aaa7658e747ff6500ad4179d0
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

# Überblick {#overview}

Wenn Ihr Adobe Marketo Engage-Abonnement am oder nach dem 21.10.2019 bereitgestellt wurde, wird es in das Adobe Identity Management System integriert. Diese Integration ermöglicht es Benutzern, sich mit einer gemeinsamen Adobe Identity bei Marketo Engage und anderen Experience Cloud-Anwendungen anzumelden.

## Profilebenen

Adobe Marketo Engage-Abonnements, die in der Adobe Identity Management System integriert sind, unterstützen verschiedene Profile. Im Folgenden finden Sie die Typen von Benutzerprofilen, die für diese Integration relevant sind.

<table>
 <tr>
  <td><strong>Adobe Admin Console-Systemadministrator</strong></td>
  <td>Zuständig für die Einrichtung von Identitätskonzepten für die Adobe-Organisation und das Marketo Engage-Produkt in der Adobe Admin Console. Rolle bei der Einrichtung der Adobe.</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console Product Admin</strong></td>
  <td>Zuständig für die Berechtigung von Benutzern für das Marketo Engage-Produkt in der Adobe Admin Console. Rolle in Adobe Admin Console zugewiesen.</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage Product Admin</strong></td>
  <td>Eine Person, der Zugriff auf Marketo Engage mit Administratorrechten gewährt wurde. Rolle in Marketo Engage zugewiesen, nicht in Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage User</strong></td>
  <td>Eine Person, der Zugang zum Marketo Engage gewährt wurde. Keine Administratorrechte.</td>
 </tr>
</table>

## FAQs

**Was ist Adobe Identity?**

Adobe Identity Management System besteht aus drei Komponenten.

* Adobe Identity-Dienst: Verarbeitet die Authentifizierung und Validierung des Endbenutzers, einschließlich Verband und Laufzeit Single-Sign-On (SSO).

* Adobe Admin Console: Die Admin Console bietet einen zentralen Speicherort für die Verwaltung von Berechtigungen für Adoben in Ihrem gesamten Unternehmen. Es verwaltet Benutzerverwaltung, Cloud Service, Berechtigungen für Desktop-Lizenzen, Verknüpfungskonfiguration und bietet Sicherheitsfunktionen zur Datenverlustvermeidung.

* Adobe User Management API (UMAPI): Ermöglicht Unternehmen die Verwaltung von Unternehmensbenutzern und -berechtigungen in der Adobe Admin Console auf API-Ebene.

**Was ist der Unterschied zwischen einem Adobe Product Admin und einem Marketo Engage Admin?**

* Adobe Product Admin ist eine neue Rolle auf der Marketo-Plattform.
* Adobe Product Admin-Rolle wird Benutzern zugewiesen, die in Adobe Admin Console als Produktadministrator hinzugefügt werden.
* Adobe Product Admin ist eine schreibgeschützte Rolle und kann nicht in Marketo Engage bearbeitet oder gelöscht werden.
* Adobe Product Admin hat dieselben Berechtigungen wie ein Marketo-Standardadministrator.
* Die Rolle des Marketo Engage-Administrators ist weiterhin ein Administrator und wird einem Benutzer in Marketo Engage zugewiesen.

**Gibt es eine Änderung bei der API-Client-Unterstützung?**

Ja. Benutzer, die mit Adobe IMS integriert wurden, können nicht alle bestehenden Marketo User Management-APIs verwenden. Bei Aktionen zum Einladen, Aktualisieren und Löschen von Benutzern muss die [IMS-APIs](https://www.adobe.io/apis/experienceplatform/umapi-new.html) verwendet werden. Für die Rollenverwaltung gelten weiterhin die Marketo User Management-APIs.

**An wen wenden wir uns für Support?**

Sie folgen dem Standardverfahren für die Kontaktaufnahme mit dem [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support).

**Werden Marketo-Benutzerrollen (innerhalb von Arbeitsbereichen) in Adobe Admin Console verwaltet?**

Anz. Die Benutzerrollenverwaltung (innerhalb von Arbeitsbereichen) ist in Marketo Engage abgeschlossen.

**Ich bin Marketo-Administrator und habe keinen Zugriff auf die Admin Console. Wie erhalte ich Zugriff?**

Jedes Adobe-System oder jeder Produktadministrator, der Zugriff auf die Admin Console Ihres Unternehmens hat, kann Ihnen Zugriff gewähren. Wenn Sie sich nicht sicher sind, wer in Ihrem Unternehmen über Administratorrechte in der Konsole verfügt, wenden Sie sich an [Adobe-Kundenunterstützung](https://helpx.adobe.com/contact.html).

**Wie kann ein Administrator Benutzer zu Marketo Sales Connect hinzufügen?**

Obwohl in Admin Console für Sales Connect eine Produktkarte vorhanden sein wird, sollte die Admin Console nicht zum Hinzufügen/Verwalten von Benutzern verwendet werden. Über den folgenden Link können Administratoren Benutzer über Marketo Sales Connect verwalten: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management).

**Wo erhalte ich weitere Informationen über die Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html).

**Wechsele ich immer noch zum Abschnitt &quot;Admin&quot;in Marketo, um Kontoänderungen vorzunehmen?**

Nein, Sie müssen zu [account.adobe.com](https://account.adobe.com).

**Wie funktioniert dies mit der universellen ID von Marketo?**

Diejenigen, die mit der Adobe-ID integriert sind, können über den Abonnementschalter im Produkt nahtlos auf alle IMS-fähigen Abonnements zugreifen.

**Funktioniert dies mit SSO?**

Ja. Die Marketo-Integration mit Adobe IMS unterstützt universelle ID-Benutzer und SSO. SSO wird jetzt von Adobe IMS gesteuert und auf Unternehmensebene in der Adobe Admin Console eingerichtet. [Weitere Informationen finden Sie hier](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

**Wie funktioniert die Geräteregistrierung?**

Adobe IMS unterstützt derzeit keine Funktionen wie die Marketo-Funktion zur Geräteregistrierung.

**Ist es weiterhin möglich, die Funktion &quot;Anmelden im Dialogfeld &quot;Benutzer einladen&quot;zu verwenden, um die Anmeldung von unserer E-Mail eindeutig zu machen?**

Anz. Der Workflow Benutzereinladung ist nicht mehr aktiv, wenn ein Abonnement IMS-fähig ist, sodass die Funktion nicht mehr gültig ist. Für die Identität einer Adobe muss die Identität eines Benutzers durch seine E-Mail-Adresse gesteuert werden.

**Haben wir für Adobe IMS die Möglichkeit, Adobe ID, Enterprise ID oder Federated ID zu verwenden?**

Ja, Sie bestimmen den Identitätstyp, den Ihre Organisation unterstützen soll. Weitere Informationen finden Sie hier: [Identitätsübersicht](https://helpx.adobe.com/enterprise/using/identity.html) und hier: [Einrichten der Identität](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

>[!MORELIKETHIS]
>
>* [Admin-Einrichtung](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md)
>* [Hinzufügen oder Entfernen eines Produkt-Admins](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md)
>* [Hinzufügen oder Entfernen von Benutzern](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md)

