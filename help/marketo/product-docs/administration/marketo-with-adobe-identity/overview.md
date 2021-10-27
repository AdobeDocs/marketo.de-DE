---
description: Übersicht - Marketo-Dokumente - Produktdokumentation
title: Überblick
hide: true
hidefromtoc: true
source-git-commit: 6047665cf94a4b212734667feeb5fce911ffdebb
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 1%

---

# Überblick {#overview}

Wenn Ihr Adobe Marketo Engage-Abonnement am oder nach dem 21.10.2019 bereitgestellt wurde, wird es in das Adobe Identity Management System integriert. Mit AIMS können Benutzer sich mit einer gemeinsamen Adobe Identity bei Marketo Engage und anderen Experience Cloud-Anwendungen anmelden.

## Profilebenen

Es gibt drei Profilebenen.

<table>
 <tr>
  <td><strong>Systemadministrator</strong></td>
  <td>Zuständig für die Einrichtung von Identitätskonzepten für die Adobe-Organisation und das Marketo Engage-Produkt in der Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Produkt-Admin</strong></td>
  <td>Zuständig für die Berechtigung von Benutzern für das Marketo Engage-Produkt in der Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Benutzer</strong></td>
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
* Es handelt sich um eine schreibgeschützte Rolle, die nicht in Marketo bearbeitet oder gelöscht werden kann.
* Sie hat dieselben Berechtigungen wie der standardmäßige Marketo-Administrator.

**Gibt es eine Änderung bei der API-Client-Unterstützung?**

Ja. Benutzer, die mit Adobe IMS integriert wurden, können die vorhandenen Marketo User Management-APIs nicht verwenden. Sie würden die [IMS-APIs](https://www.adobe.io/apis/experienceplatform/umapi-new.html).

**An wen wenden wir uns für Support?**

Sie folgen dem Standardverfahren für die Kontaktaufnahme mit dem [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support).

**Werden Marketo-Benutzerrollen (innerhalb von Arbeitsbereichen) in Adobe Admin Console verwaltet?**

Anz. Die Benutzerrollenverwaltung (innerhalb von Arbeitsbereichen) ist in Marketo abgeschlossen.

**Ich bin Marketo-Administrator und habe keinen Zugriff auf die Admin Console. Wie erhalte ich Zugriff?**

Jeder System- oder Produktadministrator, der Zugriff auf die Admin Console Ihres Unternehmens hat, kann Ihnen Zugriff gewähren. Wenn Sie sich nicht sicher sind, wer in Ihrem Unternehmen über Administratorrechte in der Konsole verfügt, wenden Sie sich an [Adobe-Kundenunterstützung](https://helpx.adobe.com/contact.html).

**Wie kann ein Administrator Benutzer zu Marketo Sales Connect hinzufügen?**

Es wird zwar eine Produktkarte in AC for Sales Connect geben, aber AC sollte nicht zum Hinzufügen/Verwalten von Benutzern verwendet werden. Über den folgenden Link können Administratoren Benutzer über Marketo Sales Connect verwalten: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management).

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

Ja, Sie bestimmen den Identitätstyp, den Ihre Organisation unterstützen soll. Weitere Infos [here](https://helpx.adobe.com/enterprise/using/identity.html) und [here](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

>[!MORELIKETHIS]
>
>* [Admin-Einrichtung](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md)
>* [Hinzufügen oder Entfernen eines Produkt-Admins](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md)
>* [Hinzufügen oder Entfernen von Benutzern](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md)

