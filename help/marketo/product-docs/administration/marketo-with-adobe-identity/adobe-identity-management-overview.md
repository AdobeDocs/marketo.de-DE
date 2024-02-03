---
description: Adobe Identity Management-Übersicht - Marketo-Dokumente - Produktdokumentation
title: Adobe Identity Management - Überblick
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: 6f9790c2243407f2622970d228c9de6be7697df6
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Adobe Identity Management - Überblick {#adobe-identity-management-overview}

Alle neuen Adobe Marketo Engage-Abonnements (31. Juli 2023 oder höher) sind in das Adobe Identity Management-System integriert. Bestehende Marketo-Abonnements werden derzeit bei Verlängerungs- und/oder Wiedervergabeereignissen in das Adobe Identity Management-System migriert. Migrationen außerhalb eines Erneuerungs- oder Neuvertragsereignisses werden derzeit nicht unterstützt.

>[!NOTE]
>
>Der Marketo-Support kann keine Aktualisierungen zur Adobe IMS-Migration bereitstellen. Das Adobe Account-Team wird in den kommenden Monaten mit dem voraussichtlichen Zeitplan Kontakt aufnehmen. Weitere Informationen finden Sie unter [diesem Artikel](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console.md){target="_blank"}, and the [Frequently Asked Questions](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

Bei Anmeldungen mit einer Adobe-Identität wird die Adobe Admin Console für die Benutzerverwaltung verwendet. Identitätsbezogene Konzepte wie Single Sign-On werden ebenfalls in der Admin Console verwaltet.

* Weitere Informationen zu [Adobe Admin Console](https://helpx.adobe.com/de/enterprise/using/admin-console.html){target="_blank"}.
* Weitere Informationen finden Sie [Einrichten Ihrer Adobe-Organisation für Ihr Marketo-Abonnement](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

>[!NOTE]
>
>Wenn Sie Single Sign-On implementieren möchten und Ihr Abonnement auf Adobe Identity integriert wurde, ohne dass SSO in der Adobe-Org implementiert ist, senden Sie bitte ein Ticket an [Marketo-Support](https://nation.marketo.com/){target="_blank"} und geben Sie das Thema als &quot;Marketo on Admin Console, implementieren von SSO&quot;an.

## Profilebenen {#profile-levels}

Adobe Marketo Engage-Abonnements, die im Adobe Identity Management System integriert sind, unterstützen verschiedene Profile. Im Folgenden finden Sie die Typen von Benutzerprofilen, die für diese Integration relevant sind.

<table>
 <tr>
  <td><strong>Adobe Admin Console-Systemadministrator</strong></td>
  <td>Verantwortlich für die Einrichtung von Identitätskonzepten für die Adobe-Organisation und das Marketo Engage-Produkt in der Adobe Admin Console. Rolle bei der Einrichtung der Adobe-Organisation.</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console Product Admin</strong></td>
  <td>Zuständig für die Berechtigung von Benutzern für das Marketo Engage-Produkt in der Adobe Admin Console. Rolle in Adobe Admin Console zugewiesen.</td>
 </tr>
 <tr>
  <td><strong>Adobe Admin Console-Produktprofiladministrator</strong></td>
  <td>Verantwortlich für die Verwaltung von Benutzern in einem Produktprofil. Benutzer können nicht außerhalb dieses spezifischen Profils verwaltet werden. Ein Produktprofiladministrator hat keinen Zugriff auf die Marketo-Anwendung, es sei denn, er wurde zum Produktprofil als Benutzer hinzugefügt. Ihre Rolle wäre weiterhin ein Standardbenutzer (Standardarbeitsbereich, wenn mehrere Arbeitsbereiche vorhanden sind).
</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage Product Admin</strong></td>
  <td>Eine Person, die Zugriff auf Marketo Engage mit Administratorrechten hat. Rolle in Marketo Engage, nicht in Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Marketo Engage User</strong></td>
  <td>Eine Person, die Zugang zu Marketo Engage hat. Keine Administratorberechtigungen.</td>
 </tr>
</table>

## FAQs {#faq}

Häufig gestellte Fragen [finden Sie hier .](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Admin-Einrichtung](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [Hinzufügen oder Entfernen eines Produkt-Admins](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [Hinzufügen oder Entfernen von Benutzern](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}
